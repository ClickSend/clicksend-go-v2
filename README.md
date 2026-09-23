# ClickSend Go SDK

[![Go Reference](https://pkg.go.dev/badge/github.com/ClickSend/clicksend-go-v2/v6.svg)](https://pkg.go.dev/github.com/ClickSend/clicksend-go-v2/v6)
[![License: MIT](https://img.shields.io/badge/license-MIT-blue.svg)](https://opensource.org/licenses/MIT)
[![API: v3](https://img.shields.io/badge/ClickSend%20API-v3-brightgreen.svg)](https://developers.clicksend.com/docs/rest/v3/)

Official Go client for the [ClickSend API](https://developers.clicksend.com/) — send SMS, MMS, voice and email messages, run SMS and MMS campaigns, manage numbers, contacts and subaccounts, and pull delivery receipts and reporting through a single authenticated HTTPS client.

This library is generated from ClickSend's official OpenAPI v3 specification and is maintained by ClickSend. It covers every endpoint of the [ClickSend REST API](https://developers.clicksend.com/docs/rest/v3/).

- 📚 **API reference:** https://developers.clicksend.com/docs/rest/v3/
- 🔑 **Dashboard & API credentials:** https://dashboard.clicksend.com
- 🗂 **Source & issues:** https://github.com/ClickSend/clicksend-go-v2
- 💬 **Support:** https://help.clicksend.com

## Features

- **Messaging** — SMS, MMS, voice / text-to-speech, transactional email, email-to-SMS
- **Campaigns** — SMS and MMS campaigns
- **Numbers & sender IDs** — dedicated numbers, own numbers, alpha tags, default senders
- **Contacts** — contact lists, contacts and the address book
- **Account & billing** — account details, transactions, subaccounts, referrals, reseller accounts
- **Delivery & reporting** — delivery receipts, inbound messages, statistics
- **Extras** — URL shortening, file uploads, number verification, international messaging
- **Typed models** for every request and response
- **HTTP Basic auth** with your ClickSend username and API key
- **Identifiable traffic** — requests are sent with a `ClickSend-SDK/<version>/go` `User-Agent` by default
- MIT licensed

## Requirements

- Go 1.23 or newer

## Installation

```sh
go get github.com/ClickSend/clicksend-go-v2/v6
```

## Authentication

Every API call authenticates with HTTP Basic auth using your ClickSend **username** and **API key**, both available from the [ClickSend Dashboard](https://dashboard.clicksend.com/#/account/subaccount). Supply them through environment variables rather than hard-coding them:

```sh
export CLICKSEND_USERNAME="your-username"
export CLICKSEND_API_KEY="your-api-key"
```

## Quickstart

```go
package main

import (
	"context"
	"fmt"
	"os"

	clicksend "github.com/ClickSend/clicksend-go-v2/v6"
)

func main() {
	cfg := clicksend.NewConfiguration()
	client := clicksend.NewAPIClient(cfg)

	auth := context.WithValue(context.Background(), clicksend.ContextBasicAuth, clicksend.BasicAuth{
		UserName: os.Getenv("CLICKSEND_USERNAME"),
		Password: os.Getenv("CLICKSEND_API_KEY"),
	})

	message := clicksend.NewSendSmsRequestMessagesInner("Hello from ClickSend!")
	message.SetTo("+61411111111")
	message.SetSource("sdk")

	sendSmsRequest := clicksend.NewSendSmsRequest()
	sendSmsRequest.SetMessages([]clicksend.SendSmsRequestMessagesInner{*message})

	result, _, err := client.SmsAPI.SendSms(auth).SendSmsRequest(*sendSmsRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error calling SendSms: %v\n", err)
		return
	}
	fmt.Println(result)
}
```

## More Examples

### View account details

```go
result, _, err := client.ManagementAPI.ViewAccountDetails(auth).Execute()
if err != nil {
	fmt.Fprintf(os.Stderr, "Error calling ViewAccountDetails: %v\n", err)
	return
}
fmt.Println(result)
```

### Send an MMS

```go
mmsMessage := clicksend.NewSendMmsRequestMessagesInner()
mmsMessage.SetTo("+61411111111")
mmsMessage.SetFrom("sdk")
mmsMessage.SetSubject("Hello")
mmsMessage.SetBody("Hello from ClickSend!")
mmsMessage.SetSource("sdk")

sendMmsRequest := clicksend.NewSendMmsRequest()
sendMmsRequest.SetMediaFile("https://clicksend.com/logo.png")
sendMmsRequest.SetMessages([]clicksend.SendMmsRequestMessagesInner{*mmsMessage})

result, _, err := client.MmsAPI.SendMms(auth).SendMmsRequest(*sendMmsRequest).Execute()
if err != nil {
	fmt.Fprintf(os.Stderr, "Error calling SendMms: %v\n", err)
	return
}
fmt.Println(result)
```

## Configuration

```go
cfg := clicksend.NewConfiguration()

// Override the API base URL (default: https://rest.clicksend.com).
cfg.Servers = clicksend.ServerConfigurations{
	{URL: "https://rest.clicksend.com"},
}

// Supply your own *http.Client for timeouts, proxies or retries.
cfg.HTTPClient = &http.Client{Timeout: 30 * time.Second}

client := clicksend.NewAPIClient(cfg)
```

## Error Handling

`Execute()` returns the parsed result, the raw `*http.Response`, and an `error`. On non-2xx responses
the error is a `*clicksend.GenericOpenAPIError`:

```go
result, httpRes, err := client.SmsAPI.SendSms(auth).SendSmsRequest(*sendSmsRequest).Execute()
if err != nil {
	if apiErr, ok := err.(*clicksend.GenericOpenAPIError); ok {
		fmt.Println(string(apiErr.Body())) // raw error payload from the API
	}
	fmt.Println(httpRes.StatusCode)         // HTTP status code
}
```

## Documentation

- Full REST API reference: https://developers.clicksend.com/docs/rest/v3/
- Package reference: https://pkg.go.dev/github.com/ClickSend/clicksend-go-v2/v6
- Per-endpoint SDK docs: the [`docs/`](docs) directory in this repository

## Versioning

This module follows [semantic versioning](https://semver.org/). Breaking changes are released as major versions.

## Support

- Help Centre: https://help.clicksend.com
- Contact support: https://clicksend.com/contact
- SDK bugs and feature requests: https://github.com/ClickSend/clicksend-go-v2/issues

## License

Released under the [MIT License](https://opensource.org/licenses/MIT).

---

**Keywords:** clicksend, sms, sms api, send sms, bulk sms, text message, texting, mms, mms api, voice, voice call, text to speech, tts, ivr, email to sms, sms campaign, mms campaign, url shortening, number verification, messaging, notifications, otp, 2fa, two factor authentication, transactional sms, marketing sms, appointment reminders, alerts, go, golang, rest api, clicksend sdk
