# \UrlShorteningAPI

All URIs are relative to *https://rest.clicksend.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**ShortUrlGetStatistics**](UrlShorteningAPI.md#ShortUrlGetStatistics) | **Get** /v3/short-url/statistics/{source}/{source_id} | Get Statistics
[**ShortUrlGetTracking**](UrlShorteningAPI.md#ShortUrlGetTracking) | **Get** /v3/short-url/tracking/{long_url_id} | Get Tracking



## ShortUrlGetStatistics

> GetStatistics ShortUrlGetStatistics(ctx, source, sourceId).ContentType(contentType).Execute()

Get Statistics



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
	source := "source_example" // string | Source of the request.
	sourceId := "sourceId_example" // string | ID of the source (e.g. message ID).
	contentType := "application/json" // string |  (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.UrlShorteningAPI.ShortUrlGetStatistics(context.Background(), source, sourceId).ContentType(contentType).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `UrlShorteningAPI.ShortUrlGetStatistics``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ShortUrlGetStatistics`: GetStatistics
	fmt.Fprintf(os.Stdout, "Response from `UrlShorteningAPI.ShortUrlGetStatistics`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**source** | **string** | Source of the request. | 
**sourceId** | **string** | ID of the source (e.g. message ID). | 

### Other Parameters

Other parameters are passed through a pointer to a apiShortUrlGetStatisticsRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


 **contentType** | **string** |  | 

### Return type

[**GetStatistics**](GetStatistics.md)

### Authorization

[basicAuth](../README.md#basicAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## ShortUrlGetTracking

> GetTracking ShortUrlGetTracking(ctx, longUrlId).ContentType(contentType).Execute()

Get Tracking



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
	longUrlId := "longUrlId_example" // string | ID of the long URL (uniquely defined by the source, source ID, and long URL). Obtained from the GET statistics endpoint.
	contentType := "application/json" // string |  (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.UrlShorteningAPI.ShortUrlGetTracking(context.Background(), longUrlId).ContentType(contentType).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `UrlShorteningAPI.ShortUrlGetTracking``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ShortUrlGetTracking`: GetTracking
	fmt.Fprintf(os.Stdout, "Response from `UrlShorteningAPI.ShortUrlGetTracking`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**longUrlId** | **string** | ID of the long URL (uniquely defined by the source, source ID, and long URL). Obtained from the GET statistics endpoint. | 

### Other Parameters

Other parameters are passed through a pointer to a apiShortUrlGetTrackingRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **contentType** | **string** |  | 

### Return type

[**GetTracking**](GetTracking.md)

### Authorization

[basicAuth](../README.md#basicAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)

