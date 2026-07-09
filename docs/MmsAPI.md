# \MmsAPI

All URIs are relative to *https://rest.clicksend.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**CalculateMmsPrice**](MmsAPI.md#CalculateMmsPrice) | **Post** /v3/mms/price | Calculate MMS Price
[**ExportMmsHistory**](MmsAPI.md#ExportMmsHistory) | **Get** /v3/mms/history/export | Export MMS History
[**SendMms**](MmsAPI.md#SendMms) | **Post** /v3/mms/send | Send MMS
[**ViewMmsHistory**](MmsAPI.md#ViewMmsHistory) | **Get** /v3/mms/history | View MMS History



## CalculateMmsPrice

> CalculateMmsPrice CalculateMmsPrice(ctx).ContentType(contentType).CalculateMmsPriceRequest(calculateMmsPriceRequest).Execute()

Calculate MMS Price



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
	calculateMmsPriceRequest := *openapiclient.NewCalculateMmsPriceRequest() // CalculateMmsPriceRequest |  (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.MmsAPI.CalculateMmsPrice(context.Background()).ContentType(contentType).CalculateMmsPriceRequest(calculateMmsPriceRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `MmsAPI.CalculateMmsPrice``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `CalculateMmsPrice`: CalculateMmsPrice
	fmt.Fprintf(os.Stdout, "Response from `MmsAPI.CalculateMmsPrice`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiCalculateMmsPriceRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **contentType** | **string** |  | 
 **calculateMmsPriceRequest** | [**CalculateMmsPriceRequest**](CalculateMmsPriceRequest.md) |  | 

### Return type

[**CalculateMmsPrice**](CalculateMmsPrice.md)

### Authorization

[basicAuth](../README.md#basicAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## ExportMmsHistory

> ExportMmsHistory ExportMmsHistory(ctx).ContentType(contentType).Filename(filename).Q(q).OrderBy(orderBy).DateFrom(dateFrom).DateTo(dateTo).Limit(limit).Execute()

Export MMS History



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
	filename := "MMS_history.csv" // string |  (optional)
	q := "q_example" // string |  (optional)
	orderBy := "date_added:desc" // string |  (optional)
	dateFrom := "dateFrom_example" // string |  (optional)
	dateTo := "dateTo_example" // string |  (optional)
	limit := int32(50000) // int32 |  (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.MmsAPI.ExportMmsHistory(context.Background()).ContentType(contentType).Filename(filename).Q(q).OrderBy(orderBy).DateFrom(dateFrom).DateTo(dateTo).Limit(limit).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `MmsAPI.ExportMmsHistory``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ExportMmsHistory`: ExportMmsHistory
	fmt.Fprintf(os.Stdout, "Response from `MmsAPI.ExportMmsHistory`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiExportMmsHistoryRequest struct via the builder pattern


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

[**ExportMmsHistory**](ExportMmsHistory.md)

### Authorization

[basicAuth](../README.md#basicAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## SendMms

> SendMms SendMms(ctx).ContentType(contentType).SendMmsRequest(sendMmsRequest).Execute()

Send MMS



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
	sendMmsRequest := *openapiclient.NewSendMmsRequest() // SendMmsRequest |  (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.MmsAPI.SendMms(context.Background()).ContentType(contentType).SendMmsRequest(sendMmsRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `MmsAPI.SendMms``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `SendMms`: SendMms
	fmt.Fprintf(os.Stdout, "Response from `MmsAPI.SendMms`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiSendMmsRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **contentType** | **string** |  | 
 **sendMmsRequest** | [**SendMmsRequest**](SendMmsRequest.md) |  | 

### Return type

[**SendMms**](SendMms.md)

### Authorization

[basicAuth](../README.md#basicAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## ViewMmsHistory

> ViewMmsHistory ViewMmsHistory(ctx).ContentType(contentType).Limit(limit).Execute()

View MMS History



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
	limit := int32(100) // int32 |  (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.MmsAPI.ViewMmsHistory(context.Background()).ContentType(contentType).Limit(limit).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `MmsAPI.ViewMmsHistory``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ViewMmsHistory`: ViewMmsHistory
	fmt.Fprintf(os.Stdout, "Response from `MmsAPI.ViewMmsHistory`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiViewMmsHistoryRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **contentType** | **string** |  | 
 **limit** | **int32** |  | 

### Return type

[**ViewMmsHistory**](ViewMmsHistory.md)

### Authorization

[basicAuth](../README.md#basicAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)

