# \VoiceMessagingAPI

All URIs are relative to *https://rest.clicksend.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**CalculateVoicePrice**](VoiceMessagingAPI.md#CalculateVoicePrice) | **Post** /v3/voice/price | Calculate Voice Price
[**CancelAllVoiceMessages**](VoiceMessagingAPI.md#CancelAllVoiceMessages) | **Put** /v3/voice/cancel-all | Cancel All Voice Messages
[**CancelVoiceMessage**](VoiceMessagingAPI.md#CancelVoiceMessage) | **Put** /v3/voice/{message_id}/cancel | Cancel Voice Message
[**ExportVoiceHistory**](VoiceMessagingAPI.md#ExportVoiceHistory) | **Get** /v3/voice/history/export | Export Voice History
[**GetVoiceHistory**](VoiceMessagingAPI.md#GetVoiceHistory) | **Get** /v3/voice/history | Get Voice History
[**SendVoiceMessage**](VoiceMessagingAPI.md#SendVoiceMessage) | **Post** /v3/voice/send | Send Voice Message
[**ViewVoiceLanguages**](VoiceMessagingAPI.md#ViewVoiceLanguages) | **Get** /v3/voice/lang | View Voice Languages
[**ViewVoiceReceipts**](VoiceMessagingAPI.md#ViewVoiceReceipts) | **Get** /v3/voice/receipts | View Voice Receipts



## CalculateVoicePrice

> CalculateVoicePrice CalculateVoicePrice(ctx).ContentType(contentType).CalculateVoicePriceRequest(calculateVoicePriceRequest).Execute()

Calculate Voice Price



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
	calculateVoicePriceRequest := *openapiclient.NewCalculateVoicePriceRequest() // CalculateVoicePriceRequest |  (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.VoiceMessagingAPI.CalculateVoicePrice(context.Background()).ContentType(contentType).CalculateVoicePriceRequest(calculateVoicePriceRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `VoiceMessagingAPI.CalculateVoicePrice``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `CalculateVoicePrice`: CalculateVoicePrice
	fmt.Fprintf(os.Stdout, "Response from `VoiceMessagingAPI.CalculateVoicePrice`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiCalculateVoicePriceRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **contentType** | **string** |  | 
 **calculateVoicePriceRequest** | [**CalculateVoicePriceRequest**](CalculateVoicePriceRequest.md) |  | 

### Return type

[**CalculateVoicePrice**](CalculateVoicePrice.md)

### Authorization

[basicAuth](../README.md#basicAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## CancelAllVoiceMessages

> CancelAllVoiceMessages CancelAllVoiceMessages(ctx).ContentType(contentType).Body(body).Execute()

Cancel All Voice Messages



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
	contentType := "application/x-www-form-urlencoded" // string |  (optional)
	body := map[string]interface{}{ ... } // map[string]interface{} |  (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.VoiceMessagingAPI.CancelAllVoiceMessages(context.Background()).ContentType(contentType).Body(body).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `VoiceMessagingAPI.CancelAllVoiceMessages``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `CancelAllVoiceMessages`: CancelAllVoiceMessages
	fmt.Fprintf(os.Stdout, "Response from `VoiceMessagingAPI.CancelAllVoiceMessages`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiCancelAllVoiceMessagesRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **contentType** | **string** |  | 
 **body** | **map[string]interface{}** |  | 

### Return type

[**CancelAllVoiceMessages**](CancelAllVoiceMessages.md)

### Authorization

[basicAuth](../README.md#basicAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## CancelVoiceMessage

> CancelVoiceMessage CancelVoiceMessage(ctx, messageId).ContentType(contentType).Body(body).Execute()

Cancel Voice Message



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
	messageId := "messageId_example" // string | 
	contentType := "application/x-www-form-urlencoded" // string |  (optional)
	body := map[string]interface{}{ ... } // map[string]interface{} |  (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.VoiceMessagingAPI.CancelVoiceMessage(context.Background(), messageId).ContentType(contentType).Body(body).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `VoiceMessagingAPI.CancelVoiceMessage``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `CancelVoiceMessage`: CancelVoiceMessage
	fmt.Fprintf(os.Stdout, "Response from `VoiceMessagingAPI.CancelVoiceMessage`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**messageId** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiCancelVoiceMessageRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **contentType** | **string** |  | 
 **body** | **map[string]interface{}** |  | 

### Return type

[**CancelVoiceMessage**](CancelVoiceMessage.md)

### Authorization

[basicAuth](../README.md#basicAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## ExportVoiceHistory

> ExportVoiceHistory ExportVoiceHistory(ctx).ContentType(contentType).Filename(filename).Q(q).OrderBy(orderBy).DateFrom(dateFrom).DateTo(dateTo).Limit(limit).Execute()

Export Voice History



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
	filename := "Voice_history.csv" // string |  (optional)
	q := "q_example" // string |  (optional)
	orderBy := "date_added:desc" // string |  (optional)
	dateFrom := "dateFrom_example" // string |  (optional)
	dateTo := "dateTo_example" // string |  (optional)
	limit := int32(50000) // int32 |  (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.VoiceMessagingAPI.ExportVoiceHistory(context.Background()).ContentType(contentType).Filename(filename).Q(q).OrderBy(orderBy).DateFrom(dateFrom).DateTo(dateTo).Limit(limit).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `VoiceMessagingAPI.ExportVoiceHistory``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ExportVoiceHistory`: ExportVoiceHistory
	fmt.Fprintf(os.Stdout, "Response from `VoiceMessagingAPI.ExportVoiceHistory`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiExportVoiceHistoryRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **contentType** | **string** |  | 
 **filename** | **string** |  | 
 **q** | **string** |  | 
 **orderBy** | **string** |  | 
 **dateFrom** | **string** |  | 
 **dateTo** | **string** |  | 
 **limit** | **int32** |  | 

### Return type

[**ExportVoiceHistory**](ExportVoiceHistory.md)

### Authorization

[basicAuth](../README.md#basicAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## GetVoiceHistory

> GetVoiceHistory GetVoiceHistory(ctx).ContentType(contentType).DateTo(dateTo).Limit(limit).Operator(operator).OrderBy(orderBy).Page(page).Execute()

Get Voice History



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
	dateTo := "dateTo_example" // string |  (optional)
	limit := int32(20) // int32 |  (optional)
	operator := "AND" // string |  (optional)
	orderBy := "date_added:desc" // string |  (optional)
	page := int32(1) // int32 |  (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.VoiceMessagingAPI.GetVoiceHistory(context.Background()).ContentType(contentType).DateTo(dateTo).Limit(limit).Operator(operator).OrderBy(orderBy).Page(page).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `VoiceMessagingAPI.GetVoiceHistory``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `GetVoiceHistory`: GetVoiceHistory
	fmt.Fprintf(os.Stdout, "Response from `VoiceMessagingAPI.GetVoiceHistory`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiGetVoiceHistoryRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **contentType** | **string** |  | 
 **dateTo** | **string** |  | 
 **limit** | **int32** |  | 
 **operator** | **string** |  | 
 **orderBy** | **string** |  | 
 **page** | **int32** |  | 

### Return type

[**GetVoiceHistory**](GetVoiceHistory.md)

### Authorization

[basicAuth](../README.md#basicAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## SendVoiceMessage

> SendVoiceMessage SendVoiceMessage(ctx).ContentType(contentType).SendVoiceMessageRequest(sendVoiceMessageRequest).Execute()

Send Voice Message



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
	sendVoiceMessageRequest := *openapiclient.NewSendVoiceMessageRequest() // SendVoiceMessageRequest |  (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.VoiceMessagingAPI.SendVoiceMessage(context.Background()).ContentType(contentType).SendVoiceMessageRequest(sendVoiceMessageRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `VoiceMessagingAPI.SendVoiceMessage``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `SendVoiceMessage`: SendVoiceMessage
	fmt.Fprintf(os.Stdout, "Response from `VoiceMessagingAPI.SendVoiceMessage`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiSendVoiceMessageRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **contentType** | **string** |  | 
 **sendVoiceMessageRequest** | [**SendVoiceMessageRequest**](SendVoiceMessageRequest.md) |  | 

### Return type

[**SendVoiceMessage**](SendVoiceMessage.md)

### Authorization

[basicAuth](../README.md#basicAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## ViewVoiceLanguages

> ViewVoiceLanguages ViewVoiceLanguages(ctx).ContentType(contentType).Execute()

View Voice Languages



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
	resp, r, err := apiClient.VoiceMessagingAPI.ViewVoiceLanguages(context.Background()).ContentType(contentType).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `VoiceMessagingAPI.ViewVoiceLanguages``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ViewVoiceLanguages`: ViewVoiceLanguages
	fmt.Fprintf(os.Stdout, "Response from `VoiceMessagingAPI.ViewVoiceLanguages`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiViewVoiceLanguagesRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **contentType** | **string** |  | 

### Return type

[**ViewVoiceLanguages**](ViewVoiceLanguages.md)

### Authorization

[basicAuth](../README.md#basicAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## ViewVoiceReceipts

> ViewVoiceReceipts ViewVoiceReceipts(ctx).ContentType(contentType).Execute()

View Voice Receipts



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
	resp, r, err := apiClient.VoiceMessagingAPI.ViewVoiceReceipts(context.Background()).ContentType(contentType).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `VoiceMessagingAPI.ViewVoiceReceipts``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ViewVoiceReceipts`: ViewVoiceReceipts
	fmt.Fprintf(os.Stdout, "Response from `VoiceMessagingAPI.ViewVoiceReceipts`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiViewVoiceReceiptsRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **contentType** | **string** |  | 

### Return type

[**ViewVoiceReceipts**](ViewVoiceReceipts.md)

### Authorization

[basicAuth](../README.md#basicAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)

