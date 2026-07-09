# \SubaccountsAPI

All URIs are relative to *https://rest.clicksend.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**CreateSubaccount**](SubaccountsAPI.md#CreateSubaccount) | **Post** /v3/subaccounts | Create Subaccount
[**DeleteSubaccount**](SubaccountsAPI.md#DeleteSubaccount) | **Delete** /v3/subaccounts/{subaccount_id} | Delete Subaccount
[**GenerateNewApiKey**](SubaccountsAPI.md#GenerateNewApiKey) | **Put** /v3/subaccounts/{subaccount_id}/regen-api-key | Generate New API Key
[**UpdateSubaccount**](SubaccountsAPI.md#UpdateSubaccount) | **Put** /v3/subaccounts/{subaccount_id} | Update Subaccount
[**ViewSpecificSubaccount**](SubaccountsAPI.md#ViewSpecificSubaccount) | **Get** /v3/subaccounts/{subaccount_id} | View Specific Subaccount
[**ViewSubaccounts**](SubaccountsAPI.md#ViewSubaccounts) | **Get** /v3/subaccounts | View Subaccounts



## CreateSubaccount

> CreateSubaccount CreateSubaccount(ctx).ContentType(contentType).CreateSubaccountRequest(createSubaccountRequest).Execute()

Create Subaccount



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
	createSubaccountRequest := *openapiclient.NewCreateSubaccountRequest() // CreateSubaccountRequest |  (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.SubaccountsAPI.CreateSubaccount(context.Background()).ContentType(contentType).CreateSubaccountRequest(createSubaccountRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `SubaccountsAPI.CreateSubaccount``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `CreateSubaccount`: CreateSubaccount
	fmt.Fprintf(os.Stdout, "Response from `SubaccountsAPI.CreateSubaccount`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiCreateSubaccountRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **contentType** | **string** |  | 
 **createSubaccountRequest** | [**CreateSubaccountRequest**](CreateSubaccountRequest.md) |  | 

### Return type

[**CreateSubaccount**](CreateSubaccount.md)

### Authorization

[basicAuth](../README.md#basicAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## DeleteSubaccount

> DeleteSubaccount DeleteSubaccount(ctx, subaccountId).ContentType(contentType).Execute()

Delete Subaccount



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
	subaccountId := "subaccountId_example" // string | 
	contentType := "application/json" // string |  (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.SubaccountsAPI.DeleteSubaccount(context.Background(), subaccountId).ContentType(contentType).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `SubaccountsAPI.DeleteSubaccount``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `DeleteSubaccount`: DeleteSubaccount
	fmt.Fprintf(os.Stdout, "Response from `SubaccountsAPI.DeleteSubaccount`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**subaccountId** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiDeleteSubaccountRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **contentType** | **string** |  | 

### Return type

[**DeleteSubaccount**](DeleteSubaccount.md)

### Authorization

[basicAuth](../README.md#basicAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## GenerateNewApiKey

> GenerateNewApiKey GenerateNewApiKey(ctx, subaccountId).ContentType(contentType).GenerateNewApiKeyRequest(generateNewApiKeyRequest).Execute()

Generate New API Key



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
	subaccountId := "subaccountId_example" // string | 
	contentType := "application/json" // string |  (optional)
	generateNewApiKeyRequest := *openapiclient.NewGenerateNewApiKeyRequest() // GenerateNewApiKeyRequest |  (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.SubaccountsAPI.GenerateNewApiKey(context.Background(), subaccountId).ContentType(contentType).GenerateNewApiKeyRequest(generateNewApiKeyRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `SubaccountsAPI.GenerateNewApiKey``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `GenerateNewApiKey`: GenerateNewApiKey
	fmt.Fprintf(os.Stdout, "Response from `SubaccountsAPI.GenerateNewApiKey`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**subaccountId** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiGenerateNewApiKeyRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **contentType** | **string** |  | 
 **generateNewApiKeyRequest** | [**GenerateNewApiKeyRequest**](GenerateNewApiKeyRequest.md) |  | 

### Return type

[**GenerateNewApiKey**](GenerateNewApiKey.md)

### Authorization

[basicAuth](../README.md#basicAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## UpdateSubaccount

> UpdateSubaccount UpdateSubaccount(ctx, subaccountId).ContentType(contentType).UpdateSubaccountRequest(updateSubaccountRequest).Execute()

Update Subaccount



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
	subaccountId := "subaccountId_example" // string | 
	contentType := "application/json" // string |  (optional)
	updateSubaccountRequest := *openapiclient.NewUpdateSubaccountRequest() // UpdateSubaccountRequest |  (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.SubaccountsAPI.UpdateSubaccount(context.Background(), subaccountId).ContentType(contentType).UpdateSubaccountRequest(updateSubaccountRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `SubaccountsAPI.UpdateSubaccount``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `UpdateSubaccount`: UpdateSubaccount
	fmt.Fprintf(os.Stdout, "Response from `SubaccountsAPI.UpdateSubaccount`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**subaccountId** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiUpdateSubaccountRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **contentType** | **string** |  | 
 **updateSubaccountRequest** | [**UpdateSubaccountRequest**](UpdateSubaccountRequest.md) |  | 

### Return type

[**UpdateSubaccount**](UpdateSubaccount.md)

### Authorization

[basicAuth](../README.md#basicAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## ViewSpecificSubaccount

> ViewSpecificSubaccount ViewSpecificSubaccount(ctx, subaccountId).ContentType(contentType).Execute()

View Specific Subaccount



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
	subaccountId := "subaccountId_example" // string | 
	contentType := "application/json" // string |  (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.SubaccountsAPI.ViewSpecificSubaccount(context.Background(), subaccountId).ContentType(contentType).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `SubaccountsAPI.ViewSpecificSubaccount``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ViewSpecificSubaccount`: ViewSpecificSubaccount
	fmt.Fprintf(os.Stdout, "Response from `SubaccountsAPI.ViewSpecificSubaccount`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**subaccountId** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiViewSpecificSubaccountRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **contentType** | **string** |  | 

### Return type

[**ViewSpecificSubaccount**](ViewSpecificSubaccount.md)

### Authorization

[basicAuth](../README.md#basicAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## ViewSubaccounts

> ViewSubaccounts ViewSubaccounts(ctx).ContentType(contentType).Execute()

View Subaccounts



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
	resp, r, err := apiClient.SubaccountsAPI.ViewSubaccounts(context.Background()).ContentType(contentType).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `SubaccountsAPI.ViewSubaccounts``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ViewSubaccounts`: ViewSubaccounts
	fmt.Fprintf(os.Stdout, "Response from `SubaccountsAPI.ViewSubaccounts`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiViewSubaccountsRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **contentType** | **string** |  | 

### Return type

[**ViewSubaccounts**](ViewSubaccounts.md)

### Authorization

[basicAuth](../README.md#basicAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)

