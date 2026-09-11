# Migration Guide: clicksend-go (legacy) → clicksend-go-v2

This guide helps you migrate from the legacy ClickSend Go SDK (`github.com/ClickSend/clicksend-go`, package `clicksend`) to the current v2 SDK (`github.com/ClickSend/clicksend-go-v2`, also package `clicksend`). Both SDKs talk to the same ClickSend v3 REST API, but the calling convention, response shapes, and API groupings have all changed. Read this guide fully before upgrading — almost every call site in your existing integration will need to change, and because both packages share the import name `clicksend`, the compiler alone won't catch every difference.

## Contents

1. [Why this migration isn't a drop-in replacement](#1-why-this-migration-isnt-a-drop-in-replacement)
2. [Installation & imports](#2-installation--imports)
3. [Authentication & client setup](#3-authentication--client-setup)
4. [Base path / URL changes](#4-base-path--url-changes)
5. [Calling an endpoint: positional args → fluent builder](#5-calling-an-endpoint-positional-args--fluent-builder)
6. [Request payloads: builder + `*Request` models replace struct literals](#6-request-payloads-builder--request-models-replace-struct-literals)
7. [Response payloads: typed structs instead of raw strings](#7-response-payloads-typed-structs-instead-of-raw-strings)
8. [Error handling: same shape, no exceptions, but the type changed from a value to a pointer](#8-error-handling-same-shape-no-exceptions-but-the-type-changed-from-a-value-to-a-pointer)
9. [Removed: `*ApiXxxOpts` + `antihax/optional` — replaced by chained setters](#9-removed-apixxxopts--antihaxoptional--replaced-by-chained-setters)
10. [Service-by-service mapping (all 37 legacy services)](#10-service-by-service-mapping-all-37-legacy-services)
11. [Side-by-side examples for common operations](#11-side-by-side-examples-for-common-operations)
12. [The Voice naming trap (read this before touching voice code)](#12-the-voice-naming-trap-read-this-before-touching-voice-code)
13. [Endpoints/methods removed in v2](#13-endpointsmethods-removed-in-v2)
14. [Brand-new resources and methods in v2](#14-brand-new-resources-and-methods-in-v2)
15. [Step-by-step migration checklist](#15-step-by-step-migration-checklist)

## 1. Why this migration isn't a drop-in replacement

The legacy SDK grew organically against ClickSend's v3 API: one API service per literal URL path segment (37 `api_*.go` files, e.g. `AccountApi`, `AccountRechargeApi`, `EmailMarketingApi`, `MasterEmailTemplatesApi`, `UserEmailTemplatesApi`, `EmailDeliveryReceiptRulesApi` as five *separate* email-related services), methods named after `{PathSegment}{HTTPVerb}` (`SmsSendPost`, `SmsHistoryGet`), request bodies passed as reusable domain models directly as function arguments (`SmsMessage`, `SmsMessageCollection`), optional query parameters passed as a pointer to a generated `*ApiXxxOpts` struct built with the third-party `github.com/antihax/optional` package, and — critically — **every successful response typed as a plain `string`** (see [§7](#7-response-payloads-typed-structs-instead-of-raw-strings)).

The v2 SDK is generated fresh from ClickSend's current OpenAPI v3 specification for Go, which:

- Groups methods into **26 services instead of 37** — several legacy services were merged, the Account and Number services each split/gained a new group, and the Fax, Letters, Postcards, and address-detection services were dropped entirely (see [§13](#13-endpointsmethods-removed-in-v2)).
- Names methods after the endpoint's **operationId** (`SendSms`, `ViewSmsHistory`, `ExportSmsHistory`) instead of `{PathSegment}{Verb}`.
- Replaces direct positional calls with a **fluent request-builder pattern**: the top-level method returns a request-builder struct, you chain setter methods onto it, and call `.Execute()` to send it (see [§5](#5-calling-an-endpoint-positional-args--fluent-builder)).
- Wraps every request body in a dedicated, single-purpose `*Request` model instead of reusing broad domain models.
- Returns a **fully typed struct pointer** for every successful response instead of a raw, un-decoded JSON string.
- Renames the generic error type `GenericSwaggerError` → `GenericOpenAPIError`, and changes it from a returned **value** to a returned **pointer** (see [§8](#8-error-handling-same-shape-no-exceptions-but-the-type-changed-from-a-value-to-a-pointer)).
- Drops the `github.com/antihax/optional` dependency entirely — optional/query parameters are now plain typed chained setters (see [§9](#9-removed-apixxxopts--antihaxoptional--replaced-by-chained-setters)).
- Ships as a proper Go module (`go.mod`/`go.sum` committed, `go 1.23`) with a real import path, `github.com/ClickSend/clicksend-go-v2` — the legacy SDK has **no `go.mod` of its own at all** (see [§2](#2-installation--imports)).

What did **not** change: Go's error model. Neither SDK has exceptions — both legacy and v2 return the idiomatic Go 3-tuple `(result, *http.Response, error)` (or a 2-tuple for a few no-body v2 endpoints), and both already required a `context.Context` as the first argument on every call. If you're coming from the Python or Node migration guides in this repo, do not expect an exception hierarchy or an `async_req` flag here — those don't apply to Go and this guide does not force that narrative (see [§8](#8-error-handling-same-shape-no-exceptions-but-the-type-changed-from-a-value-to-a-pointer) and [§9](#9-removed-apixxxopts--antihaxoptional--replaced-by-chained-setters)).

None of this changes the underlying REST API — it's the same ClickSend v3 API — but it does change **every call site** in your existing integration.

## 2. Installation & imports

| | Legacy | v2 |
|---|---|---|
| Import path | `github.com/ClickSend/clicksend-go` | `github.com/ClickSend/clicksend-go-v2` |
| Go package name | `clicksend` | `clicksend` (same — see the warning below) |
| Module manifest | **none** — no `go.mod`, `go.sum`, `Gopkg.toml`, or `glide.yaml` anywhere in the legacy source tree | `go.mod` + `go.sum` committed, `module github.com/ClickSend/clicksend-go-v2`, `go 1.23` |
| Declared dependencies | `github.com/antihax/optional` (optional-param wrapper, used throughout `api_*.go`), `golang.org/x/oauth2` (imported in `client.go` for an OAuth2 context-value code path, unused by Basic-Auth callers) — neither is vendored or pinned by the legacy SDK itself | `gopkg.in/validator.v2` only |
| Version at time of writing | untagged / no `go.mod` version | `6.0.2` (per the `User-Agent` string baked into `configuration.go`) |

Because the legacy SDK ships with no `go.mod`, its own README documents installing it by copying the source into your project rather than `go get`-ing it as a module:

```sh
# Legacy README's documented approach — no go.mod means no real module path
# "Put the package under your project folder and add the following in import"
```
```go
import "./clicksend"
```

In practice, most real integrations today reference the legacy SDK one of two ways instead: vendoring the source directly under `vendor/` or a local subdirectory, or adding a `replace` directive in their own `go.mod` pointing at a specific commit SHA on GitHub (`replace github.com/ClickSend/clicksend-go => github.com/ClickSend/clicksend-go v0.0.0-<sha>`), since there is no tagged, versioned module to `go get` normally. Confirm which approach your project actually uses before you start removing it.

v2 is a proper Go module and installs the normal way:

```sh
go get github.com/ClickSend/clicksend-go-v2
```

```go
import clicksend "github.com/ClickSend/clicksend-go-v2"
```

**Both SDKs use the same Go package name, `clicksend`.** If your project currently imports the legacy SDK under an implicit `clicksend` identifier and you swap only the import path, the package name is identical, so `go build` will *not* flag the import line itself as wrong — it will instead fail (or worse, silently type-check against the wrong types if you have some transitional aliasing) at every call site whose method or type no longer exists. Do not rely on "the import still compiles" as a signal that the migration is complete; there is no cohabitation concern only because you should remove the legacy import entirely rather than run both.

## 3. Authentication & client setup

Client construction and HTTP Basic authentication are unchanged in spirit — this is the easy part of the migration:

```go
// Legacy
cfg := clicksend.NewConfiguration()
client := clicksend.NewAPIClient(cfg)

auth := context.WithValue(context.Background(), clicksend.ContextBasicAuth, clicksend.BasicAuth{
    UserName: username,
    Password: apiKey,
})
```

```go
// v2 — identical shape
cfg := clicksend.NewConfiguration()
client := clicksend.NewAPIClient(cfg)

auth := context.WithValue(context.Background(), clicksend.ContextBasicAuth, clicksend.BasicAuth{
    UserName: username,
    Password: apiKey,
})
```

Nothing about `Configuration`/`APIClient`/`BasicAuth` construction needs to change. What changes is:

- **Which field you call on `client`.** Legacy exposes 37 fields named after the URL path (`client.SMSApi`, `client.MMSApi`, `client.ContactApi`, …). v2 exposes 26 fields with a capitalized `API` suffix (`client.SmsAPI`, `client.MmsAPI`, `client.ContactsAPI`, …) — see the full field list in [§10](#10-service-by-service-mapping-all-37-legacy-services).
- **How you call the method on that field** — see [§5](#5-calling-an-endpoint-positional-args--fluent-builder).
- **Default `User-Agent`.** Legacy defaults to `Swagger-Codegen/1.0.0/go`; v2 defaults to `ClickSend-SDK/6.0.2/go`, settable via `cfg.UserAgent = "..."` in both SDKs (same field name).
- **`cfg.HTTPClient`** (a `*http.Client` for supplying your own timeouts/proxies/transport) exists on `Configuration` in both SDKs with the same field name — no change needed there.

## 4. Base path / URL changes

Legacy `Configuration` bakes the API version into a single string field:

```go
// Legacy
cfg := clicksend.NewConfiguration()
cfg.BasePath = "https://rest.clicksend.com/v3"   // this is also the default
```

v2 replaces `BasePath` with a `Servers` list (`[]ServerConfiguration`, supporting multiple servers and per-operation overrides), and the `/v3` prefix moves from the base path into each operation's individual path:

```go
// v2
cfg := clicksend.NewConfiguration()
cfg.Servers = clicksend.ServerConfigurations{
    {URL: "https://rest.clicksend.com"},   // this is also the default; no /v3 suffix
}
```

The final resolved URL is identical either way (`https://rest.clicksend.com/v3/sms/send`). This only matters if:

- **You set `cfg.BasePath` for a mock server or proxy.** Move that value to `cfg.Servers[0].URL` and **drop the `/v3` suffix** — otherwise every request becomes `.../v3/v3/sms/send`.
- **`cfg.Debug`** is new in v2 (`bool`, verbose request/response logging) and `cfg.OperationServers` (`map[string]ServerConfigurations`, per-endpoint server overrides) is also new — neither has a legacy equivalent.

## 5. Calling an endpoint: positional args → fluent builder

This is the single most impactful change in the whole migration, and the one most likely to require restructuring real code rather than a mechanical rename.

The legacy SDK calls a method directly with positional arguments and receives a plain 3-tuple back:

```go
// Legacy
result, httpResp, err := client.SMSApi.SmsSendPost(auth, clicksend.SmsMessageCollection{
    Messages: []clicksend.SmsMessage{
        {From: "MyBusiness", To: "+61411111111", Body: "Hello from ClickSend!", Source: "go-sdk"},
    },
})
```

v2's top-level method takes only `ctx` (and any required path parameters) and returns a **request-builder struct**, not the result. You chain setter methods onto that builder — starting with the request body, if there is one — and the call isn't actually sent until you call `.Execute()`:

```go
// v2
message := clicksend.NewSendSmsRequestMessagesInner("Hello from ClickSend!")
message.SetTo("+61411111111")
message.SetFrom("MyBusiness")
message.SetSource("go-sdk")

sendSmsRequest := clicksend.NewSendSmsRequest()
sendSmsRequest.SetMessages([]clicksend.SendSmsRequestMessagesInner{*message})

result, httpResp, err := client.SmsAPI.SendSms(auth).SendSmsRequest(*sendSmsRequest).Execute()
```

Points to note, confirmed directly against `api_sms.go`:

- `client.SmsAPI.SendSms(ctx)` returns an `ApiSendSmsRequest` struct (not a result) — its fields are `ctx`, `ApiService`, `contentType`, and `sendSmsRequest`, all unexported; you can only reach them through the chained setters.
- `.SendSmsRequest(sendSmsRequest SendSmsRequest)` sets the body and returns the same builder type, so calls chain.
- `.Execute()` is what actually performs the HTTP call — it's a thin wrapper that calls the service's own `SendSmsExecute(r)`, which does the real work and returns `(*SendSms, *http.Response, error)`.
- **Forgetting `.Execute()` is a compile error**, not a silent no-op — `client.SmsAPI.SendSms(auth).SendSmsRequest(*sendSmsRequest)` on its own is a value of type `ApiSendSmsRequest`, which doesn't satisfy whatever you assign it to. This fails safely, unlike, say, forgetting to await a promise in another language.
- The service field is `client.SmsAPI` — capitalized `API` suffix — not `client.SMSApi`.
- The operation is named after what it does (`SendSms`), not the literal path/verb (`SmsSendPost`).

For a `GET` with query parameters, the pattern is the same, minus a body setter, with query params as additional chained setters instead of an `Opts` struct (see [§9](#9-removed-apixxxopts--antihaxoptional--replaced-by-chained-setters)):

```go
// Legacy
opts := &clicksend.SMSApiSmsHistoryGetOpts{Page: optional.NewInt32(1), Limit: optional.NewInt32(50)}
result, httpResp, err := client.SMSApi.SmsHistoryGet(auth, opts)

// v2
result, httpResp, err := client.SmsAPI.ViewSmsHistory(auth).Page(1).Limit(50).Execute()
```

Every operation in v2 also exposes a `<Method>Execute(r Api<Method>Request)` function directly on the service (e.g. `SendSmsExecute`) — this is what `.Execute()` on the builder calls internally. You will not normally call it yourself, but it's useful to know it exists if you ever need to build and pass around a request object before executing it.

## 6. Request payloads: builder + `*Request` models replace struct literals

Legacy methods took a broad, reusable domain model directly as a struct-literal argument:

```go
// Legacy
sms := clicksend.SmsMessage{
    From:   "MyBusiness",
    To:     "+61411111111",
    Body:   "Hello from ClickSend!",
    Source: "go-sdk",
}
collection := clicksend.SmsMessageCollection{Messages: []clicksend.SmsMessage{sms}}
client.SMSApi.SmsSendPost(auth, collection)
```

`SmsMessage` fields are plain, non-pointer Go types (`From string`, `Body string`, `To string`, `Source string`, `Schedule int32`, `CustomString string`, `ListId int32`, `Country string`, `FromEmail string`), all tagged `omitempty` except `Body`.

v2 introduces **one dedicated `*Request` model per operation**, and its nested per-message model uses **pointer fields** so the SDK can distinguish "not set" from the zero value:

```go
// v2
message := clicksend.NewSendSmsRequestMessagesInner("Hello from ClickSend!")   // Body is required, passed to the constructor
message.SetTo("+61411111111")
message.SetFrom("MyBusiness")
message.SetSource("go-sdk")

sendSmsRequest := clicksend.NewSendSmsRequest()
sendSmsRequest.SetMessages([]clicksend.SendSmsRequestMessagesInner{*message})

client.SmsAPI.SendSms(auth).SendSmsRequest(*sendSmsRequest).Execute()
```

Practical implications:

- **The old domain-model class names mostly don't exist in v2.** `SmsMessage`, `SmsMessageCollection`, `Contact`, `ContactList`, `Subaccount`, etc. are gone. The `model_*.go` file count went from 47 to 383 — almost every model is named after a specific operation (`model_send_sms_request.go`, `model_create_new_contact_request.go`, …) rather than a domain noun, and nested list items get their own generated model too (e.g. `SendSmsRequestMessagesInner`, confirmed in `model_send_sms_request_messages_inner.go`).
- **Model fields are pointers.** `SendSmsRequestMessagesInner.From` is `*string` with `json:"from,omitempty"` (confirmed in `model_send_sms_request_messages_inner.go`) — the same field name as legacy's `From string`, just a pointer now. Prefer each model's `New*()` constructor plus `Set*()`/`Get*()`/`Has*()` accessor methods, as shown above — they handle the pointer wrapping for you. Struct-literal field assignment still works if you'd rather build the value directly, but then you need to wrap literals with the generated `Ptr*` helpers (`clicksend.PtrString(...)`, `clicksend.PtrInt32(...)`, `clicksend.PtrBool(...)`) or take the address of a local variable — a bare `&"MyBusiness"` isn't valid Go.
- **There is no keyword-collision or reserved-word renaming issue for the sender field the way some other languages have.** Both legacy and v2 simply call it `From` (legacy: `From string` / JSON `from`; v2: `From *string` / JSON `from,omitempty`). The only change is the pointer type, handled via `SetFrom(...)`.
- **`source` now defaults to `"sdk-go"`** on SMS, MMS, and voice message items if you never call `.SetSource(...)` — confirmed by the `var source string = "sdk-go"` line inside both `NewSendSmsRequestMessagesInner(...)` and `NewSendSmsRequestMessagesInnerWithDefaults()` in `model_send_sms_request_messages_inner.go` (and the equivalent MMS/voice model files). Legacy had no such default — `Source` was simply omitted from the JSON body if left as the zero value.
- **Collection wrapper types are gone.** `SmsMessageCollection{Messages: []SmsMessage{...}}` becomes `SendSmsRequest` with a `Messages []SendSmsRequestMessagesInner` field, set via `.SetMessages(...)`.
- Generic error responses are now modeled explicitly too (e.g. `Model400Error`), instead of you parsing the same shape out of a raw string by hand.

## 7. Response payloads: typed structs instead of raw strings

This is the most consequential change for anyone actually consuming ClickSend's data in Go. In the legacy SDK, **every single operation is declared to return `string`**:

```go
func (a *SMSApiService) SmsSendPost(ctx context.Context, smsMessages SmsMessageCollection) (string, *http.Response, error)
```

That `string` is not a message ID or a status flag — it is the **raw, un-decoded JSON response body**. The legacy client's internal `decode()` helper tries `json.Unmarshal(b, v)` against whatever target you gave it; when the target is `*string` and the body is a JSON object (which it always is for these endpoints), unmarshalling into a string fails, and the client falls back to copying the raw bytes in as-is (this fallback is visible directly in `client.go`):

```go
// legacy client.go
if err = json.Unmarshal(b, v); err != nil {
    if sp, ok := v.(*string); ok {
        *sp = string(b)
        return nil
    }
    return err
}
```

In practice this meant every caller of the legacy SDK had to `json.Unmarshal([]byte(result), &myStruct)` themselves to get structured data out — nothing in the return type documents the shape; you only learn it from the API reference docs.

v2 returns a fully typed struct pointer for every successful response:

```go
func (a *SmsAPIService) SendSmsExecute(r ApiSendSmsRequest) (*SendSms, *http.Response, error)
```

```go
result, httpResp, err := client.SmsAPI.SendSms(auth).SendSmsRequest(*sendSmsRequest).Execute()
if err != nil {
    // handle error — see §8
}
fmt.Println(result.Data.Messages[0].MessageId)   // typed field access, no unmarshalling
```

**Migration action:** find every place your code does `json.Unmarshal([]byte(result), ...)` (or ad-hoc string/byte digging) on a legacy call's return value, and replace it with direct field access on the struct v2 now returns. This is usually a net reduction in code, and the compiler will now catch a field-name typo that used to fail silently at runtime.

**Not every v2 endpoint returns a struct, though — check the signature, don't assume.** A handful of endpoints with no meaningful response body return `(*http.Response, error)` — a 2-tuple, no result value at all:

- `AlphaTagsAPIService.DeleteAlphaTagExecute` → `(*http.Response, error)`
- `DefaultSendersAPIService.DeleteDefaultSenderExecute` → `(*http.Response, error)`
- `UploadsAPIService.UploadAMediaFileExecute` → `(*http.Response, error)` (confirmed in `api_uploads.go` — even though this is a *create*, not a delete)
- `EmailAPIService.ExportEmailCampaignHistoryExecute` → `(*http.Response, error)`
- `ListsAPIService.ViewContactListsExecute` → `(*http.Response, error)` (this is the search-contacts-by-lists endpoint — see [§10](#10-service-by-service-mapping-all-37-legacy-services))

This isn't a "deletes have no body" rule — `DeleteSmsTemplate`, `DeleteContact`, `DeleteReturnAddress`, `DeleteSubaccount`, and `DeleteVoiceDeliveryReceiptRule` all still return a typed struct describing what was deleted, and `OwnNumbersAPIService.DeleteOwnNumberExecute` returns `(*OwnNumber, *http.Response, error)`. Check the actual function signature in the relevant `api_*.go` file (or `docs/<GroupName>API.md`) rather than assuming either way from the operation's name.

## 8. Error handling: same shape, no exceptions, but the type changed from a value to a pointer

Go has no exceptions in either SDK — both signal failure through the returned `error` value, exactly as idiomatic Go code does everywhere else. Both SDKs also expose a generic error type with the same three accessor methods, just renamed — **and the value/pointer-ness of the type itself changed, which is easy to get wrong in a type assertion:**

| | Legacy | v2 |
|---|---|---|
| Type name | `GenericSwaggerError` | `GenericOpenAPIError` |
| Returned as | **value** — `newErr := GenericSwaggerError{...}` | **pointer** — `newErr := &GenericOpenAPIError{...}` (confirmed throughout `api_sms.go` and `client.go`) |
| `.Error() string` | yes (value receiver) | yes (value receiver, but you'll be holding a pointer) |
| `.Body() []byte` | yes | yes |
| `.Model() interface{}` | yes | yes |

```go
// Legacy — type assertion on the VALUE type
result, httpResp, err := client.SMSApi.SmsSendPost(auth, collection)
if err != nil {
    if apiErr, ok := err.(clicksend.GenericSwaggerError); ok {
        fmt.Println("raw body:", string(apiErr.Body()))
    }
    return err
}

// v2 — type assertion on the POINTER type
result, httpResp, err := client.SmsAPI.SendSms(auth).SendSmsRequest(*sendSmsRequest).Execute()
if err != nil {
    if apiErr, ok := err.(*clicksend.GenericOpenAPIError); ok {
        fmt.Println("raw body:", string(apiErr.Body()))
    }
    fmt.Println(httpResp.StatusCode)
    return err
}
```

**A mechanical find-and-replace of `GenericSwaggerError` → `GenericOpenAPIError` is not enough** — `err.(clicksend.GenericOpenAPIError)` (no `*`) will silently fail the type assertion (`ok` will be `false`) against every real v2 error, because v2 always constructs and returns a `*GenericOpenAPIError`, never a bare value. Add the pointer.

v2 does **not** add status-specific error subclasses (no `BadRequestError`/`NotFoundError`/etc.) — there's a single `GenericOpenAPIError` for every non-2xx response in both SDKs, same as legacy. If you need to branch on status code, read `httpResp.StatusCode` from the second return value (always populated, in both SDKs, whenever the request actually reached the server) rather than trying to type-switch on the error. `client.go` in v2 does add a `formatErrorMessage` helper that enriches `.Error()`'s string with an RFC 7807 `title`/`detail` when the decoded error model has those fields — a readability improvement, not a new type to catch.

## 9. Removed: `*ApiXxxOpts` + `antihax/optional` — replaced by chained setters

Legacy endpoints with optional query parameters take a pointer to a generated `*ApiXxxOpts` struct whose fields are wrapped in the third-party `github.com/antihax/optional` package, which distinguishes "not provided" from the Go zero value:

```go
// Legacy
import "github.com/antihax/optional"

opts := &clicksend.SMSApiSmsHistoryGetOpts{
    Q:        optional.NewString("status:Sent"),
    DateFrom: optional.NewInt32(1700000000),
    Page:     optional.NewInt32(1),
    Limit:    optional.NewInt32(50),
}
result, httpResp, err := client.SMSApi.SmsHistoryGet(auth, opts)
```

v2 has **no `Opts` struct and no `antihax/optional` dependency at all** — every optional parameter is a plain, typed, chained setter method on the request builder introduced in [§5](#5-calling-an-endpoint-positional-args--fluent-builder):

```go
// v2
result, httpResp, err := client.SmsAPI.ViewSmsHistory(auth).
    Q("status:Sent").
    DateFrom(1700000000).
    Page(1).
    Limit(50).
    Execute()
```

Only call the setters you actually need — an unset field is simply omitted from the request, the same behavior as leaving a legacy `Opts` field at its zero value. This is the structural replacement for the whole `antihax/optional` import in your code: delete it, and convert every `Opts{...}` literal into a setter chain. Confirmed present on every list/history-style v2 endpoint, e.g. `ApiViewSmsHistoryRequest` in `api_sms.go` exposes `Page`, `Limit`, `Q`, `OrderBy`, `DateFrom`, `DateTo` as chained setters.

**On concurrency:** neither SDK has an `async_req`-style thread-pool flag — that concept doesn't exist in either the legacy or the v2 Go SDK, and both already require an explicit `context.Context` on every call (confirmed: legacy's `SmsSendPost(ctx context.Context, ...)` already takes `ctx` as the first argument, exactly like v2's `SendSms(ctx context.Context)`). If you need concurrent calls, use goroutines and your own synchronization in both SDKs — that was already true before this migration and remains the idiomatic Go approach; nothing about v2 changes it. Likewise, per-call timeouts/cancellation in both SDKs come from the `context.Context` you pass in (`context.WithTimeout(...)`), not from a per-call SDK parameter — v2 does not add an equivalent to other languages' `_request_timeout` kwarg.

## 10. Service-by-service mapping (all 37 legacy services)

v2 consolidates the legacy SDK's 37 `api_*.go` services (named after URL path segments) into **26** services (named after resource/capability), confirmed by direct file listing of both source trees. Some legacy services merged, the Account and Number services each partly split off a new group, and Fax/Letters/Postcards/address-detection were dropped entirely (see [§13](#13-endpointsmethods-removed-in-v2)) — and, critically, the two Voice services **swapped roles** in v2 naming (see [§12](#12-the-voice-naming-trap-read-this-before-touching-voice-code)).

| Legacy service (`client.<Field>`) | → | v2 service (`client.<Field>`) | Notes |
|---|---|---|---|
| `AccountApi` | → | `ManagementAPI`, `VerificationAPI` | Split: `AccountGet`/`AccountUseageBySubaccountGet` → `ManagementAPI`; `ForgotPasswordPut`/`ForgotUsernamePut` → `VerificationAPI`. 4 methods have no v2 equivalent — see [§13](#13-endpointsmethods-removed-in-v2). |
| `AccountRechargeApi` | → | `TransactionsAPI` | Renamed 1:1 (6 methods). |
| `ContactApi` | → | `ContactsAPI`, `ListsAPI` | Split: single-contact-by-id CRUD (`ListsContactsByListIdAndContactId{Get,Put,Delete}`) → `ContactsAPI`; list-scoped contact ops (create/list/copy/transfer/remove-opted-out) → `ListsAPI`. |
| `ContactListApi` | → | `ListsAPI` | Merged into `ListsAPI`. |
| `CountriesApi` | → | `InternationalMessagingAPI` | `CountriesGet` → `ListCountries`. |
| `DeliveryIssuesApi` | → | `MessageDeliveryAPI` | Renamed 1:1 (2 methods). |
| `DetectAddressApi` | → | _(removed)_ | Address detection has no v2 equivalent — see [§13](#13-endpointsmethods-removed-in-v2). |
| `EmailDeliveryReceiptRulesApi` | → | `EmailAPI` | Folded into the unified `EmailAPI`. |
| `EmailMarketingApi` | → | `EmailAPI` | Folded into the unified `EmailAPI`. |
| `EmailToSmsApi` | → | `EmailToSmsAPI` | Same name, methods renamed (7 → 7). |
| `FAXApi` | → | _(removed)_ | Fax is not part of the v2 SDK — see [§13](#13-endpointsmethods-removed-in-v2). |
| `FAXDeliveryReceiptRulesApi` | → | _(removed)_ | Fax is not part of the v2 SDK. |
| `GlobalSendingApi` | → | `InternationalMessagingAPI` | Folded in (4 methods). |
| `InboundFAXRulesApi` | → | _(removed)_ | Fax is not part of the v2 SDK. |
| `InboundSMSRulesApi` | → | `SmsAPI` | Folded in as `*SmsInboundAutomation(s)`. |
| `MMSApi` | → | `MmsAPI` | 4 of 6 methods carried over; 2 dropped — see [§13](#13-endpointsmethods-removed-in-v2). |
| `MasterEmailTemplatesApi` | → | `EmailAPI` | Folded into the unified `EmailAPI`. |
| `MmsCampaignApi` | → | `MmsCampaignsAPI` | Renamed 1:1 (6 methods). |
| `NumberApi` | → | `NumbersAPI` (+ `OwnNumbersAPI`) | Renamed 1:1 (3 methods) plus a brand-new `RegisterNumbers`; own-number verification is a wholly new `OwnNumbersAPI` group — see [§14](#14-brand-new-resources-and-methods-in-v2). |
| `PostLetterApi` | → | _(removed)_ | Letters is not part of the v2 SDK. |
| `PostPostcardApi` | → | _(removed)_ | Postcards is not part of the v2 SDK. |
| `PostReturnAddressApi` | → | `AddressesAPI` | Renamed 1:1 (5 methods) — still present even though letters/postcards are not. |
| `ReferralAccountApi` | → | `ReferralsAPI` | `ReferralAccountsGet` → `ViewReferralAccounts`. |
| `ResellerAccountApi` | → | `ResellerAPI` | Merged with `TransferCreditApi`. |
| `SMSApi` | → | `SmsAPI` | Renamed 1:1 for all 18 core methods. |
| `SMSDeliveryReceiptRulesApi` | → | `SmsAPI` | Folded in as `*SmsDeliveryReceiptRule(s)`. |
| `SearchApi` | → | `ListsAPI` | `SearchContactsListsGet` → `ViewContactLists`. |
| `SmsCampaignApi` | → | `SmsCampaignsAPI` | Renamed 1:1 (6 methods). |
| `StatisticsApi` | → | `StatisticsAPI` | Same name: `StatisticsSmsGet` → `ViewSmsStatistics`, `StatisticsVoiceGet` → `ViewVoiceStatistics`. |
| `SubaccountApi` | → | `SubaccountsAPI` | Renamed 1:1 (6 methods). |
| `TimezonesApi` | → | `InternationalMessagingAPI` | `TimezonesGet` → `Timezones`. |
| `TransactionalEmailApi` | → | `EmailAPI` | Folded into the unified `EmailAPI`. |
| `TransferCreditApi` | → | `ResellerAPI` | Merged with `ResellerAccountApi`; `ResellerTransferCreditPut` → `ResellerTransferCredit`. |
| `UploadApi` | → | `UploadsAPI` | `UploadsPost` → `UploadAMediaFile` (now returns no body — see [§7](#7-response-payloads-typed-structs-instead-of-raw-strings)). |
| `UserEmailTemplatesApi` | → | `EmailAPI` | Folded into the unified `EmailAPI`. |
| `VoiceApi` (send/history/price/lang/cancel/receipts) | → | **`VoiceMessagingAPI`** | ⚠️ See [§12](#12-the-voice-naming-trap-read-this-before-touching-voice-code) — this is *not* the new `VoiceAPI`. 2 methods dropped — see [§13](#13-endpointsmethods-removed-in-v2). |
| `VoiceDeliveryReceiptRulesApi` | → | **`VoiceAPI`** | ⚠️ See [§12](#12-the-voice-naming-trap-read-this-before-touching-voice-code) — the new `VoiceAPI` only has delivery-receipt-rule methods. |

`AlphaTagsAPI`, `DefaultSendersAPI`, `OwnNumbersAPI`, and `UrlShorteningAPI` in v2 have **no legacy predecessor at all** — see [§14](#14-brand-new-resources-and-methods-in-v2).

### Email: five legacy services → `EmailAPI` (33 methods, 1:1 coverage)

| Legacy | v2 (`EmailAPI`) |
|---|---|
| `TransactionalEmailApi.EmailSendPost` | `SendEmail` |
| `TransactionalEmailApi.EmailHistoryGet` | `ViewEmailHistory` |
| `TransactionalEmailApi.EmailHistoryExportGet` | `ExportEmailHistory` |
| `TransactionalEmailApi.EmailPricePost` | `CalculateEmailPrice` |
| `EmailMarketingApi.EmailCampaignPost` | `SendEmailCampaign` |
| `EmailMarketingApi.EmailCampaignsGet` | `ViewAllEmailCampaigns` |
| `EmailMarketingApi.EmailCampaignGet` | `ViewEmailCampaign` |
| `EmailMarketingApi.EmailCampaignPut` | `UpdateEmailCampaign` |
| `EmailMarketingApi.CancelEmailCampaignPut` | `CancelEmailCampaign` |
| `EmailMarketingApi.EmailCampaignPricePost` | `CalculateEmailCampaignPrice` |
| `EmailMarketingApi.EmailCampaignHistoryGet` | `ViewEmailCampaignHistory` |
| `EmailMarketingApi.EmailCampaignHistoryExportGet` | `ExportEmailCampaignHistory` (now returns `(*http.Response, error)`, no body — see [§7](#7-response-payloads-typed-structs-instead-of-raw-strings)) |
| `EmailMarketingApi.AllowedEmailAddressGet` | `ViewAllowedEmailAddresses` |
| `EmailMarketingApi.AllowedEmailAddressPost` | `CreateAllowedEmailAddress` |
| `EmailMarketingApi.SpecificAllowedEmailAddressGet` | `ViewAllowedEmailAddress` |
| `EmailMarketingApi.SpecificAllowedEmailAddressDelete` | `DeleteAllowedEmailAddress` |
| `EmailMarketingApi.VerifyAllowedEmailAddressGet` | `VerifyAllowedEmailAddress` |
| `EmailMarketingApi.SendVerificationTokenGet` | `SendEmailVerificationToken` |
| `UserEmailTemplatesApi.EmailTemplatesGet` | `ViewEmailTemplates` |
| `UserEmailTemplatesApi.EmailTemplateGet` | `ViewEmailTemplate` |
| `UserEmailTemplatesApi.EmailTemplatePost` | `CreateEmailTemplate` |
| `UserEmailTemplatesApi.EmailTemplatePut` | `UpdateEmailTemplate` |
| `UserEmailTemplatesApi.EmailTemplateDelete` | `DeleteEmailTemplate` |
| `MasterEmailTemplatesApi.MasterEmailTemplatesGet` | `ViewMasterEmailTemplates` |
| `MasterEmailTemplatesApi.MasterEmailTemplateGet` | `ViewMasterEmailTemplate` |
| `MasterEmailTemplatesApi.MasterEmailTemplateCategoriesGet` | `ViewTemplateCategories` |
| `MasterEmailTemplatesApi.MasterEmailTemplateCategoryGet` | `ViewTemplateCategory` |
| `MasterEmailTemplatesApi.MasterEmailTemplatesInCategoryGet` | `ViewTemplatesInCategory` |
| `EmailDeliveryReceiptRulesApi.EmailDeliveryReceiptAutomationsGet` | `ViewEmailDeliveryReceiptRules` |
| `EmailDeliveryReceiptRulesApi.EmailDeliveryReceiptAutomationGet` | `ViewEmailDeliveryReceiptRule` |
| `EmailDeliveryReceiptRulesApi.EmailDeliveryReceiptAutomationPost` | `CreateEmailDeliveryReceiptRule` |
| `EmailDeliveryReceiptRulesApi.EmailDeliveryReceiptAutomationPut` | `UpdateEmailDeliveryReceiptRule` |
| `EmailDeliveryReceiptRulesApi.EmailDeliveryReceiptAutomationDelete` | `DeleteEmailDeliveryReceiptRule` |

### SMS: `SMSApi` + `InboundSMSRulesApi` + `SMSDeliveryReceiptRulesApi` → `SmsAPI` (28 legacy methods → 30 v2 methods)

| Legacy | v2 (`SmsAPI`) |
|---|---|
| `SMSApi.SmsSendPost` | `SendSms` |
| `SMSApi.SmsHistoryGet` | `ViewSmsHistory` |
| `SMSApi.SmsHistoryExportGet` | `ExportSmsHistory` |
| `SMSApi.SmsPricePost` | `CalculateSmsPrice` |
| `SMSApi.SmsCancelAllPut` | `CancelAllSms` |
| `SMSApi.SmsCancelByMessageIdPut` | `CancelSms` |
| `SMSApi.SmsInboundGet` | `ViewInboundSms` |
| `SMSApi.SmsInboundPost` | `CreateTestInboundSms` |
| `SMSApi.SmsInboundReadPut` | `MarkInboundSmsAsRead` |
| `SMSApi.SmsInboundReadByMessageIdPut` | `MarkSpecificInboundSmsMessageAsRead` |
| `SMSApi.SmsReceiptsGet` | `ViewSmsReceipts` |
| `SMSApi.SmsReceiptsByMessageIdGet` | `ViewSpecificSmsReceipt` |
| `SMSApi.SmsReceiptsPost` | `CreateTestSmsReceipt` |
| `SMSApi.SmsReceiptsReadPut` | `MarkSmsReceiptAsRead` |
| `SMSApi.SmsTemplatesGet` | `ViewSmsTemplates` |
| `SMSApi.SmsTemplatesPost` | `CreateSmsTemplate` |
| `SMSApi.SmsTemplatesByTemplateIdPut` | `UpdateSmsTemplate` |
| `SMSApi.SmsTemplatesByTemplateIdDelete` | `DeleteSmsTemplate` |
| `InboundSMSRulesApi.SmsInboundAutomationsGet` | `ViewSmsInboundAutomations` |
| `InboundSMSRulesApi.SmsInboundAutomationGet` | `ViewSmsInboundAutomation` |
| `InboundSMSRulesApi.SmsInboundAutomationPost` | `CreateSmsInboundAutomation` |
| `InboundSMSRulesApi.SmsInboundAutomationPut` | `UpdateSmsInboundAutomation` |
| `InboundSMSRulesApi.SmsInboundAutomationDelete` | `DeleteSmsInboundAutomation` |
| `SMSDeliveryReceiptRulesApi.SmsDeliveryReceiptAutomationsGet` | `ViewSmsDeliveryReceiptRules` |
| `SMSDeliveryReceiptRulesApi.SmsDeliveryReceiptAutomationGet` | `ViewSmsDeliveryReceiptRule` |
| `SMSDeliveryReceiptRulesApi.SmsDeliveryReceiptAutomationPost` | `CreateSmsDeliveryReceiptRule` |
| `SMSDeliveryReceiptRulesApi.SmsDeliveryReceiptAutomationPut` | `UpdateSmsDeliveryReceiptRule` |
| `SMSDeliveryReceiptRulesApi.SmsDeliveryReceiptAutomationDelete` | `DeleteSmsDeliveryReceiptRule` |
| — | `ViewASpecificSmsTemplate` *(new — see [§14](#14-brand-new-resources-and-methods-in-v2))* |
| — | `ViewASpecificInboundSmsMessage` *(new — see [§14](#14-brand-new-resources-and-methods-in-v2))* |

### Contacts & lists: `ContactApi` + `ContactListApi` + `SearchApi` → `ContactsAPI` + `ListsAPI`

| Legacy | v2 | Notes |
|---|---|---|
| `ContactApi.ListsContactsByListIdAndContactIdGet(ctx, listId int32, contactId int32)` | `ContactsAPI.GetSpecificContact(ctx, listId string, contactId string)` | `listId`/`contactId` change from `int32` to `string`. |
| `ContactApi.ListsContactsByListIdAndContactIdPut` | `ContactsAPI.UpdateContact` | Same type change. |
| `ContactApi.ListsContactsByListIdAndContactIdDelete` | `ContactsAPI.DeleteContact` | Same type change. |
| `ContactApi.ListsContactsByListIdPost(ctx, contact Contact, listId int32)` | `ListsAPI.CreateNewContact(ctx, listId string)` + `.CreateNewContactRequest(...)` builder | Argument order and type both changed — `listId` is now the trailing positional arg (still required), and the payload moved to the builder. |
| `ContactApi.ListsContactsByListIdGet` | `ListsAPI.ViewListContacts(ctx, listId string)` | **Pagination params dropped** — no `Page`/`Limit`/`updated_after` setter exists on `ApiViewListContactsRequest` (confirmed: its only fields are `ctx`, `listId`, `contentType`). |
| `ContactApi.ListsCopyContactPut(ctx, fromListId, contactId, toListId int32)` | `ListsAPI.CopyContactToList(ctx, fromListId, contactId, toListId string)` | Same 3-arg order, `int32` → `string`. |
| `ContactApi.ListsTransferContactPut` | `ListsAPI.TransferContactToList` | Same 3-arg order, `int32` → `string`. |
| `ContactApi.ListsRemoveOptedOutContactsByListIdAndOptOutListIdPut` | `ListsAPI.RemoveOptedOutContacts` | Same 2-arg order, `int32` → `string`. |
| `ContactListApi.ListsGet` | `ListsAPI.ViewLists` | **Pagination params dropped** — `ApiViewListsRequest` has no `Page`/`Limit` setters at all. |
| `ContactListApi.ListsPost` | `ListsAPI.CreateList` | |
| `ContactListApi.ListsByListIdGet` | `ListsAPI.ViewSpecificList` | |
| `ContactListApi.ListsByListIdPut` | `ListsAPI.UpdateList` | |
| `ContactListApi.ListsByListIdDelete` | `ListsAPI.DeleteList` | |
| `ContactListApi.ListsImportByListIdPost` | `ListsAPI.ImportContacts` | |
| `ContactListApi.ListsRemoveDuplicatesByListIdPut` | `ListsAPI.RemoveDuplicateContacts` | |
| `SearchApi.SearchContactsListsGet` | `ListsAPI.ViewContactLists` | **Search functionality is not gone** — it maps directly to `ViewContactLists`, which takes a `Q(q string)` setter. It returns `(*http.Response, error)` in v2 (no typed body) — see [§7](#7-response-payloads-typed-structs-instead-of-raw-strings). |

### Account & billing

| Legacy | v2 |
|---|---|
| `AccountApi.AccountGet` | `ManagementAPI.ViewAccountDetails` |
| `AccountApi.AccountUseageBySubaccountGet(ctx, year int32, month int32)` | `ManagementAPI.ViewAccountUsage(ctx, year string, month string)` |
| `AccountApi.ForgotPasswordPut` | `VerificationAPI.ForgotPassword` |
| `AccountApi.ForgotUsernamePut` | `VerificationAPI.ForgotUsername` |
| `AccountRechargeApi.RechargeCreditCardGet` | `TransactionsAPI.CurrentPaymentInfo` |
| `AccountRechargeApi.RechargeCreditCardPut` | `TransactionsAPI.UpdatePaymentInfo` |
| `AccountRechargeApi.RechargePackagesGet` | `TransactionsAPI.ViewRechargePackages` |
| `AccountRechargeApi.RechargePurchaseByPackageIdPut` | `TransactionsAPI.PurchaseRechargePackage` |
| `AccountRechargeApi.RechargeTransactionsGet` | `TransactionsAPI.ViewAllTransactions` |
| `AccountRechargeApi.RechargeTransactionsByTransactionIdGet` | `TransactionsAPI.ViewSpecificTransaction` |
| `ResellerAccountApi.ResellerAccountsGet` | `ResellerAPI.ViewClientAccounts` |
| `ResellerAccountApi.ResellerAccountsPost` | `ResellerAPI.CreateResellerAccount` |
| `ResellerAccountApi.ResellerAccountsByClientUserIdGet` | `ResellerAPI.ViewSpecificClientAccount` |
| `ResellerAccountApi.ResellerAccountsByClientUserIdPut` | `ResellerAPI.UpdateClientAccount` |
| `TransferCreditApi.ResellerTransferCreditPut` | `ResellerAPI.ResellerTransferCredit` |
| `SubaccountApi.SubaccountsGet` | `SubaccountsAPI.ViewSubaccounts` |
| `SubaccountApi.SubaccountsPost` | `SubaccountsAPI.CreateSubaccount` |
| `SubaccountApi.SubaccountsBySubaccountIdGet` | `SubaccountsAPI.ViewSpecificSubaccount` |
| `SubaccountApi.SubaccountsBySubaccountIdPut` | `SubaccountsAPI.UpdateSubaccount` |
| `SubaccountApi.SubaccountsBySubaccountIdDelete` | `SubaccountsAPI.DeleteSubaccount` |
| `SubaccountApi.SubaccountsRegenApiKeyBySubaccountIdPut` | `SubaccountsAPI.GenerateNewApiKey` |
| `ReferralAccountApi.ReferralAccountsGet` | `ReferralsAPI.ViewReferralAccounts` |

### Numbers, addresses, uploads, international, delivery issues

| Legacy | v2 |
|---|---|
| `NumberApi.NumbersGet` | `NumbersAPI.ViewYourNumbers` |
| `NumberApi.NumbersSearchByCountryGet` | `NumbersAPI.ViewAvailableNumbers` |
| `NumberApi.NumbersBuyByDedicatedNumberPost` | `NumbersAPI.PurchaseDedicatedNumber` |
| `PostReturnAddressApi.PostReturnAddressesGet` | `AddressesAPI.ViewYourReturnAddresses` |
| `PostReturnAddressApi.PostReturnAddressesPost` | `AddressesAPI.CreateReturnAddress` |
| `PostReturnAddressApi.PostReturnAddressesByReturnAddressIdGet` | `AddressesAPI.ViewSpecificReturnAddress` |
| `PostReturnAddressApi.PostReturnAddressesByReturnAddressIdPut` | `AddressesAPI.UpdateReturnAddress` |
| `PostReturnAddressApi.PostReturnAddressesByReturnAddressIdDelete` | `AddressesAPI.DeleteReturnAddress` |
| `UploadApi.UploadsPost(ctx, uploadFile UploadFile, convert string)` | `UploadsAPI.UploadAMediaFile(ctx).Body(map[string]interface{}{...})` | payload is now a generic `map[string]interface{}` body via the builder, not a typed `UploadFile{Content: "..."}` struct, and it returns no body (see [§7](#7-response-payloads-typed-structs-instead-of-raw-strings)) |
| `CountriesApi.CountriesGet` | `InternationalMessagingAPI.ListCountries` |
| `TimezonesApi.TimezonesGet` | `InternationalMessagingAPI.Timezones` |
| `GlobalSendingApi.ListCountriesGet` | `InternationalMessagingAPI.GetCountriesForGlobalSending` |
| `GlobalSendingApi.UserCountriesGet` | `InternationalMessagingAPI.ViewCountries` |
| `GlobalSendingApi.UserCountriesPost` | `InternationalMessagingAPI.SelectCountriesForGlobalSending` |
| `GlobalSendingApi.UserCountriesAgreePost` | `InternationalMessagingAPI.AgreeToRulesAndRegulation` |
| `DeliveryIssuesApi.DeliveryIssuesGet` | `MessageDeliveryAPI.GetAllDeliveryIssues` |
| `DeliveryIssuesApi.DeliveryIssuesPost` | `MessageDeliveryAPI.CreateDeliveryIssue` |

### MMS, campaigns, voice, statistics

| Legacy | v2 |
|---|---|
| `MMSApi.MmsSendPost` | `MmsAPI.SendMms` |
| `MMSApi.MmsHistoryGet` | `MmsAPI.ViewMmsHistory` |
| `MMSApi.MmsHistoryExportGet` | `MmsAPI.ExportMmsHistory` |
| `MMSApi.MmsPricePost` | `MmsAPI.CalculateMmsPrice` |
| `MmsCampaignApi.MmsCampaignsSendPost` | `MmsCampaignsAPI.SendMmsCampaign` |
| `MmsCampaignApi.MmsCampaignsGet` | `MmsCampaignsAPI.ViewAllMmsCampaigns` |
| `MmsCampaignApi.MmsCampaignByMmsCampaignIdGet` | `MmsCampaignsAPI.ViewMmsCampaign` |
| `MmsCampaignApi.MmsCampaignsByMmsCampaignIdPut` | `MmsCampaignsAPI.UpdateMmsCampaign` |
| `MmsCampaignApi.MmsCampaignsCancelByMmsCampaignIdPut` | `MmsCampaignsAPI.CancelMmsCampaign` |
| `MmsCampaignApi.MmsCampaignsPricePost` | `MmsCampaignsAPI.CalculateMmsCampaignPrice` |
| `SmsCampaignApi.SmsCampaignsSendPost` | `SmsCampaignsAPI.SendSmsCampaign` |
| `SmsCampaignApi.SmsCampaignsGet` | `SmsCampaignsAPI.ViewSmsCampaigns` |
| `SmsCampaignApi.SmsCampaignBySmsCampaignIdGet` | `SmsCampaignsAPI.ViewSpecificSmsCampaign` |
| `SmsCampaignApi.SmsCampaignsBySmsCampaignIdPut` | `SmsCampaignsAPI.UpdateSmsCampaign` |
| `SmsCampaignApi.SmsCampaignsCancelBySmsCampaignIdPut` | `SmsCampaignsAPI.CancelSmsCampaign` |
| `SmsCampaignApi.SmsCampaignsPricePost` | `SmsCampaignsAPI.CalculateSmsCampaignPrice` |
| `VoiceApi.VoiceSendPost` | `VoiceMessagingAPI.SendVoiceMessage` ⚠️ [§12](#12-the-voice-naming-trap-read-this-before-touching-voice-code) |
| `VoiceApi.VoiceHistoryGet` | `VoiceMessagingAPI.GetVoiceHistory` |
| `VoiceApi.VoiceHistoryExportGet` | `VoiceMessagingAPI.ExportVoiceHistory` |
| `VoiceApi.VoicePricePost` | `VoiceMessagingAPI.CalculateVoicePrice` |
| `VoiceApi.VoiceLangGet` | `VoiceMessagingAPI.ViewVoiceLanguages` |
| `VoiceApi.VoiceCancelAllPut` | `VoiceMessagingAPI.CancelAllVoiceMessages` |
| `VoiceApi.VoiceCancelByMessageIdPut` | `VoiceMessagingAPI.CancelVoiceMessage` |
| `VoiceApi.VoiceReceiptsGet` | `VoiceMessagingAPI.ViewVoiceReceipts` |
| `VoiceDeliveryReceiptRulesApi.VoiceDeliveryReceiptAutomationsGet` | `VoiceAPI.ViewVoiceDeliveryReceiptRules` ⚠️ [§12](#12-the-voice-naming-trap-read-this-before-touching-voice-code) |
| `VoiceDeliveryReceiptRulesApi.VoiceDeliveryReceiptAutomationGet` | `VoiceAPI.ViewVoiceDeliveryReceiptRule` |
| `VoiceDeliveryReceiptRulesApi.VoiceDeliveryReceiptAutomationPost` | `VoiceAPI.CreateVoiceDeliveryReceiptRule` |
| `VoiceDeliveryReceiptRulesApi.VoiceDeliveryReceiptAutomationPut` | `VoiceAPI.UpdateVoiceDeliveryReceiptRule` |
| `VoiceDeliveryReceiptRulesApi.VoiceDeliveryReceiptAutomationDelete` | `VoiceAPI.DeleteVoiceDeliveryReceiptRule` |
| `StatisticsApi.StatisticsSmsGet` | `StatisticsAPI.ViewSmsStatistics` |
| `StatisticsApi.StatisticsVoiceGet` | `StatisticsAPI.ViewVoiceStatistics` |

### Email-to-SMS: `EmailToSmsApi` → `EmailToSmsAPI`

| Legacy | v2 |
|---|---|
| `SmsEmailSmsGet` | `ViewAllowedEmails` |
| `SmsEmailSmsPost` | `AddAllowedEmail` |
| `SmsEmailSmsStrippedStringPost` | `CreateStrippedStringRule` |
| `SmsEmailSmsStrippedStringGet` | `ViewStrippedStringRule` |
| `SmsEmailSmsStrippedStringsGet` | `ViewStrippedStringRules` |
| `SmsEmailSmsStrippedStringPut` | `UpdateStrippedStringRule` |
| `SmsEmailSmsStrippedStringDelete` | `DeleteStrippedStringRule` |

## 11. Side-by-side examples for common operations

### Send an SMS (the full calling-convention change, end to end)

```go
// Legacy
import (
    "context"
    "fmt"
    clicksend "github.com/ClickSend/clicksend-go"
)

cfg := clicksend.NewConfiguration()
client := clicksend.NewAPIClient(cfg)
auth := context.WithValue(context.Background(), clicksend.ContextBasicAuth, clicksend.BasicAuth{
    UserName: username, Password: apiKey,
})

collection := clicksend.SmsMessageCollection{
    Messages: []clicksend.SmsMessage{
        {From: "MyBusiness", To: "+61411111111", Body: "Hello from ClickSend!", Source: "go-sdk"},
    },
}

result, httpResp, err := client.SMSApi.SmsSendPost(auth, collection)
if err != nil {
    if apiErr, ok := err.(clicksend.GenericSwaggerError); ok {
        fmt.Println("raw body:", string(apiErr.Body()))
    }
    return err
}
var parsed map[string]interface{}
json.Unmarshal([]byte(result), &parsed)   // manual, untyped
fmt.Println(parsed)
```

```go
// v2
import (
    "context"
    "fmt"
    clicksend "github.com/ClickSend/clicksend-go-v2"
)

cfg := clicksend.NewConfiguration()
client := clicksend.NewAPIClient(cfg)
auth := context.WithValue(context.Background(), clicksend.ContextBasicAuth, clicksend.BasicAuth{
    UserName: username, Password: apiKey,
})

message := clicksend.NewSendSmsRequestMessagesInner("Hello from ClickSend!")
message.SetTo("+61411111111")
message.SetFrom("MyBusiness")
message.SetSource("go-sdk")

sendSmsRequest := clicksend.NewSendSmsRequest()
sendSmsRequest.SetMessages([]clicksend.SendSmsRequestMessagesInner{*message})

result, httpResp, err := client.SmsAPI.SendSms(auth).SendSmsRequest(*sendSmsRequest).Execute()
if err != nil {
    if apiErr, ok := err.(*clicksend.GenericOpenAPIError); ok {
        fmt.Println("raw body:", string(apiErr.Body()))
    }
    fmt.Println("status:", httpResp.StatusCode)
    return err
}
fmt.Println(result.Data.Messages[0].MessageId)   // typed field access
```

### View SMS history — query params via chained setters, not an `Opts` struct

```go
// Legacy
opts := &clicksend.SMSApiSmsHistoryGetOpts{
    Q:        optional.NewString(q),
    DateFrom: optional.NewInt32(dateFrom),
    DateTo:   optional.NewInt32(dateTo),
    Page:     optional.NewInt32(page),
    Limit:    optional.NewInt32(limit),
}
result, httpResp, err := client.SMSApi.SmsHistoryGet(auth, opts)

// v2 — same params, plus a new OrderBy setter
result, httpResp, err := client.SmsAPI.ViewSmsHistory(auth).
    Q(q).
    DateFrom(dateFrom).
    DateTo(dateTo).
    Page(page).
    Limit(limit).
    OrderBy("date:desc").
    Execute()
```

### Send an MMS / Email / Voice message

Same pattern on every channel — build the message model(s), wrap them in the operation's `*Request` model, call `Send<Channel>(ctx).<Channel>Request(...).Execute()`:

| Channel | Legacy call | v2 call |
|---|---|---|
| MMS | `client.MMSApi.MmsSendPost(auth, mmsMessageCollection)` | `client.MmsAPI.SendMms(auth).SendMmsRequest(sendMmsRequest).Execute()` |
| Email | `client.TransactionalEmailApi.EmailSendPost(auth, email)` | `client.EmailAPI.SendEmail(auth).SendEmailRequest(sendEmailRequest).Execute()` |
| Voice | `client.VoiceApi.VoiceSendPost(auth, voiceMessageCollection)` (legacy `VoiceApi`) | `client.VoiceMessagingAPI.SendVoiceMessage(auth).SendVoiceMessageRequest(req).Execute()` (⚠️ new `VoiceMessagingAPI`, see [§12](#12-the-voice-naming-trap-read-this-before-touching-voice-code)) |

> **Fax, Letters, and Postcards are not part of the v2 SDK** — there is no `FaxAPI`/`LettersAPI`/`PostcardsAPI` service or `SendFax`/equivalent method. See [§13](#13-endpointsmethods-removed-in-v2).

### Create a contact in a list — argument type changed, payload moved to the builder

```go
// Legacy — Contact struct first, int32 listId second
client.ContactApi.ListsContactsByListIdPost(auth, contact, listId)

// v2 — listId is a STRING, passed to the top-level method; payload goes through the builder
client.ListsAPI.CreateNewContact(auth, strconv.Itoa(listId)).
    CreateNewContactRequest(createNewContactRequest).
    Execute()
```

### List contacts / lists — pagination parameters were dropped, not just renamed

```go
// Legacy — Page/Limit were real Opts fields
client.ContactApi.ListsContactsByListIdGet(auth, listId, &clicksend.ContactApiListsContactsByListIdGetOpts{
    Page: optional.NewInt32(page), Limit: optional.NewInt32(limit),
})
client.ContactListApi.ListsGet(auth, &clicksend.ContactListApiListsGetOpts{
    Page: optional.NewInt32(page), Limit: optional.NewInt32(limit),
})
client.SubaccountApi.SubaccountsGet(auth, &clicksend.SubaccountApiSubaccountsGetOpts{
    Page: optional.NewInt32(page), Limit: optional.NewInt32(limit),
})

// v2 — no Page/Limit setters exist on these request builders at all
client.ListsAPI.ViewListContacts(auth, listId).Execute()
client.ListsAPI.ViewLists(auth).Execute()
client.SubaccountsAPI.ViewSubaccounts(auth).Execute()
```

**This is a real behavior change, confirmed by reading the generated request-builder structs directly** — `ApiViewListContactsRequest`, `ApiViewListsRequest`, and `ApiViewSubaccountsRequest` in the v2 source have no `Page`/`Limit` fields or setter methods at all. Verify against the current API reference how pagination is handled for any workflow that relied on them before you ship.

### Upload a media file — typed struct → generic map body

```go
// Legacy
uploadFile := clicksend.UploadFile{Content: base64EncodedContent}
result, httpResp, err := client.UploadApi.UploadsPost(auth, uploadFile, "true")

// v2 — generic map body through the same builder pattern as every other call;
// check docs/UploadsAPI.md for the exact field names expected, and note this
// endpoint returns no typed result — only (*http.Response, error)
httpResp, err := client.UploadsAPI.UploadAMediaFile(auth).
    Body(map[string]interface{}{"file": base64EncodedContent, "convert": "true"}).
    Execute()
```

### Create a subaccount

```go
// Legacy
client.SubaccountApi.SubaccountsPost(auth, subaccount)

// v2
client.SubaccountsAPI.CreateSubaccount(auth).CreateSubaccountRequest(createSubaccountRequest).Execute()
```

## 12. The Voice naming trap (read this before touching voice code)

This is the single most confusing rename in the whole migration, and it's identical in shape to the same trap in every other ClickSend SDK — a naive search-and-replace of `VoiceApi` will silently point your code at the wrong service:

- Legacy **`VoiceApi`** (send a voice message, view/export history, calculate price, list voice languages, cancel, view receipts — 10 methods on `VoiceApiService`) → renamed to new **`VoiceMessagingAPI`** (`VoiceMessagingAPIService`, 8 methods; 2 dropped, see [§13](#13-endpointsmethods-removed-in-v2)).
- Legacy **`VoiceDeliveryReceiptRulesApi`** (create/update/delete/view delivery-receipt rules — 5 methods on `VoiceDeliveryReceiptRulesApiService`) → renamed to new **`VoiceAPI`** (`VoiceAPIService`, the same 5 methods, confirmed by direct listing of `api_voice.go`).

The new `VoiceAPI` has **nothing to do with sending voice calls** — it is purely the old delivery-receipt-rules service under a new, and very similarly spelled, name. To migrate voice-*sending* code, use `client.VoiceMessagingAPI`, not `client.VoiceAPI`:

```go
// Wrong — this compiles, but VoiceAPIService in v2 only has delivery-receipt-rule methods
client.VoiceAPI.SendVoiceMessage(auth)   // compile error: no method SendVoiceMessage on *VoiceAPIService

// Correct
message := clicksend.NewSendVoiceMessageRequestMessagesInner("Hello from ClickSend!")
message.SetTo("+61411111111")

sendVoiceMessageRequest := clicksend.NewSendVoiceMessageRequest()
sendVoiceMessageRequest.SetMessages([]clicksend.SendVoiceMessageRequestMessagesInner{*message})

result, httpResp, err := client.VoiceMessagingAPI.SendVoiceMessage(auth).
    SendVoiceMessageRequest(*sendVoiceMessageRequest).
    Execute()
```

Unlike the equivalent dynamically-typed-language trap, Go's compiler *will* catch a call to a method that doesn't exist on `VoiceAPIService` — but it will not catch you constructing the wrong service reference and simply never noticing the returned pointer is `nil`-shaped for what you wanted, or copy-pasting a `VoiceDeliveryReceiptRule`-shaped snippet under the assumption that `VoiceAPI` means "the voice API." Read the field name, not just the fact that it compiles.

## 13. Endpoints/methods removed in v2

### Entire products dropped

The **Fax**, **Letters**, and **Postcards** products have **no presence at all** in the v2 SDK — no service, no models, confirmed by the absence of any matching `api_*.go` or `model_*.go` file in `output/go`. If your integration sends faxes, letters, or postcards, there is currently no v2 SDK path for it; call the REST API directly or keep the legacy SDK installed for just that functionality.

| Legacy service(s) | Covered (legacy) | v2 |
|---|---|---|
| `FAXApi`, `FAXDeliveryReceiptRulesApi`, `InboundFAXRulesApi` | send fax, fax history/export, fax price, fax receipts, fax delivery-receipt rules, inbound fax rules | _none_ |
| `PostLetterApi` | send letter, letter history/export, letter price | _none_ |
| `PostPostcardApi` | send postcard, postcard history/export, postcard price | _none_ |
| `DetectAddressApi` | address detection/parsing (`DetectAddressPost`) | _none_ |

### Individual methods dropped (service otherwise survived)

The following legacy operations have **no equivalent anywhere in the v2 SDK**, confirmed by grepping every v2 `api_*.go` for a matching operation. If your integration depends on any of these, check the current ClickSend API reference before upgrading — the underlying endpoint may have been retired, moved, or simply not covered by the new spec at build time:

- `AccountApi.AccountPost` — update account details
- `AccountApi.AccountVerifySendPut` — send account verification email
- `AccountApi.AccountVerifyVerifyByActivationTokenPut` — verify account by activation token
- `AccountApi.ForgotPasswordVerifyPut` — verify a forgotten-password token
- `MMSApi.MmsReceiptsGet` — view MMS delivery receipts
- `MMSApi.MmsReceiptsReadPut` — mark MMS receipts as read
- `VoiceApi.VoiceReceiptsPost` (legacy service) — create a test voice receipt
- `VoiceApi.VoiceReceiptsReadPut` (legacy service) — mark voice receipts as read

Additionally, **pagination parameters (`Page`, `Limit`, and any `updated_after`-equivalent) were dropped** from several request builders even where the service survived — notably `ListsAPI.ViewLists`, `ListsAPI.ViewListContacts`, and `SubaccountsAPI.ViewSubaccounts` (see [§11](#11-side-by-side-examples-for-common-operations)).

## 14. Brand-new resources and methods in v2

No legacy counterpart at all — nothing to migrate, but worth knowing they exist:

- **`AlphaTagsAPI`** — `ListAlphaTags`, `GetAlphaTag`, `RequestAlphaTag`, `DeleteAlphaTag` (the last returns `(*http.Response, error)`, no body)
- **`DefaultSendersAPI`** — `GetDefaultSendersList`, `GetDefaultSenderDetails`, `CreateDefaultSender`, `UpdateDefaultSender`, `DeleteDefaultSender` (no body), `ListCompliantSenderTypes`
- **`OwnNumbersAPI`** (Bring Your Own Number) — `ListOwnNumbers`, `GetOwnNumberDetail`, `UpdateOwnNumber`, `DeleteOwnNumber`, `RequestOwnNumberVerificationOtp`, `VerifyOwnNumberOtp`
- **`UrlShorteningAPI`** — `ShortUrlGetStatistics`, `ShortUrlGetTracking`
- **`NumbersAPI.RegisterNumbers`** — number registration (alongside the renamed `NumberApi` methods)
- **`SmsAPI.ViewASpecificInboundSmsMessage`** and **`SmsAPI.ViewASpecificSmsTemplate`** — fetch a single inbound message / template by ID (legacy only exposed the list endpoints)

## 15. Step-by-step migration checklist

1. **Swap the import path**: `github.com/ClickSend/clicksend-go` → `github.com/ClickSend/clicksend-go-v2`, and switch your install mechanism from however you currently vendor/`replace` the legacy source (it has no `go.mod`) to a normal `go get` ([§2](#2-installation--imports)). Both packages import as `clicksend`, so the import line alone won't flag anything — every call site has to be checked.
2. **Rename every service field on `client`**: `client.SMSApi` → `client.SmsAPI`, `client.MMSApi` → `client.MmsAPI`, etc., using the [§10](#10-service-by-service-mapping-all-37-legacy-services) tables. **Pay special attention to `VoiceApi` → `VoiceMessagingAPI`** and `VoiceDeliveryReceiptRulesApi` → `VoiceAPI` ([§12](#12-the-voice-naming-trap-read-this-before-touching-voice-code)).
3. **Convert every call site from positional arguments to the fluent builder pattern**, ending each chain in `.Execute()` ([§5](#5-calling-an-endpoint-positional-args--fluent-builder)). The compiler will flag a missing `.Execute()` and a nonexistent method, but not a builder call made on the wrong service field.
4. **Rebuild every request payload** using the matching `New*Request()` constructor and `Set*()` methods (or a struct literal wrapped in `Ptr*` helpers) instead of the old domain-model struct literal ([§6](#6-request-payloads-builder--request-models-replace-struct-literals)).
5. **Update response handling** — delete any `json.Unmarshal([]byte(result), ...)` calls and replace them with direct field access on the typed struct pointer v2 now returns. Check each endpoint's actual signature (some return `(*http.Response, error)` with no body) rather than assuming ([§7](#7-response-payloads-typed-structs-instead-of-raw-strings)).
6. **Fix every error type assertion**: `err.(clicksend.GenericSwaggerError)` → `err.(*clicksend.GenericOpenAPIError)` — note the added pointer, not just the renamed type ([§8](#8-error-handling-same-shape-no-exceptions-but-the-type-changed-from-a-value-to-a-pointer)).
7. **Replace every `*ApiXxxOpts` + `antihax/optional` construction** with chained setter calls on the request builder, and remove the `github.com/antihax/optional` import once nothing references it ([§9](#9-removed-apixxxopts--antihaxoptional--replaced-by-chained-setters)).
8. **Re-check parameters for every call** — several methods reordered arguments, changed types (`listId`/`contactId` `int32` → `string`), added params (`OrderBy`), or dropped pagination parameters entirely ([§11](#11-side-by-side-examples-for-common-operations), [§13](#13-endpointsmethods-removed-in-v2)).
9. **If you set `cfg.BasePath`**, switch to `cfg.Servers[0].URL` and drop the `/v3` suffix ([§4](#4-base-path--url-changes)).
10. **Confirm you don't depend on Fax, Letters, Postcards, or address detection** — none of these are available in v2 ([§13](#13-endpointsmethods-removed-in-v2)).
11. **Run `go build`** — it will catch every renamed/removed method and type immediately, since Go is statically compiled; treat every resulting compile error as a checklist item, then run your test suite against ClickSend's sandbox/test credentials before deploying to confirm behavior (not just compilation) matches.

## Things this guide could not verify with full certainty

- **Exact wording/edge cases of the pagination drop.** The absence of `Page`/`Limit` setters was confirmed directly on `ApiViewListsRequest`, `ApiViewListContactsRequest`, and `ApiViewSubaccountsRequest`, but whether the underlying REST endpoints still accept these as raw query parameters outside the SDK (i.e. whether this is an SDK-generation gap vs. an intentional API change) was not independently verified against the live API.
- **The real-world install mechanism legacy users actually use.** The legacy SDK ships no `go.mod`, and its own README documents copying the source in; this guide describes the most common alternatives (vendoring, a `replace` directive at a commit SHA) as the likely real pattern, but could not confirm which one any specific consumer's `go.mod` currently uses.
- **Whether every v2 "no body" endpoint listed in §7 is a permanent design choice or an artifact of the current OpenAPI spec/generator run** — confirmed accurate as of this generation, but could change on a future spec regeneration.
