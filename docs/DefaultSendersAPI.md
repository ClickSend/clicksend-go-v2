# \DefaultSendersAPI

All URIs are relative to *https://rest.clicksend.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**CreateDefaultSender**](DefaultSendersAPI.md#CreateDefaultSender) | **Post** /v3/senders/default-senders | Create Default Sender
[**DeleteDefaultSender**](DefaultSendersAPI.md#DeleteDefaultSender) | **Delete** /v3/senders/default-senders/{default_sender_id} | Delete Default Sender
[**GetDefaultSenderDetails**](DefaultSendersAPI.md#GetDefaultSenderDetails) | **Get** /v3/senders/default-senders/{default_sender_id} | Get Default Sender Details
[**GetDefaultSendersList**](DefaultSendersAPI.md#GetDefaultSendersList) | **Get** /v3/senders/default-senders | Get List of Default Senders
[**ListCompliantSenderTypes**](DefaultSendersAPI.md#ListCompliantSenderTypes) | **Get** /v3/senders/compliant-sender-types | List Compliant Sender Types
[**UpdateDefaultSender**](DefaultSendersAPI.md#UpdateDefaultSender) | **Patch** /v3/senders/default-senders/{default_sender_id} | Update Default Sender



## CreateDefaultSender

> CreateDefaultSender CreateDefaultSender(ctx).ContentType(contentType).CreateDefaultSenderRequest(createDefaultSenderRequest).Execute()

Create Default Sender



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
	createDefaultSenderRequest := *openapiclient.NewCreateDefaultSenderRequest("AU", "ProductType_example", []openapiclient.CreateDefaultSenderRequestDefaultSenderStrategiesInner{*openapiclient.NewCreateDefaultSenderRequestDefaultSenderStrategiesInner("SenderType_example", "SenderId_example")}) // CreateDefaultSenderRequest |  (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.DefaultSendersAPI.CreateDefaultSender(context.Background()).ContentType(contentType).CreateDefaultSenderRequest(createDefaultSenderRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `DefaultSendersAPI.CreateDefaultSender``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `CreateDefaultSender`: CreateDefaultSender
	fmt.Fprintf(os.Stdout, "Response from `DefaultSendersAPI.CreateDefaultSender`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiCreateDefaultSenderRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **contentType** | **string** |  | 
 **createDefaultSenderRequest** | [**CreateDefaultSenderRequest**](CreateDefaultSenderRequest.md) |  | 

### Return type

[**CreateDefaultSender**](CreateDefaultSender.md)

### Authorization

[basicAuth](../README.md#basicAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## DeleteDefaultSender

> DeleteDefaultSender(ctx, defaultSenderId).ContentType(contentType).Execute()

Delete Default Sender



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
	defaultSenderId := "defaultSenderId_example" // string | The ID of the default sender to delete
	contentType := "application/json" // string |  (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	r, err := apiClient.DefaultSendersAPI.DeleteDefaultSender(context.Background(), defaultSenderId).ContentType(contentType).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `DefaultSendersAPI.DeleteDefaultSender``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**defaultSenderId** | **string** | The ID of the default sender to delete | 

### Other Parameters

Other parameters are passed through a pointer to a apiDeleteDefaultSenderRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **contentType** | **string** |  | 

### Return type

 (empty response body)

### Authorization

[basicAuth](../README.md#basicAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## GetDefaultSenderDetails

> GetDefaultSenderDetails GetDefaultSenderDetails(ctx, defaultSenderId).ContentType(contentType).Execute()

Get Default Sender Details



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
	defaultSenderId := "defaultSenderId_example" // string | The ID of the default sender to retrieve
	contentType := "application/json" // string |  (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.DefaultSendersAPI.GetDefaultSenderDetails(context.Background(), defaultSenderId).ContentType(contentType).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `DefaultSendersAPI.GetDefaultSenderDetails``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `GetDefaultSenderDetails`: GetDefaultSenderDetails
	fmt.Fprintf(os.Stdout, "Response from `DefaultSendersAPI.GetDefaultSenderDetails`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**defaultSenderId** | **string** | The ID of the default sender to retrieve | 

### Other Parameters

Other parameters are passed through a pointer to a apiGetDefaultSenderDetailsRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **contentType** | **string** |  | 

### Return type

[**GetDefaultSenderDetails**](GetDefaultSenderDetails.md)

### Authorization

[basicAuth](../README.md#basicAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## GetDefaultSendersList

> GetDefaultSendersList GetDefaultSendersList(ctx).ContentType(contentType).Offset(offset).PerPage(perPage).SortBy(sortBy).SortDirection(sortDirection).Execute()

Get List of Default Senders



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
	offset := "offset_example" // string | Page (offset) to be used for pagination (optional)
	perPage := int32(56) // int32 | Size of the page in pagination (optional) (default to 10)
	sortBy := "sortBy_example" // string | Parameter to sort the results by (optional) (default to "created_timestamp")
	sortDirection := "sortDirection_example" // string | Direction of sorting (optional) (default to "desc")

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.DefaultSendersAPI.GetDefaultSendersList(context.Background()).ContentType(contentType).Offset(offset).PerPage(perPage).SortBy(sortBy).SortDirection(sortDirection).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `DefaultSendersAPI.GetDefaultSendersList``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `GetDefaultSendersList`: GetDefaultSendersList
	fmt.Fprintf(os.Stdout, "Response from `DefaultSendersAPI.GetDefaultSendersList`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiGetDefaultSendersListRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **contentType** | **string** |  | 
 **offset** | **string** | Page (offset) to be used for pagination | 
 **perPage** | **int32** | Size of the page in pagination | [default to 10]
 **sortBy** | **string** | Parameter to sort the results by | [default to &quot;created_timestamp&quot;]
 **sortDirection** | **string** | Direction of sorting | [default to &quot;desc&quot;]

### Return type

[**GetDefaultSendersList**](GetDefaultSendersList.md)

### Authorization

[basicAuth](../README.md#basicAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## ListCompliantSenderTypes

> ListCompliantSenderTypes200Response ListCompliantSenderTypes(ctx).FilterProductType(filterProductType).FilterCountryCodeIndex(filterCountryCodeIndex).Execute()

List Compliant Sender Types



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
	filterProductType := "SMS" // string | Type of the product
	filterCountryCodeIndex := []string{"Inner_example"} // []string | Array of recipient country codes (ISO 3166-1 alpha-2). If not specified, will get all compliant sender types for all countries. Replace `{index}` with the appropriate index value.  <small>Example:</small> <small><code style=\"color: #424242;\">filter[country_code][0]=US&filter[country_code][1]=AU</code></small>  (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.DefaultSendersAPI.ListCompliantSenderTypes(context.Background()).FilterProductType(filterProductType).FilterCountryCodeIndex(filterCountryCodeIndex).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `DefaultSendersAPI.ListCompliantSenderTypes``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ListCompliantSenderTypes`: ListCompliantSenderTypes200Response
	fmt.Fprintf(os.Stdout, "Response from `DefaultSendersAPI.ListCompliantSenderTypes`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiListCompliantSenderTypesRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **filterProductType** | **string** | Type of the product | 
 **filterCountryCodeIndex** | **[]string** | Array of recipient country codes (ISO 3166-1 alpha-2). If not specified, will get all compliant sender types for all countries. Replace &#x60;{index}&#x60; with the appropriate index value.  &lt;small&gt;Example:&lt;/small&gt; &lt;small&gt;&lt;code style&#x3D;\&quot;color: #424242;\&quot;&gt;filter[country_code][0]&#x3D;US&amp;filter[country_code][1]&#x3D;AU&lt;/code&gt;&lt;/small&gt;  | 

### Return type

[**ListCompliantSenderTypes200Response**](ListCompliantSenderTypes200Response.md)

### Authorization

[basicAuth](../README.md#basicAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## UpdateDefaultSender

> UpdateDefaultSender UpdateDefaultSender(ctx, defaultSenderId).ContentType(contentType).UpdateDefaultSenderRequest(updateDefaultSenderRequest).Execute()

Update Default Sender



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
	defaultSenderId := "defaultSenderId_example" // string | The ID of the default sender to update
	contentType := "application/json" // string |  (optional)
	updateDefaultSenderRequest := *openapiclient.NewUpdateDefaultSenderRequest([]openapiclient.CreateDefaultSenderRequestDefaultSenderStrategiesInner{*openapiclient.NewCreateDefaultSenderRequestDefaultSenderStrategiesInner("SenderType_example", "SenderId_example")}) // UpdateDefaultSenderRequest |  (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.DefaultSendersAPI.UpdateDefaultSender(context.Background(), defaultSenderId).ContentType(contentType).UpdateDefaultSenderRequest(updateDefaultSenderRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `DefaultSendersAPI.UpdateDefaultSender``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `UpdateDefaultSender`: UpdateDefaultSender
	fmt.Fprintf(os.Stdout, "Response from `DefaultSendersAPI.UpdateDefaultSender`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**defaultSenderId** | **string** | The ID of the default sender to update | 

### Other Parameters

Other parameters are passed through a pointer to a apiUpdateDefaultSenderRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **contentType** | **string** |  | 
 **updateDefaultSenderRequest** | [**UpdateDefaultSenderRequest**](UpdateDefaultSenderRequest.md) |  | 

### Return type

[**UpdateDefaultSender**](UpdateDefaultSender.md)

### Authorization

[basicAuth](../README.md#basicAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)

