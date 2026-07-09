# \AddressesAPI

All URIs are relative to *https://rest.clicksend.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**CreateReturnAddress**](AddressesAPI.md#CreateReturnAddress) | **Post** /v3/post/return-addresses | Create Return Address
[**DeleteReturnAddress**](AddressesAPI.md#DeleteReturnAddress) | **Delete** /v3/post/return-addresses/{return_address_id} | Delete Return Address
[**UpdateReturnAddress**](AddressesAPI.md#UpdateReturnAddress) | **Put** /v3/post/return-addresses/{return_address_id} | Update Return Address
[**ViewSpecificReturnAddress**](AddressesAPI.md#ViewSpecificReturnAddress) | **Get** /v3/post/return-addresses/{return_address_id} | View Specific Return Address
[**ViewYourReturnAddresses**](AddressesAPI.md#ViewYourReturnAddresses) | **Get** /v3/post/return-addresses | View Your Return Addresses



## CreateReturnAddress

> CreateReturnAddress CreateReturnAddress(ctx).ContentType(contentType).CreateReturnAddressRequest(createReturnAddressRequest).Execute()

Create Return Address



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
	createReturnAddressRequest := *openapiclient.NewCreateReturnAddressRequest() // CreateReturnAddressRequest |  (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.AddressesAPI.CreateReturnAddress(context.Background()).ContentType(contentType).CreateReturnAddressRequest(createReturnAddressRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `AddressesAPI.CreateReturnAddress``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `CreateReturnAddress`: CreateReturnAddress
	fmt.Fprintf(os.Stdout, "Response from `AddressesAPI.CreateReturnAddress`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiCreateReturnAddressRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **contentType** | **string** |  | 
 **createReturnAddressRequest** | [**CreateReturnAddressRequest**](CreateReturnAddressRequest.md) |  | 

### Return type

[**CreateReturnAddress**](CreateReturnAddress.md)

### Authorization

[basicAuth](../README.md#basicAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## DeleteReturnAddress

> DeleteReturnAddress DeleteReturnAddress(ctx, returnAddressId).ContentType(contentType).Execute()

Delete Return Address



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
	returnAddressId := "returnAddressId_example" // string | 
	contentType := "application/json" // string |  (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.AddressesAPI.DeleteReturnAddress(context.Background(), returnAddressId).ContentType(contentType).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `AddressesAPI.DeleteReturnAddress``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `DeleteReturnAddress`: DeleteReturnAddress
	fmt.Fprintf(os.Stdout, "Response from `AddressesAPI.DeleteReturnAddress`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**returnAddressId** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiDeleteReturnAddressRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **contentType** | **string** |  | 

### Return type

[**DeleteReturnAddress**](DeleteReturnAddress.md)

### Authorization

[basicAuth](../README.md#basicAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## UpdateReturnAddress

> UpdateReturnAddress UpdateReturnAddress(ctx, returnAddressId).ContentType(contentType).UpdateReturnAddressRequest(updateReturnAddressRequest).Execute()

Update Return Address



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
	returnAddressId := "returnAddressId_example" // string | 
	contentType := "application/json" // string |  (optional)
	updateReturnAddressRequest := *openapiclient.NewUpdateReturnAddressRequest() // UpdateReturnAddressRequest |  (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.AddressesAPI.UpdateReturnAddress(context.Background(), returnAddressId).ContentType(contentType).UpdateReturnAddressRequest(updateReturnAddressRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `AddressesAPI.UpdateReturnAddress``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `UpdateReturnAddress`: UpdateReturnAddress
	fmt.Fprintf(os.Stdout, "Response from `AddressesAPI.UpdateReturnAddress`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**returnAddressId** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiUpdateReturnAddressRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **contentType** | **string** |  | 
 **updateReturnAddressRequest** | [**UpdateReturnAddressRequest**](UpdateReturnAddressRequest.md) |  | 

### Return type

[**UpdateReturnAddress**](UpdateReturnAddress.md)

### Authorization

[basicAuth](../README.md#basicAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## ViewSpecificReturnAddress

> ViewSpecificReturnAddress ViewSpecificReturnAddress(ctx, returnAddressId).ContentType(contentType).Execute()

View Specific Return Address



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
	returnAddressId := "returnAddressId_example" // string | 
	contentType := "application/json" // string |  (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.AddressesAPI.ViewSpecificReturnAddress(context.Background(), returnAddressId).ContentType(contentType).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `AddressesAPI.ViewSpecificReturnAddress``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ViewSpecificReturnAddress`: ViewSpecificReturnAddress
	fmt.Fprintf(os.Stdout, "Response from `AddressesAPI.ViewSpecificReturnAddress`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**returnAddressId** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiViewSpecificReturnAddressRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **contentType** | **string** |  | 

### Return type

[**ViewSpecificReturnAddress**](ViewSpecificReturnAddress.md)

### Authorization

[basicAuth](../README.md#basicAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## ViewYourReturnAddresses

> ViewYourReturnAddresses ViewYourReturnAddresses(ctx).ContentType(contentType).Execute()

View Your Return Addresses



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
	resp, r, err := apiClient.AddressesAPI.ViewYourReturnAddresses(context.Background()).ContentType(contentType).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `AddressesAPI.ViewYourReturnAddresses``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ViewYourReturnAddresses`: ViewYourReturnAddresses
	fmt.Fprintf(os.Stdout, "Response from `AddressesAPI.ViewYourReturnAddresses`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiViewYourReturnAddressesRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **contentType** | **string** |  | 

### Return type

[**ViewYourReturnAddresses**](ViewYourReturnAddresses.md)

### Authorization

[basicAuth](../README.md#basicAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)

