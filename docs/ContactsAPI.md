# \ContactsAPI

All URIs are relative to *https://rest.clicksend.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**DeleteContact**](ContactsAPI.md#DeleteContact) | **Delete** /v3/lists/{list_id}/contacts/{contact_id} | Delete Contact
[**GetSpecificContact**](ContactsAPI.md#GetSpecificContact) | **Get** /v3/lists/{list_id}/contacts/{contact_id} | Get Specific Contact
[**UpdateContact**](ContactsAPI.md#UpdateContact) | **Put** /v3/lists/{list_id}/contacts/{contact_id} | Update Contact



## DeleteContact

> DeleteContact DeleteContact(ctx, listId, contactId).ContentType(contentType).Execute()

Delete Contact



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
	listId := "listId_example" // string | 
	contactId := "contactId_example" // string | 
	contentType := "application/json" // string |  (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.ContactsAPI.DeleteContact(context.Background(), listId, contactId).ContentType(contentType).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `ContactsAPI.DeleteContact``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `DeleteContact`: DeleteContact
	fmt.Fprintf(os.Stdout, "Response from `ContactsAPI.DeleteContact`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**listId** | **string** |  | 
**contactId** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiDeleteContactRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


 **contentType** | **string** |  | 

### Return type

[**DeleteContact**](DeleteContact.md)

### Authorization

[basicAuth](../README.md#basicAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## GetSpecificContact

> GetSpecificContact GetSpecificContact(ctx, listId, contactId).ContentType(contentType).Execute()

Get Specific Contact



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
	listId := "listId_example" // string | 
	contactId := "contactId_example" // string | 
	contentType := "application/json" // string |  (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.ContactsAPI.GetSpecificContact(context.Background(), listId, contactId).ContentType(contentType).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `ContactsAPI.GetSpecificContact``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `GetSpecificContact`: GetSpecificContact
	fmt.Fprintf(os.Stdout, "Response from `ContactsAPI.GetSpecificContact`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**listId** | **string** |  | 
**contactId** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiGetSpecificContactRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


 **contentType** | **string** |  | 

### Return type

[**GetSpecificContact**](GetSpecificContact.md)

### Authorization

[basicAuth](../README.md#basicAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## UpdateContact

> UpdateContact UpdateContact(ctx, listId, contactId).ContentType(contentType).CreateNewContactRequest(createNewContactRequest).Execute()

Update Contact



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
	listId := "listId_example" // string | 
	contactId := "contactId_example" // string | 
	contentType := "application/json" // string |  (optional)
	createNewContactRequest := *openapiclient.NewCreateNewContactRequest() // CreateNewContactRequest |  (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.ContactsAPI.UpdateContact(context.Background(), listId, contactId).ContentType(contentType).CreateNewContactRequest(createNewContactRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `ContactsAPI.UpdateContact``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `UpdateContact`: UpdateContact
	fmt.Fprintf(os.Stdout, "Response from `ContactsAPI.UpdateContact`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**listId** | **string** |  | 
**contactId** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiUpdateContactRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


 **contentType** | **string** |  | 
 **createNewContactRequest** | [**CreateNewContactRequest**](CreateNewContactRequest.md) |  | 

### Return type

[**UpdateContact**](UpdateContact.md)

### Authorization

[basicAuth](../README.md#basicAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)

