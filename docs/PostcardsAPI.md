# \PostcardsAPI

All URIs are relative to *https://rest.clicksend.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**CalculatePostcardPrice**](PostcardsAPI.md#CalculatePostcardPrice) | **Post** /v3/post/postcards/price | Calculate Postcard Price
[**CancelScheduledPostcard**](PostcardsAPI.md#CancelScheduledPostcard) | **Put** /v3/post/postcards/{message_id}/cancel | Cancel Scheduled Postcard
[**ExportPostcardHistory**](PostcardsAPI.md#ExportPostcardHistory) | **Get** /v3/post/postcards/history/export | Export Postcard History
[**SendPostcard**](PostcardsAPI.md#SendPostcard) | **Post** /v3/post/postcards/send | Send Postcard
[**ViewPostcardHistory**](PostcardsAPI.md#ViewPostcardHistory) | **Get** /v3/post/postcards/history | View Postcard History



## CalculatePostcardPrice

> CalculatePostcardPrice CalculatePostcardPrice(ctx).ContentType(contentType).SendPostcardRequest(sendPostcardRequest).Execute()

Calculate Postcard Price



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
	sendPostcardRequest := *openapiclient.NewSendPostcardRequest() // SendPostcardRequest |  (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.PostcardsAPI.CalculatePostcardPrice(context.Background()).ContentType(contentType).SendPostcardRequest(sendPostcardRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `PostcardsAPI.CalculatePostcardPrice``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `CalculatePostcardPrice`: CalculatePostcardPrice
	fmt.Fprintf(os.Stdout, "Response from `PostcardsAPI.CalculatePostcardPrice`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiCalculatePostcardPriceRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **contentType** | **string** |  | 
 **sendPostcardRequest** | [**SendPostcardRequest**](SendPostcardRequest.md) |  | 

### Return type

[**CalculatePostcardPrice**](CalculatePostcardPrice.md)

### Authorization

[basicAuth](../README.md#basicAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## CancelScheduledPostcard

> CancelScheduledPostcard CancelScheduledPostcard(ctx, messageId).Execute()

Cancel Scheduled Postcard



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

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.PostcardsAPI.CancelScheduledPostcard(context.Background(), messageId).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `PostcardsAPI.CancelScheduledPostcard``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `CancelScheduledPostcard`: CancelScheduledPostcard
	fmt.Fprintf(os.Stdout, "Response from `PostcardsAPI.CancelScheduledPostcard`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**messageId** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiCancelScheduledPostcardRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


### Return type

[**CancelScheduledPostcard**](CancelScheduledPostcard.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## ExportPostcardHistory

> ExportPostcardHistory ExportPostcardHistory(ctx).ContentType(contentType).Execute()

Export Postcard History



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
	resp, r, err := apiClient.PostcardsAPI.ExportPostcardHistory(context.Background()).ContentType(contentType).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `PostcardsAPI.ExportPostcardHistory``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ExportPostcardHistory`: ExportPostcardHistory
	fmt.Fprintf(os.Stdout, "Response from `PostcardsAPI.ExportPostcardHistory`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiExportPostcardHistoryRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **contentType** | **string** |  | 

### Return type

[**ExportPostcardHistory**](ExportPostcardHistory.md)

### Authorization

[basicAuth](../README.md#basicAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## SendPostcard

> SendPostcard SendPostcard(ctx).ContentType(contentType).SendPostcardRequest(sendPostcardRequest).Execute()

Send Postcard



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
	sendPostcardRequest := *openapiclient.NewSendPostcardRequest() // SendPostcardRequest |  (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.PostcardsAPI.SendPostcard(context.Background()).ContentType(contentType).SendPostcardRequest(sendPostcardRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `PostcardsAPI.SendPostcard``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `SendPostcard`: SendPostcard
	fmt.Fprintf(os.Stdout, "Response from `PostcardsAPI.SendPostcard`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiSendPostcardRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **contentType** | **string** |  | 
 **sendPostcardRequest** | [**SendPostcardRequest**](SendPostcardRequest.md) |  | 

### Return type

[**SendPostcard**](SendPostcard.md)

### Authorization

[basicAuth](../README.md#basicAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## ViewPostcardHistory

> ViewPostcardHistory ViewPostcardHistory(ctx).ContentType(contentType).Execute()

View Postcard History



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
	resp, r, err := apiClient.PostcardsAPI.ViewPostcardHistory(context.Background()).ContentType(contentType).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `PostcardsAPI.ViewPostcardHistory``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ViewPostcardHistory`: ViewPostcardHistory
	fmt.Fprintf(os.Stdout, "Response from `PostcardsAPI.ViewPostcardHistory`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiViewPostcardHistoryRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **contentType** | **string** |  | 

### Return type

[**ViewPostcardHistory**](ViewPostcardHistory.md)

### Authorization

[basicAuth](../README.md#basicAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)

