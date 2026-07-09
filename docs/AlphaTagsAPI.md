# \AlphaTagsAPI

All URIs are relative to *https://rest.clicksend.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**DeleteAlphaTag**](AlphaTagsAPI.md#DeleteAlphaTag) | **Delete** /v3/alpha-tags/{alpha_tag_id} | Delete Alpha Tag
[**GetAlphaTag**](AlphaTagsAPI.md#GetAlphaTag) | **Get** /v3/alpha-tags/{alpha_tag_id} | Get Alpha Tag
[**ListAlphaTags**](AlphaTagsAPI.md#ListAlphaTags) | **Get** /v3/alpha-tags | List Alpha Tags
[**RequestAlphaTag**](AlphaTagsAPI.md#RequestAlphaTag) | **Post** /v3/alpha-tags | Request Alpha Tag



## DeleteAlphaTag

> DeleteAlphaTag(ctx, alphaTagId).ContentType(contentType).Execute()

Delete Alpha Tag



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
	alphaTagId := "alphaTagId_example" // string | 
	contentType := "application/json" // string |  (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	r, err := apiClient.AlphaTagsAPI.DeleteAlphaTag(context.Background(), alphaTagId).ContentType(contentType).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `AlphaTagsAPI.DeleteAlphaTag``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**alphaTagId** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiDeleteAlphaTagRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **contentType** | **string** |  | 

### Return type

 (empty response body)

### Authorization

[basicAuth](../README.md#basicAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## GetAlphaTag

> AlphaTag GetAlphaTag(ctx, alphaTagId).ContentType(contentType).Execute()

Get Alpha Tag



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
	alphaTagId := "alphaTagId_example" // string | 
	contentType := "application/json" // string |  (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.AlphaTagsAPI.GetAlphaTag(context.Background(), alphaTagId).ContentType(contentType).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `AlphaTagsAPI.GetAlphaTag``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `GetAlphaTag`: AlphaTag
	fmt.Fprintf(os.Stdout, "Response from `AlphaTagsAPI.GetAlphaTag`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**alphaTagId** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiGetAlphaTagRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **contentType** | **string** |  | 

### Return type

[**AlphaTag**](AlphaTag.md)

### Authorization

[basicAuth](../README.md#basicAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## ListAlphaTags

> ListAlphaTags ListAlphaTags(ctx).SortDirection(sortDirection).PageSize(pageSize).Execute()

List Alpha Tags



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
	sortDirection := "asc" // string | The sort direction for the results. The default value is asc. (optional) (default to "asc")
	pageSize := int32(10) // int32 | The number of items to return per page. This parameter controls the size of each page of results. The default value is 10. (optional) (default to 10)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.AlphaTagsAPI.ListAlphaTags(context.Background()).SortDirection(sortDirection).PageSize(pageSize).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `AlphaTagsAPI.ListAlphaTags``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ListAlphaTags`: ListAlphaTags
	fmt.Fprintf(os.Stdout, "Response from `AlphaTagsAPI.ListAlphaTags`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiListAlphaTagsRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **sortDirection** | **string** | The sort direction for the results. The default value is asc. | [default to &quot;asc&quot;]
 **pageSize** | **int32** | The number of items to return per page. This parameter controls the size of each page of results. The default value is 10. | [default to 10]

### Return type

[**ListAlphaTags**](ListAlphaTags.md)

### Authorization

[basicAuth](../README.md#basicAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## RequestAlphaTag

> AlphaTag RequestAlphaTag(ctx).ContentType(contentType).RequestAlphaTagRequest(requestAlphaTagRequest).Execute()

Request Alpha Tag



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
	requestAlphaTagRequest := *openapiclient.NewRequestAlphaTagRequest() // RequestAlphaTagRequest |  (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.AlphaTagsAPI.RequestAlphaTag(context.Background()).ContentType(contentType).RequestAlphaTagRequest(requestAlphaTagRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `AlphaTagsAPI.RequestAlphaTag``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `RequestAlphaTag`: AlphaTag
	fmt.Fprintf(os.Stdout, "Response from `AlphaTagsAPI.RequestAlphaTag`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiRequestAlphaTagRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **contentType** | **string** |  | 
 **requestAlphaTagRequest** | [**RequestAlphaTagRequest**](RequestAlphaTagRequest.md) |  | 

### Return type

[**AlphaTag**](AlphaTag.md)

### Authorization

[basicAuth](../README.md#basicAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)

