# \ListsAPI

All URIs are relative to *https://rest.clicksend.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**CopyContactToList**](ListsAPI.md#CopyContactToList) | **Put** /v3/lists/{from_list_id}/contacts/{contact_id}/copy/{to_list_id} | Copy Contact to List
[**CreateList**](ListsAPI.md#CreateList) | **Post** /v3/lists | Create List
[**CreateNewContact**](ListsAPI.md#CreateNewContact) | **Post** /v3/lists/{list_id}/contacts | Create New Contact
[**DeleteList**](ListsAPI.md#DeleteList) | **Delete** /v3/lists/{list_id} | Delete List
[**ImportContacts**](ListsAPI.md#ImportContacts) | **Post** /v3/lists/{list_id}/import | Import Contacts
[**RemoveDuplicateContacts**](ListsAPI.md#RemoveDuplicateContacts) | **Put** /v3/lists/{list_id}/remove-duplicates/ | Remove Duplicate Contacts
[**RemoveOptedOutContacts**](ListsAPI.md#RemoveOptedOutContacts) | **Put** /v3/lists/{list_id}/remove-opted-out-contacts/{opt_out_list_id} | Remove Opted Out Contacts
[**TransferContactToList**](ListsAPI.md#TransferContactToList) | **Put** /v3/lists/{from_list_id}/contacts/{contact_id}/transfer/{to_list_id} | Transfer Contact to List
[**UpdateList**](ListsAPI.md#UpdateList) | **Put** /v3/lists/{list_id} | Update List
[**ViewContactLists**](ListsAPI.md#ViewContactLists) | **Get** /v3/search/contacts-lists | View Contact Lists
[**ViewListContacts**](ListsAPI.md#ViewListContacts) | **Get** /v3/lists/{list_id}/contacts | View List Contacts
[**ViewLists**](ListsAPI.md#ViewLists) | **Get** /v3/lists | View Lists
[**ViewSpecificList**](ListsAPI.md#ViewSpecificList) | **Get** /v3/lists/{list_id} | View Specific List



## CopyContactToList

> CopyContactToList CopyContactToList(ctx, fromListId, contactId, toListId).ContentType(contentType).Body(body).Execute()

Copy Contact to List



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
	fromListId := "fromListId_example" // string | 
	contactId := "contactId_example" // string | 
	toListId := "toListId_example" // string | 
	contentType := "application/json" // string |  (optional)
	body := map[string]interface{}{ ... } // map[string]interface{} |  (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.ListsAPI.CopyContactToList(context.Background(), fromListId, contactId, toListId).ContentType(contentType).Body(body).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `ListsAPI.CopyContactToList``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `CopyContactToList`: CopyContactToList
	fmt.Fprintf(os.Stdout, "Response from `ListsAPI.CopyContactToList`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**fromListId** | **string** |  | 
**contactId** | **string** |  | 
**toListId** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiCopyContactToListRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------



 **contentType** | **string** |  | 
 **body** | **map[string]interface{}** |  | 

### Return type

[**CopyContactToList**](CopyContactToList.md)

### Authorization

[basicAuth](../README.md#basicAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## CreateList

> CreateList CreateList(ctx).ContentType(contentType).CreateListRequest(createListRequest).Execute()

Create List



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
	createListRequest := *openapiclient.NewCreateListRequest() // CreateListRequest |  (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.ListsAPI.CreateList(context.Background()).ContentType(contentType).CreateListRequest(createListRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `ListsAPI.CreateList``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `CreateList`: CreateList
	fmt.Fprintf(os.Stdout, "Response from `ListsAPI.CreateList`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiCreateListRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **contentType** | **string** |  | 
 **createListRequest** | [**CreateListRequest**](CreateListRequest.md) |  | 

### Return type

[**CreateList**](CreateList.md)

### Authorization

[basicAuth](../README.md#basicAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## CreateNewContact

> CreateNewContact CreateNewContact(ctx, listId).ContentType(contentType).CreateNewContactRequest(createNewContactRequest).Execute()

Create New Contact



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
	listId := "listId_example" // string | 
	contentType := "application/json" // string |  (optional)
	createNewContactRequest := *openapiclient.NewCreateNewContactRequest() // CreateNewContactRequest |  (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.ListsAPI.CreateNewContact(context.Background(), listId).ContentType(contentType).CreateNewContactRequest(createNewContactRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `ListsAPI.CreateNewContact``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `CreateNewContact`: CreateNewContact
	fmt.Fprintf(os.Stdout, "Response from `ListsAPI.CreateNewContact`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**listId** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiCreateNewContactRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **contentType** | **string** |  | 
 **createNewContactRequest** | [**CreateNewContactRequest**](CreateNewContactRequest.md) |  | 

### Return type

[**CreateNewContact**](CreateNewContact.md)

### Authorization

[basicAuth](../README.md#basicAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## DeleteList

> DeleteList DeleteList(ctx, listId).ContentType(contentType).Execute()

Delete List



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
	listId := "listId_example" // string | 
	contentType := "application/json" // string |  (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.ListsAPI.DeleteList(context.Background(), listId).ContentType(contentType).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `ListsAPI.DeleteList``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `DeleteList`: DeleteList
	fmt.Fprintf(os.Stdout, "Response from `ListsAPI.DeleteList`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**listId** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiDeleteListRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **contentType** | **string** |  | 

### Return type

[**DeleteList**](DeleteList.md)

### Authorization

[basicAuth](../README.md#basicAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## ImportContacts

> ImportContacts ImportContacts(ctx, listId).ContentType(contentType).ImportContactsRequest(importContactsRequest).Execute()

Import Contacts



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
	listId := "listId_example" // string | 
	contentType := "application/json" // string |  (optional)
	importContactsRequest := *openapiclient.NewImportContactsRequest() // ImportContactsRequest |  (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.ListsAPI.ImportContacts(context.Background(), listId).ContentType(contentType).ImportContactsRequest(importContactsRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `ListsAPI.ImportContacts``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ImportContacts`: ImportContacts
	fmt.Fprintf(os.Stdout, "Response from `ListsAPI.ImportContacts`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**listId** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiImportContactsRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **contentType** | **string** |  | 
 **importContactsRequest** | [**ImportContactsRequest**](ImportContactsRequest.md) |  | 

### Return type

[**ImportContacts**](ImportContacts.md)

### Authorization

[basicAuth](../README.md#basicAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## RemoveDuplicateContacts

> RemoveDuplicateContacts RemoveDuplicateContacts(ctx, listId).ContentType(contentType).RemoveDuplicateContactsRequest(removeDuplicateContactsRequest).Execute()

Remove Duplicate Contacts



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
	listId := "listId_example" // string | 
	contentType := "application/json" // string |  (optional)
	removeDuplicateContactsRequest := *openapiclient.NewRemoveDuplicateContactsRequest() // RemoveDuplicateContactsRequest |  (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.ListsAPI.RemoveDuplicateContacts(context.Background(), listId).ContentType(contentType).RemoveDuplicateContactsRequest(removeDuplicateContactsRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `ListsAPI.RemoveDuplicateContacts``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `RemoveDuplicateContacts`: RemoveDuplicateContacts
	fmt.Fprintf(os.Stdout, "Response from `ListsAPI.RemoveDuplicateContacts`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**listId** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiRemoveDuplicateContactsRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **contentType** | **string** |  | 
 **removeDuplicateContactsRequest** | [**RemoveDuplicateContactsRequest**](RemoveDuplicateContactsRequest.md) |  | 

### Return type

[**RemoveDuplicateContacts**](RemoveDuplicateContacts.md)

### Authorization

[basicAuth](../README.md#basicAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## RemoveOptedOutContacts

> RemoveOptedOutContacts RemoveOptedOutContacts(ctx, listId, optOutListId).ContentType(contentType).Body(body).Execute()

Remove Opted Out Contacts



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
	listId := "listId_example" // string | 
	optOutListId := "optOutListId_example" // string | 
	contentType := "application/json" // string |  (optional)
	body := map[string]interface{}{ ... } // map[string]interface{} |  (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.ListsAPI.RemoveOptedOutContacts(context.Background(), listId, optOutListId).ContentType(contentType).Body(body).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `ListsAPI.RemoveOptedOutContacts``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `RemoveOptedOutContacts`: RemoveOptedOutContacts
	fmt.Fprintf(os.Stdout, "Response from `ListsAPI.RemoveOptedOutContacts`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**listId** | **string** |  | 
**optOutListId** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiRemoveOptedOutContactsRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


 **contentType** | **string** |  | 
 **body** | **map[string]interface{}** |  | 

### Return type

[**RemoveOptedOutContacts**](RemoveOptedOutContacts.md)

### Authorization

[basicAuth](../README.md#basicAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## TransferContactToList

> TransferContactToList TransferContactToList(ctx, fromListId, contactId, toListId).ContentType(contentType).Body(body).Execute()

Transfer Contact to List



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
	fromListId := "fromListId_example" // string | 
	contactId := "contactId_example" // string | 
	toListId := "toListId_example" // string | 
	contentType := "application/json" // string |  (optional)
	body := map[string]interface{}{ ... } // map[string]interface{} |  (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.ListsAPI.TransferContactToList(context.Background(), fromListId, contactId, toListId).ContentType(contentType).Body(body).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `ListsAPI.TransferContactToList``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `TransferContactToList`: TransferContactToList
	fmt.Fprintf(os.Stdout, "Response from `ListsAPI.TransferContactToList`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**fromListId** | **string** |  | 
**contactId** | **string** |  | 
**toListId** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiTransferContactToListRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------



 **contentType** | **string** |  | 
 **body** | **map[string]interface{}** |  | 

### Return type

[**TransferContactToList**](TransferContactToList.md)

### Authorization

[basicAuth](../README.md#basicAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## UpdateList

> UpdateList UpdateList(ctx, listId).ContentType(contentType).CreateListRequest(createListRequest).Execute()

Update List



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
	listId := "listId_example" // string | 
	contentType := "application/json" // string |  (optional)
	createListRequest := *openapiclient.NewCreateListRequest() // CreateListRequest |  (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.ListsAPI.UpdateList(context.Background(), listId).ContentType(contentType).CreateListRequest(createListRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `ListsAPI.UpdateList``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `UpdateList`: UpdateList
	fmt.Fprintf(os.Stdout, "Response from `ListsAPI.UpdateList`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**listId** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiUpdateListRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **contentType** | **string** |  | 
 **createListRequest** | [**CreateListRequest**](CreateListRequest.md) |  | 

### Return type

[**UpdateList**](UpdateList.md)

### Authorization

[basicAuth](../README.md#basicAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## ViewContactLists

> ViewContactLists(ctx).Q(q).Execute()

View Contact Lists



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
	q := "Test" // string |  (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	r, err := apiClient.ListsAPI.ViewContactLists(context.Background()).Q(q).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `ListsAPI.ViewContactLists``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiViewContactListsRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **q** | **string** |  | 

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


## ViewListContacts

> ViewListContacts ViewListContacts(ctx, listId).ContentType(contentType).Execute()

View List Contacts



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
	listId := "listId_example" // string | 
	contentType := "application/json" // string |  (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.ListsAPI.ViewListContacts(context.Background(), listId).ContentType(contentType).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `ListsAPI.ViewListContacts``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ViewListContacts`: ViewListContacts
	fmt.Fprintf(os.Stdout, "Response from `ListsAPI.ViewListContacts`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**listId** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiViewListContactsRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **contentType** | **string** |  | 

### Return type

[**ViewListContacts**](ViewListContacts.md)

### Authorization

[basicAuth](../README.md#basicAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## ViewLists

> ViewLists ViewLists(ctx).ContentType(contentType).Execute()

View Lists



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
	resp, r, err := apiClient.ListsAPI.ViewLists(context.Background()).ContentType(contentType).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `ListsAPI.ViewLists``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ViewLists`: ViewLists
	fmt.Fprintf(os.Stdout, "Response from `ListsAPI.ViewLists`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiViewListsRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **contentType** | **string** |  | 

### Return type

[**ViewLists**](ViewLists.md)

### Authorization

[basicAuth](../README.md#basicAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## ViewSpecificList

> ViewSpecificList ViewSpecificList(ctx, listId).ContentType(contentType).Execute()

View Specific List



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
	listId := "listId_example" // string | 
	contentType := "application/json" // string |  (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.ListsAPI.ViewSpecificList(context.Background(), listId).ContentType(contentType).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `ListsAPI.ViewSpecificList``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ViewSpecificList`: ViewSpecificList
	fmt.Fprintf(os.Stdout, "Response from `ListsAPI.ViewSpecificList`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**listId** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiViewSpecificListRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **contentType** | **string** |  | 

### Return type

[**ViewSpecificList**](ViewSpecificList.md)

### Authorization

[basicAuth](../README.md#basicAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)

