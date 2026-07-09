# \ResellerAPI

All URIs are relative to *https://rest.clicksend.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**CreateResellerAccount**](ResellerAPI.md#CreateResellerAccount) | **Post** /v3/reseller/accounts | Create Reseller Account
[**ResellerTransferCredit**](ResellerAPI.md#ResellerTransferCredit) | **Put** /v3/reseller/transfer-credit | Reseller Transfer Credit
[**UpdateClientAccount**](ResellerAPI.md#UpdateClientAccount) | **Put** /v3/reseller/accounts/{client_user_id} | Update Client Account
[**ViewClientAccounts**](ResellerAPI.md#ViewClientAccounts) | **Get** /v3/reseller/accounts | View Client Accounts
[**ViewSpecificClientAccount**](ResellerAPI.md#ViewSpecificClientAccount) | **Get** /v3/reseller/accounts/{client_user_id} | View Specific Client Account



## CreateResellerAccount

> CreateResellerAccount CreateResellerAccount(ctx).ContentType(contentType).CreateResellerAccountRequest(createResellerAccountRequest).Execute()

Create Reseller Account



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
	createResellerAccountRequest := *openapiclient.NewCreateResellerAccountRequest() // CreateResellerAccountRequest |  (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.ResellerAPI.CreateResellerAccount(context.Background()).ContentType(contentType).CreateResellerAccountRequest(createResellerAccountRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `ResellerAPI.CreateResellerAccount``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `CreateResellerAccount`: CreateResellerAccount
	fmt.Fprintf(os.Stdout, "Response from `ResellerAPI.CreateResellerAccount`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiCreateResellerAccountRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **contentType** | **string** |  | 
 **createResellerAccountRequest** | [**CreateResellerAccountRequest**](CreateResellerAccountRequest.md) |  | 

### Return type

[**CreateResellerAccount**](CreateResellerAccount.md)

### Authorization

[basicAuth](../README.md#basicAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## ResellerTransferCredit

> ResellerTransferCredit ResellerTransferCredit(ctx).ContentType(contentType).UpdatePaymentInfoRequest(updatePaymentInfoRequest).Execute()

Reseller Transfer Credit



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
	contentType := "application/x-www-form-urlencoded" // string |  (optional)
	updatePaymentInfoRequest := *openapiclient.NewUpdatePaymentInfoRequest() // UpdatePaymentInfoRequest |  (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.ResellerAPI.ResellerTransferCredit(context.Background()).ContentType(contentType).UpdatePaymentInfoRequest(updatePaymentInfoRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `ResellerAPI.ResellerTransferCredit``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ResellerTransferCredit`: ResellerTransferCredit
	fmt.Fprintf(os.Stdout, "Response from `ResellerAPI.ResellerTransferCredit`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiResellerTransferCreditRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **contentType** | **string** |  | 
 **updatePaymentInfoRequest** | [**UpdatePaymentInfoRequest**](UpdatePaymentInfoRequest.md) |  | 

### Return type

[**ResellerTransferCredit**](ResellerTransferCredit.md)

### Authorization

[basicAuth](../README.md#basicAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## UpdateClientAccount

> UpdateClientAccount UpdateClientAccount(ctx, clientUserId).ContentType(contentType).UpdatePaymentInfoRequest(updatePaymentInfoRequest).Execute()

Update Client Account



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
	clientUserId := "clientUserId_example" // string | 
	contentType := "application/x-www-form-urlencoded" // string |  (optional)
	updatePaymentInfoRequest := *openapiclient.NewUpdatePaymentInfoRequest() // UpdatePaymentInfoRequest |  (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.ResellerAPI.UpdateClientAccount(context.Background(), clientUserId).ContentType(contentType).UpdatePaymentInfoRequest(updatePaymentInfoRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `ResellerAPI.UpdateClientAccount``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `UpdateClientAccount`: UpdateClientAccount
	fmt.Fprintf(os.Stdout, "Response from `ResellerAPI.UpdateClientAccount`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**clientUserId** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiUpdateClientAccountRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **contentType** | **string** |  | 
 **updatePaymentInfoRequest** | [**UpdatePaymentInfoRequest**](UpdatePaymentInfoRequest.md) |  | 

### Return type

[**UpdateClientAccount**](UpdateClientAccount.md)

### Authorization

[basicAuth](../README.md#basicAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## ViewClientAccounts

> ViewClientAccounts ViewClientAccounts(ctx).ContentType(contentType).Execute()

View Client Accounts



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
	resp, r, err := apiClient.ResellerAPI.ViewClientAccounts(context.Background()).ContentType(contentType).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `ResellerAPI.ViewClientAccounts``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ViewClientAccounts`: ViewClientAccounts
	fmt.Fprintf(os.Stdout, "Response from `ResellerAPI.ViewClientAccounts`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiViewClientAccountsRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **contentType** | **string** |  | 

### Return type

[**ViewClientAccounts**](ViewClientAccounts.md)

### Authorization

[basicAuth](../README.md#basicAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## ViewSpecificClientAccount

> ViewSpecificClientAccount ViewSpecificClientAccount(ctx, clientUserId).ContentType(contentType).Execute()

View Specific Client Account



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
	clientUserId := "clientUserId_example" // string | 
	contentType := "application/json" // string |  (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.ResellerAPI.ViewSpecificClientAccount(context.Background(), clientUserId).ContentType(contentType).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `ResellerAPI.ViewSpecificClientAccount``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ViewSpecificClientAccount`: ViewSpecificClientAccount
	fmt.Fprintf(os.Stdout, "Response from `ResellerAPI.ViewSpecificClientAccount`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**clientUserId** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiViewSpecificClientAccountRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **contentType** | **string** |  | 

### Return type

[**ViewSpecificClientAccount**](ViewSpecificClientAccount.md)

### Authorization

[basicAuth](../README.md#basicAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)

