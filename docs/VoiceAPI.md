# \VoiceAPI

All URIs are relative to *https://rest.clicksend.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**CreateVoiceDeliveryReceiptRule**](VoiceAPI.md#CreateVoiceDeliveryReceiptRule) | **Post** /v3/automations/voice/receipts | Create Voice Delivery Receipt Rule
[**DeleteVoiceDeliveryReceiptRule**](VoiceAPI.md#DeleteVoiceDeliveryReceiptRule) | **Delete** /v3/automations/voice/receipts/{receipt_rule_id} | Delete Voice Delivery Receipt Rule
[**UpdateVoiceDeliveryReceiptRule**](VoiceAPI.md#UpdateVoiceDeliveryReceiptRule) | **Put** /v3/automations/voice/receipts/{receipt_rule_id} | Update Voice Delivery Receipt Rule
[**ViewVoiceDeliveryReceiptRule**](VoiceAPI.md#ViewVoiceDeliveryReceiptRule) | **Get** /v3/automations/voice/receipts/{receipt_rule_id} | View Voice Delivery Receipt Rule
[**ViewVoiceDeliveryReceiptRules**](VoiceAPI.md#ViewVoiceDeliveryReceiptRules) | **Get** /v3/automations/voice/receipts | View Voice Delivery Receipt Rules



## CreateVoiceDeliveryReceiptRule

> CreateVoiceDeliveryReceiptRule CreateVoiceDeliveryReceiptRule(ctx).ContentType(contentType).CreateSmsDeliveryReceiptRuleRequest(createSmsDeliveryReceiptRuleRequest).Execute()

Create Voice Delivery Receipt Rule



### Example

```go
package main

import (
	"context"
	"fmt"
	"os"
	openapiclient "github.com/GIT_USER_ID/GIT_REPO_ID"
)

func main() {
	contentType := "application/json" // string |  (optional)
	createSmsDeliveryReceiptRuleRequest := *openapiclient.NewCreateSmsDeliveryReceiptRuleRequest() // CreateSmsDeliveryReceiptRuleRequest |  (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.VoiceAPI.CreateVoiceDeliveryReceiptRule(context.Background()).ContentType(contentType).CreateSmsDeliveryReceiptRuleRequest(createSmsDeliveryReceiptRuleRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `VoiceAPI.CreateVoiceDeliveryReceiptRule``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `CreateVoiceDeliveryReceiptRule`: CreateVoiceDeliveryReceiptRule
	fmt.Fprintf(os.Stdout, "Response from `VoiceAPI.CreateVoiceDeliveryReceiptRule`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiCreateVoiceDeliveryReceiptRuleRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **contentType** | **string** |  | 
 **createSmsDeliveryReceiptRuleRequest** | [**CreateSmsDeliveryReceiptRuleRequest**](CreateSmsDeliveryReceiptRuleRequest.md) |  | 

### Return type

[**CreateVoiceDeliveryReceiptRule**](CreateVoiceDeliveryReceiptRule.md)

### Authorization

[basicAuth](../README.md#basicAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## DeleteVoiceDeliveryReceiptRule

> DeleteVoiceDeliveryReceiptRule DeleteVoiceDeliveryReceiptRule(ctx, receiptRuleId).ContentType(contentType).Execute()

Delete Voice Delivery Receipt Rule



### Example

```go
package main

import (
	"context"
	"fmt"
	"os"
	openapiclient "github.com/GIT_USER_ID/GIT_REPO_ID"
)

func main() {
	receiptRuleId := "receiptRuleId_example" // string | 
	contentType := "application/json" // string |  (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.VoiceAPI.DeleteVoiceDeliveryReceiptRule(context.Background(), receiptRuleId).ContentType(contentType).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `VoiceAPI.DeleteVoiceDeliveryReceiptRule``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `DeleteVoiceDeliveryReceiptRule`: DeleteVoiceDeliveryReceiptRule
	fmt.Fprintf(os.Stdout, "Response from `VoiceAPI.DeleteVoiceDeliveryReceiptRule`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**receiptRuleId** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiDeleteVoiceDeliveryReceiptRuleRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **contentType** | **string** |  | 

### Return type

[**DeleteVoiceDeliveryReceiptRule**](DeleteVoiceDeliveryReceiptRule.md)

### Authorization

[basicAuth](../README.md#basicAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## UpdateVoiceDeliveryReceiptRule

> UpdateVoiceDeliveryReceiptRule UpdateVoiceDeliveryReceiptRule(ctx, receiptRuleId).ContentType(contentType).CreateSmsDeliveryReceiptRuleRequest(createSmsDeliveryReceiptRuleRequest).Execute()

Update Voice Delivery Receipt Rule



### Example

```go
package main

import (
	"context"
	"fmt"
	"os"
	openapiclient "github.com/GIT_USER_ID/GIT_REPO_ID"
)

func main() {
	receiptRuleId := "receiptRuleId_example" // string | 
	contentType := "application/json" // string |  (optional)
	createSmsDeliveryReceiptRuleRequest := *openapiclient.NewCreateSmsDeliveryReceiptRuleRequest() // CreateSmsDeliveryReceiptRuleRequest |  (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.VoiceAPI.UpdateVoiceDeliveryReceiptRule(context.Background(), receiptRuleId).ContentType(contentType).CreateSmsDeliveryReceiptRuleRequest(createSmsDeliveryReceiptRuleRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `VoiceAPI.UpdateVoiceDeliveryReceiptRule``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `UpdateVoiceDeliveryReceiptRule`: UpdateVoiceDeliveryReceiptRule
	fmt.Fprintf(os.Stdout, "Response from `VoiceAPI.UpdateVoiceDeliveryReceiptRule`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**receiptRuleId** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiUpdateVoiceDeliveryReceiptRuleRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **contentType** | **string** |  | 
 **createSmsDeliveryReceiptRuleRequest** | [**CreateSmsDeliveryReceiptRuleRequest**](CreateSmsDeliveryReceiptRuleRequest.md) |  | 

### Return type

[**UpdateVoiceDeliveryReceiptRule**](UpdateVoiceDeliveryReceiptRule.md)

### Authorization

[basicAuth](../README.md#basicAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## ViewVoiceDeliveryReceiptRule

> ViewVoiceDeliveryReceiptRule ViewVoiceDeliveryReceiptRule(ctx, receiptRuleId).ContentType(contentType).Execute()

View Voice Delivery Receipt Rule



### Example

```go
package main

import (
	"context"
	"fmt"
	"os"
	openapiclient "github.com/GIT_USER_ID/GIT_REPO_ID"
)

func main() {
	receiptRuleId := "receiptRuleId_example" // string | 
	contentType := "application/json" // string |  (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.VoiceAPI.ViewVoiceDeliveryReceiptRule(context.Background(), receiptRuleId).ContentType(contentType).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `VoiceAPI.ViewVoiceDeliveryReceiptRule``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ViewVoiceDeliveryReceiptRule`: ViewVoiceDeliveryReceiptRule
	fmt.Fprintf(os.Stdout, "Response from `VoiceAPI.ViewVoiceDeliveryReceiptRule`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**receiptRuleId** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiViewVoiceDeliveryReceiptRuleRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **contentType** | **string** |  | 

### Return type

[**ViewVoiceDeliveryReceiptRule**](ViewVoiceDeliveryReceiptRule.md)

### Authorization

[basicAuth](../README.md#basicAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## ViewVoiceDeliveryReceiptRules

> ViewVoiceDeliveryReceiptRules ViewVoiceDeliveryReceiptRules(ctx).ContentType(contentType).Execute()

View Voice Delivery Receipt Rules



### Example

```go
package main

import (
	"context"
	"fmt"
	"os"
	openapiclient "github.com/GIT_USER_ID/GIT_REPO_ID"
)

func main() {
	contentType := "application/json" // string |  (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.VoiceAPI.ViewVoiceDeliveryReceiptRules(context.Background()).ContentType(contentType).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `VoiceAPI.ViewVoiceDeliveryReceiptRules``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ViewVoiceDeliveryReceiptRules`: ViewVoiceDeliveryReceiptRules
	fmt.Fprintf(os.Stdout, "Response from `VoiceAPI.ViewVoiceDeliveryReceiptRules`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiViewVoiceDeliveryReceiptRulesRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **contentType** | **string** |  | 

### Return type

[**ViewVoiceDeliveryReceiptRules**](ViewVoiceDeliveryReceiptRules.md)

### Authorization

[basicAuth](../README.md#basicAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)

