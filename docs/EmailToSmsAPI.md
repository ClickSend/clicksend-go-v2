# \EmailToSmsAPI

All URIs are relative to *https://rest.clicksend.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**AddAllowedEmail**](EmailToSmsAPI.md#AddAllowedEmail) | **Post** /v3/sms/email-sms | Add Allowed Email
[**CreateStrippedStringRule**](EmailToSmsAPI.md#CreateStrippedStringRule) | **Post** /v3/sms/email-sms-stripped-strings | Create Stripped String Rule
[**DeleteStrippedStringRule**](EmailToSmsAPI.md#DeleteStrippedStringRule) | **Delete** /v3/sms/email-sms-stripped-strings/{rule_id} | Delete Stripped String Rule
[**UpdateStrippedStringRule**](EmailToSmsAPI.md#UpdateStrippedStringRule) | **Put** /v3/sms/email-sms-stripped-strings/{rule_id} | Update Stripped String Rule
[**ViewAllowedEmails**](EmailToSmsAPI.md#ViewAllowedEmails) | **Get** /v3/sms/email-sms | View Allowed Emails
[**ViewStrippedStringRule**](EmailToSmsAPI.md#ViewStrippedStringRule) | **Get** /v3/sms/email-sms-stripped-strings/{rule_id} | View Stripped String Rule
[**ViewStrippedStringRules**](EmailToSmsAPI.md#ViewStrippedStringRules) | **Get** /v3/sms/email-sms-stripped-strings | View Stripped String Rules



## AddAllowedEmail

> AddAllowedEmail AddAllowedEmail(ctx).ContentType(contentType).AddAllowedEmailRequest(addAllowedEmailRequest).Execute()

Add Allowed Email



### Example

```go
package main

import (
	"context"
	"fmt"
	"os"
	openapiclient "github.com/ClickSend/clicksend-go-v2"
)

func main() {
	contentType := "application/json" // string |  (optional)
	addAllowedEmailRequest := *openapiclient.NewAddAllowedEmailRequest() // AddAllowedEmailRequest |  (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.EmailToSmsAPI.AddAllowedEmail(context.Background()).ContentType(contentType).AddAllowedEmailRequest(addAllowedEmailRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `EmailToSmsAPI.AddAllowedEmail``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `AddAllowedEmail`: AddAllowedEmail
	fmt.Fprintf(os.Stdout, "Response from `EmailToSmsAPI.AddAllowedEmail`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiAddAllowedEmailRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **contentType** | **string** |  | 
 **addAllowedEmailRequest** | [**AddAllowedEmailRequest**](AddAllowedEmailRequest.md) |  | 

### Return type

[**AddAllowedEmail**](AddAllowedEmail.md)

### Authorization

[basicAuth](../README.md#basicAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## CreateStrippedStringRule

> CreateStrippedStringRule CreateStrippedStringRule(ctx).ContentType(contentType).CreateStrippedStringRuleRequest(createStrippedStringRuleRequest).Execute()

Create Stripped String Rule



### Example

```go
package main

import (
	"context"
	"fmt"
	"os"
	openapiclient "github.com/ClickSend/clicksend-go-v2"
)

func main() {
	contentType := "application/json" // string |  (optional)
	createStrippedStringRuleRequest := *openapiclient.NewCreateStrippedStringRuleRequest() // CreateStrippedStringRuleRequest |  (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.EmailToSmsAPI.CreateStrippedStringRule(context.Background()).ContentType(contentType).CreateStrippedStringRuleRequest(createStrippedStringRuleRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `EmailToSmsAPI.CreateStrippedStringRule``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `CreateStrippedStringRule`: CreateStrippedStringRule
	fmt.Fprintf(os.Stdout, "Response from `EmailToSmsAPI.CreateStrippedStringRule`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiCreateStrippedStringRuleRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **contentType** | **string** |  | 
 **createStrippedStringRuleRequest** | [**CreateStrippedStringRuleRequest**](CreateStrippedStringRuleRequest.md) |  | 

### Return type

[**CreateStrippedStringRule**](CreateStrippedStringRule.md)

### Authorization

[basicAuth](../README.md#basicAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## DeleteStrippedStringRule

> DeleteStrippedStringRule DeleteStrippedStringRule(ctx, ruleId).ContentType(contentType).Execute()

Delete Stripped String Rule



### Example

```go
package main

import (
	"context"
	"fmt"
	"os"
	openapiclient "github.com/ClickSend/clicksend-go-v2"
)

func main() {
	ruleId := "ruleId_example" // string | 
	contentType := "application/json" // string |  (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.EmailToSmsAPI.DeleteStrippedStringRule(context.Background(), ruleId).ContentType(contentType).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `EmailToSmsAPI.DeleteStrippedStringRule``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `DeleteStrippedStringRule`: DeleteStrippedStringRule
	fmt.Fprintf(os.Stdout, "Response from `EmailToSmsAPI.DeleteStrippedStringRule`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**ruleId** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiDeleteStrippedStringRuleRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **contentType** | **string** |  | 

### Return type

[**DeleteStrippedStringRule**](DeleteStrippedStringRule.md)

### Authorization

[basicAuth](../README.md#basicAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## UpdateStrippedStringRule

> UpdateStrippedStringRule UpdateStrippedStringRule(ctx, ruleId).ContentType(contentType).CreateStrippedStringRuleRequest(createStrippedStringRuleRequest).Execute()

Update Stripped String Rule



### Example

```go
package main

import (
	"context"
	"fmt"
	"os"
	openapiclient "github.com/ClickSend/clicksend-go-v2"
)

func main() {
	ruleId := "ruleId_example" // string | 
	contentType := "application/json" // string |  (optional)
	createStrippedStringRuleRequest := *openapiclient.NewCreateStrippedStringRuleRequest() // CreateStrippedStringRuleRequest |  (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.EmailToSmsAPI.UpdateStrippedStringRule(context.Background(), ruleId).ContentType(contentType).CreateStrippedStringRuleRequest(createStrippedStringRuleRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `EmailToSmsAPI.UpdateStrippedStringRule``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `UpdateStrippedStringRule`: UpdateStrippedStringRule
	fmt.Fprintf(os.Stdout, "Response from `EmailToSmsAPI.UpdateStrippedStringRule`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**ruleId** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiUpdateStrippedStringRuleRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **contentType** | **string** |  | 
 **createStrippedStringRuleRequest** | [**CreateStrippedStringRuleRequest**](CreateStrippedStringRuleRequest.md) |  | 

### Return type

[**UpdateStrippedStringRule**](UpdateStrippedStringRule.md)

### Authorization

[basicAuth](../README.md#basicAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## ViewAllowedEmails

> ViewAllowedEmails ViewAllowedEmails(ctx).ContentType(contentType).Execute()

View Allowed Emails



### Example

```go
package main

import (
	"context"
	"fmt"
	"os"
	openapiclient "github.com/ClickSend/clicksend-go-v2"
)

func main() {
	contentType := "application/json" // string |  (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.EmailToSmsAPI.ViewAllowedEmails(context.Background()).ContentType(contentType).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `EmailToSmsAPI.ViewAllowedEmails``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ViewAllowedEmails`: ViewAllowedEmails
	fmt.Fprintf(os.Stdout, "Response from `EmailToSmsAPI.ViewAllowedEmails`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiViewAllowedEmailsRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **contentType** | **string** |  | 

### Return type

[**ViewAllowedEmails**](ViewAllowedEmails.md)

### Authorization

[basicAuth](../README.md#basicAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## ViewStrippedStringRule

> ViewStrippedStringRule ViewStrippedStringRule(ctx, ruleId).ContentType(contentType).Execute()

View Stripped String Rule



### Example

```go
package main

import (
	"context"
	"fmt"
	"os"
	openapiclient "github.com/ClickSend/clicksend-go-v2"
)

func main() {
	ruleId := "ruleId_example" // string | 
	contentType := "application/json" // string |  (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.EmailToSmsAPI.ViewStrippedStringRule(context.Background(), ruleId).ContentType(contentType).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `EmailToSmsAPI.ViewStrippedStringRule``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ViewStrippedStringRule`: ViewStrippedStringRule
	fmt.Fprintf(os.Stdout, "Response from `EmailToSmsAPI.ViewStrippedStringRule`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**ruleId** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiViewStrippedStringRuleRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **contentType** | **string** |  | 

### Return type

[**ViewStrippedStringRule**](ViewStrippedStringRule.md)

### Authorization

[basicAuth](../README.md#basicAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## ViewStrippedStringRules

> ViewStrippedStringRules ViewStrippedStringRules(ctx).ContentType(contentType).Execute()

View Stripped String Rules



### Example

```go
package main

import (
	"context"
	"fmt"
	"os"
	openapiclient "github.com/ClickSend/clicksend-go-v2"
)

func main() {
	contentType := "application/json" // string |  (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.EmailToSmsAPI.ViewStrippedStringRules(context.Background()).ContentType(contentType).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `EmailToSmsAPI.ViewStrippedStringRules``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ViewStrippedStringRules`: ViewStrippedStringRules
	fmt.Fprintf(os.Stdout, "Response from `EmailToSmsAPI.ViewStrippedStringRules`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiViewStrippedStringRulesRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **contentType** | **string** |  | 

### Return type

[**ViewStrippedStringRules**](ViewStrippedStringRules.md)

### Authorization

[basicAuth](../README.md#basicAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)

