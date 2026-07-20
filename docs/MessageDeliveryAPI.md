# \MessageDeliveryAPI

All URIs are relative to *https://rest.clicksend.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**CreateDeliveryIssue**](MessageDeliveryAPI.md#CreateDeliveryIssue) | **Post** /v3/delivery-issues | Create Delivery Issues
[**GetAllDeliveryIssues**](MessageDeliveryAPI.md#GetAllDeliveryIssues) | **Get** /v3/delivery-issues | Get All Delivery Issues



## CreateDeliveryIssue

> CreateDeliveryIssue CreateDeliveryIssue(ctx).ContentType(contentType).CreateDeliveryIssueRequest(createDeliveryIssueRequest).Execute()

Create Delivery Issues



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
	createDeliveryIssueRequest := *openapiclient.NewCreateDeliveryIssueRequest() // CreateDeliveryIssueRequest |  (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.MessageDeliveryAPI.CreateDeliveryIssue(context.Background()).ContentType(contentType).CreateDeliveryIssueRequest(createDeliveryIssueRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `MessageDeliveryAPI.CreateDeliveryIssue``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `CreateDeliveryIssue`: CreateDeliveryIssue
	fmt.Fprintf(os.Stdout, "Response from `MessageDeliveryAPI.CreateDeliveryIssue`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiCreateDeliveryIssueRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **contentType** | **string** |  | 
 **createDeliveryIssueRequest** | [**CreateDeliveryIssueRequest**](CreateDeliveryIssueRequest.md) |  | 

### Return type

[**CreateDeliveryIssue**](CreateDeliveryIssue.md)

### Authorization

[basicAuth](../README.md#basicAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## GetAllDeliveryIssues

> GetAllDeliveryIssues GetAllDeliveryIssues(ctx).ContentType(contentType).Execute()

Get All Delivery Issues



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
	resp, r, err := apiClient.MessageDeliveryAPI.GetAllDeliveryIssues(context.Background()).ContentType(contentType).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `MessageDeliveryAPI.GetAllDeliveryIssues``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `GetAllDeliveryIssues`: GetAllDeliveryIssues
	fmt.Fprintf(os.Stdout, "Response from `MessageDeliveryAPI.GetAllDeliveryIssues`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiGetAllDeliveryIssuesRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **contentType** | **string** |  | 

### Return type

[**GetAllDeliveryIssues**](GetAllDeliveryIssues.md)

### Authorization

[basicAuth](../README.md#basicAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)

