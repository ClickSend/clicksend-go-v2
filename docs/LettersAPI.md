# \LettersAPI

All URIs are relative to *https://rest.clicksend.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**CalculateLetterPrice**](LettersAPI.md#CalculateLetterPrice) | **Post** /v3/post/letters/price | Calculate Letter Price
[**CancelScheduledLetter**](LettersAPI.md#CancelScheduledLetter) | **Put** /v3/post/letters/{message_id}/cancel | Cancel Scheduled Letter
[**DetectAddress**](LettersAPI.md#DetectAddress) | **Post** /v3/post/letters/detect-address | Detect Address
[**ExportLetterHistory**](LettersAPI.md#ExportLetterHistory) | **Get** /v3/post/letters/history/export | Export Letter History
[**SendLetter**](LettersAPI.md#SendLetter) | **Post** /v3/post/letters/send | Send Letter
[**ViewLetterHistory**](LettersAPI.md#ViewLetterHistory) | **Get** /v3/post/letters/history | View Letter History



## CalculateLetterPrice

> CalculateLetterPrice CalculateLetterPrice(ctx).ContentType(contentType).CalculateLetterPriceRequest(calculateLetterPriceRequest).Execute()

Calculate Letter Price



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
	calculateLetterPriceRequest := *openapiclient.NewCalculateLetterPriceRequest() // CalculateLetterPriceRequest |  (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.LettersAPI.CalculateLetterPrice(context.Background()).ContentType(contentType).CalculateLetterPriceRequest(calculateLetterPriceRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `LettersAPI.CalculateLetterPrice``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `CalculateLetterPrice`: CalculateLetterPrice
	fmt.Fprintf(os.Stdout, "Response from `LettersAPI.CalculateLetterPrice`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiCalculateLetterPriceRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **contentType** | **string** |  | 
 **calculateLetterPriceRequest** | [**CalculateLetterPriceRequest**](CalculateLetterPriceRequest.md) |  | 

### Return type

[**CalculateLetterPrice**](CalculateLetterPrice.md)

### Authorization

[basicAuth](../README.md#basicAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## CancelScheduledLetter

> CancelScheduledLetter CancelScheduledLetter(ctx, messageId).Execute()

Cancel Scheduled Letter



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
	messageId := "messageId_example" // string | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.LettersAPI.CancelScheduledLetter(context.Background(), messageId).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `LettersAPI.CancelScheduledLetter``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `CancelScheduledLetter`: CancelScheduledLetter
	fmt.Fprintf(os.Stdout, "Response from `LettersAPI.CancelScheduledLetter`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**messageId** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiCancelScheduledLetterRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


### Return type

[**CancelScheduledLetter**](CancelScheduledLetter.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## DetectAddress

> DetectAddress DetectAddress(ctx).ContentType(contentType).Body(body).Execute()

Detect Address



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
	body := map[string]interface{}{ ... } // map[string]interface{} |  (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.LettersAPI.DetectAddress(context.Background()).ContentType(contentType).Body(body).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `LettersAPI.DetectAddress``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `DetectAddress`: DetectAddress
	fmt.Fprintf(os.Stdout, "Response from `LettersAPI.DetectAddress`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiDetectAddressRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **contentType** | **string** |  | 
 **body** | **map[string]interface{}** |  | 

### Return type

[**DetectAddress**](DetectAddress.md)

### Authorization

[basicAuth](../README.md#basicAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## ExportLetterHistory

> ExportLetterHistory ExportLetterHistory(ctx).ContentType(contentType).Filename(filename).Q(q).OrderBy(orderBy).DateFrom(dateFrom).DateTo(dateTo).Limit(limit).Execute()

Export Letter History



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
	filename := "Post_history.csv" // string |  (optional)
	q := "q_example" // string |  (optional)
	orderBy := "date_added:desc" // string |  (optional)
	dateFrom := "dateFrom_example" // string |  (optional)
	dateTo := "dateTo_example" // string |  (optional)
	limit := int32(50000) // int32 |  (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.LettersAPI.ExportLetterHistory(context.Background()).ContentType(contentType).Filename(filename).Q(q).OrderBy(orderBy).DateFrom(dateFrom).DateTo(dateTo).Limit(limit).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `LettersAPI.ExportLetterHistory``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ExportLetterHistory`: ExportLetterHistory
	fmt.Fprintf(os.Stdout, "Response from `LettersAPI.ExportLetterHistory`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiExportLetterHistoryRequest struct via the builder pattern


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

[**ExportLetterHistory**](ExportLetterHistory.md)

### Authorization

[basicAuth](../README.md#basicAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## SendLetter

> SendLetter SendLetter(ctx).ContentType(contentType).SendLetterRequest(sendLetterRequest).Execute()

Send Letter



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
	sendLetterRequest := *openapiclient.NewSendLetterRequest() // SendLetterRequest |  (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.LettersAPI.SendLetter(context.Background()).ContentType(contentType).SendLetterRequest(sendLetterRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `LettersAPI.SendLetter``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `SendLetter`: SendLetter
	fmt.Fprintf(os.Stdout, "Response from `LettersAPI.SendLetter`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiSendLetterRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **contentType** | **string** |  | 
 **sendLetterRequest** | [**SendLetterRequest**](SendLetterRequest.md) |  | 

### Return type

[**SendLetter**](SendLetter.md)

### Authorization

[basicAuth](../README.md#basicAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## ViewLetterHistory

> ViewLetterHistory ViewLetterHistory(ctx).ContentType(contentType).Execute()

View Letter History



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
	resp, r, err := apiClient.LettersAPI.ViewLetterHistory(context.Background()).ContentType(contentType).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `LettersAPI.ViewLetterHistory``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ViewLetterHistory`: ViewLetterHistory
	fmt.Fprintf(os.Stdout, "Response from `LettersAPI.ViewLetterHistory`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiViewLetterHistoryRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **contentType** | **string** |  | 

### Return type

[**ViewLetterHistory**](ViewLetterHistory.md)

### Authorization

[basicAuth](../README.md#basicAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)

