# \FaxAPI

All URIs are relative to *https://rest.clicksend.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**CalculateFaxPrice**](FaxAPI.md#CalculateFaxPrice) | **Post** /v3/fax/price | Calculate Fax Price
[**CreateFaxDeliveryReceiptRule**](FaxAPI.md#CreateFaxDeliveryReceiptRule) | **Post** /v3/automations/fax/receipts | Create FAX Delivery Receipt Rule
[**CreateFaxInboundRule**](FaxAPI.md#CreateFaxInboundRule) | **Post** /v3/automations/fax/inbound | Create Fax Inbound Rule
[**DeleteFaxDeliveryReceiptRule**](FaxAPI.md#DeleteFaxDeliveryReceiptRule) | **Delete** /v3/automations/fax/receipts/{receipt_rule_id} | Delete FAX Delivery Receipt Rule
[**DeleteFaxInboundRule**](FaxAPI.md#DeleteFaxInboundRule) | **Delete** /v3/automations/fax/inbound/{inbound_rule_id} | Delete Fax Inbound Rule
[**SendFax**](FaxAPI.md#SendFax) | **Post** /v3/fax/send | Send Fax
[**UpdateFaxDeliveryReceiptRule**](FaxAPI.md#UpdateFaxDeliveryReceiptRule) | **Put** /v3/automations/fax/receipts/{receipt_rule_id} | Update FAX Delivery Receipt Rule
[**UpdateFaxInboundRule**](FaxAPI.md#UpdateFaxInboundRule) | **Put** /v3/automations/fax/inbound/{inbound_rule_id} | Update Fax Inbound Rule
[**ViewFaxDeliveryReceiptRule**](FaxAPI.md#ViewFaxDeliveryReceiptRule) | **Get** /v3/automations/fax/receipts/{receipt_rule_id} | View FAX Delivery Receipt Rule
[**ViewFaxDeliveryReceiptRules**](FaxAPI.md#ViewFaxDeliveryReceiptRules) | **Get** /v3/automations/fax/receipts | View FAX Delivery Receipt Rules
[**ViewFaxHistory**](FaxAPI.md#ViewFaxHistory) | **Get** /v3/fax/history | View Fax History
[**ViewFaxInboundRule**](FaxAPI.md#ViewFaxInboundRule) | **Get** /v3/automations/fax/inbound/{inbound_rule_id} | View Fax Inbound Rule
[**ViewFaxInboundRules**](FaxAPI.md#ViewFaxInboundRules) | **Get** /v3/automations/fax/inbound | View Fax Inbound Rules
[**ViewFaxReceipts**](FaxAPI.md#ViewFaxReceipts) | **Get** /v3/fax/receipts | View Fax Receipts
[**ViewSpecificFaxReceipt**](FaxAPI.md#ViewSpecificFaxReceipt) | **Get** /v3/fax/receipts/{message_id} | View Specific Fax Receipt



## CalculateFaxPrice

> CalculateFaxPrice CalculateFaxPrice(ctx).ContentType(contentType).CalculateFaxPriceRequest(calculateFaxPriceRequest).Execute()

Calculate Fax Price



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
	calculateFaxPriceRequest := *openapiclient.NewCalculateFaxPriceRequest() // CalculateFaxPriceRequest |  (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.FaxAPI.CalculateFaxPrice(context.Background()).ContentType(contentType).CalculateFaxPriceRequest(calculateFaxPriceRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `FaxAPI.CalculateFaxPrice``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `CalculateFaxPrice`: CalculateFaxPrice
	fmt.Fprintf(os.Stdout, "Response from `FaxAPI.CalculateFaxPrice`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiCalculateFaxPriceRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **contentType** | **string** |  | 
 **calculateFaxPriceRequest** | [**CalculateFaxPriceRequest**](CalculateFaxPriceRequest.md) |  | 

### Return type

[**CalculateFaxPrice**](CalculateFaxPrice.md)

### Authorization

[basicAuth](../README.md#basicAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## CreateFaxDeliveryReceiptRule

> CreateFaxDeliveryReceiptRule CreateFaxDeliveryReceiptRule(ctx).ContentType(contentType).CreateFaxDeliveryReceiptRuleRequest(createFaxDeliveryReceiptRuleRequest).Execute()

Create FAX Delivery Receipt Rule



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
	createFaxDeliveryReceiptRuleRequest := *openapiclient.NewCreateFaxDeliveryReceiptRuleRequest() // CreateFaxDeliveryReceiptRuleRequest |  (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.FaxAPI.CreateFaxDeliveryReceiptRule(context.Background()).ContentType(contentType).CreateFaxDeliveryReceiptRuleRequest(createFaxDeliveryReceiptRuleRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `FaxAPI.CreateFaxDeliveryReceiptRule``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `CreateFaxDeliveryReceiptRule`: CreateFaxDeliveryReceiptRule
	fmt.Fprintf(os.Stdout, "Response from `FaxAPI.CreateFaxDeliveryReceiptRule`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiCreateFaxDeliveryReceiptRuleRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **contentType** | **string** |  | 
 **createFaxDeliveryReceiptRuleRequest** | [**CreateFaxDeliveryReceiptRuleRequest**](CreateFaxDeliveryReceiptRuleRequest.md) |  | 

### Return type

[**CreateFaxDeliveryReceiptRule**](CreateFaxDeliveryReceiptRule.md)

### Authorization

[basicAuth](../README.md#basicAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## CreateFaxInboundRule

> CreateFaxInboundRule CreateFaxInboundRule(ctx).ContentType(contentType).CreateFaxInboundRuleRequest(createFaxInboundRuleRequest).Execute()

Create Fax Inbound Rule



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
	createFaxInboundRuleRequest := *openapiclient.NewCreateFaxInboundRuleRequest() // CreateFaxInboundRuleRequest |  (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.FaxAPI.CreateFaxInboundRule(context.Background()).ContentType(contentType).CreateFaxInboundRuleRequest(createFaxInboundRuleRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `FaxAPI.CreateFaxInboundRule``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `CreateFaxInboundRule`: CreateFaxInboundRule
	fmt.Fprintf(os.Stdout, "Response from `FaxAPI.CreateFaxInboundRule`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiCreateFaxInboundRuleRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **contentType** | **string** |  | 
 **createFaxInboundRuleRequest** | [**CreateFaxInboundRuleRequest**](CreateFaxInboundRuleRequest.md) |  | 

### Return type

[**CreateFaxInboundRule**](CreateFaxInboundRule.md)

### Authorization

[basicAuth](../README.md#basicAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## DeleteFaxDeliveryReceiptRule

> DeleteFaxDeliveryReceiptRule DeleteFaxDeliveryReceiptRule(ctx, receiptRuleId).ContentType(contentType).Execute()

Delete FAX Delivery Receipt Rule



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
	receiptRuleId := "receiptRuleId_example" // string | 
	contentType := "application/json" // string |  (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.FaxAPI.DeleteFaxDeliveryReceiptRule(context.Background(), receiptRuleId).ContentType(contentType).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `FaxAPI.DeleteFaxDeliveryReceiptRule``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `DeleteFaxDeliveryReceiptRule`: DeleteFaxDeliveryReceiptRule
	fmt.Fprintf(os.Stdout, "Response from `FaxAPI.DeleteFaxDeliveryReceiptRule`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**receiptRuleId** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiDeleteFaxDeliveryReceiptRuleRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **contentType** | **string** |  | 

### Return type

[**DeleteFaxDeliveryReceiptRule**](DeleteFaxDeliveryReceiptRule.md)

### Authorization

[basicAuth](../README.md#basicAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## DeleteFaxInboundRule

> DeleteFaxInboundRule DeleteFaxInboundRule(ctx, inboundRuleId).ContentType(contentType).Execute()

Delete Fax Inbound Rule



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
	inboundRuleId := "inboundRuleId_example" // string | 
	contentType := "application/json" // string |  (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.FaxAPI.DeleteFaxInboundRule(context.Background(), inboundRuleId).ContentType(contentType).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `FaxAPI.DeleteFaxInboundRule``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `DeleteFaxInboundRule`: DeleteFaxInboundRule
	fmt.Fprintf(os.Stdout, "Response from `FaxAPI.DeleteFaxInboundRule`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**inboundRuleId** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiDeleteFaxInboundRuleRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **contentType** | **string** |  | 

### Return type

[**DeleteFaxInboundRule**](DeleteFaxInboundRule.md)

### Authorization

[basicAuth](../README.md#basicAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## SendFax

> SendFax SendFax(ctx).ContentType(contentType).SendFaxRequest(sendFaxRequest).Execute()

Send Fax



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
	sendFaxRequest := *openapiclient.NewSendFaxRequest() // SendFaxRequest |  (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.FaxAPI.SendFax(context.Background()).ContentType(contentType).SendFaxRequest(sendFaxRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `FaxAPI.SendFax``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `SendFax`: SendFax
	fmt.Fprintf(os.Stdout, "Response from `FaxAPI.SendFax`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiSendFaxRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **contentType** | **string** |  | 
 **sendFaxRequest** | [**SendFaxRequest**](SendFaxRequest.md) |  | 

### Return type

[**SendFax**](SendFax.md)

### Authorization

[basicAuth](../README.md#basicAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## UpdateFaxDeliveryReceiptRule

> UpdateFaxDeliveryReceiptRule UpdateFaxDeliveryReceiptRule(ctx, receiptRuleId).ContentType(contentType).UpdateFaxDeliveryReceiptRuleRequest(updateFaxDeliveryReceiptRuleRequest).Execute()

Update FAX Delivery Receipt Rule



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
	receiptRuleId := "receiptRuleId_example" // string | 
	contentType := "application/json" // string |  (optional)
	updateFaxDeliveryReceiptRuleRequest := *openapiclient.NewUpdateFaxDeliveryReceiptRuleRequest() // UpdateFaxDeliveryReceiptRuleRequest |  (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.FaxAPI.UpdateFaxDeliveryReceiptRule(context.Background(), receiptRuleId).ContentType(contentType).UpdateFaxDeliveryReceiptRuleRequest(updateFaxDeliveryReceiptRuleRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `FaxAPI.UpdateFaxDeliveryReceiptRule``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `UpdateFaxDeliveryReceiptRule`: UpdateFaxDeliveryReceiptRule
	fmt.Fprintf(os.Stdout, "Response from `FaxAPI.UpdateFaxDeliveryReceiptRule`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**receiptRuleId** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiUpdateFaxDeliveryReceiptRuleRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **contentType** | **string** |  | 
 **updateFaxDeliveryReceiptRuleRequest** | [**UpdateFaxDeliveryReceiptRuleRequest**](UpdateFaxDeliveryReceiptRuleRequest.md) |  | 

### Return type

[**UpdateFaxDeliveryReceiptRule**](UpdateFaxDeliveryReceiptRule.md)

### Authorization

[basicAuth](../README.md#basicAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## UpdateFaxInboundRule

> UpdateFaxInboundRule UpdateFaxInboundRule(ctx, inboundRuleId).ContentType(contentType).CreateFaxInboundRuleRequest(createFaxInboundRuleRequest).Execute()

Update Fax Inbound Rule



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
	inboundRuleId := "inboundRuleId_example" // string | 
	contentType := "application/json" // string |  (optional)
	createFaxInboundRuleRequest := *openapiclient.NewCreateFaxInboundRuleRequest() // CreateFaxInboundRuleRequest |  (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.FaxAPI.UpdateFaxInboundRule(context.Background(), inboundRuleId).ContentType(contentType).CreateFaxInboundRuleRequest(createFaxInboundRuleRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `FaxAPI.UpdateFaxInboundRule``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `UpdateFaxInboundRule`: UpdateFaxInboundRule
	fmt.Fprintf(os.Stdout, "Response from `FaxAPI.UpdateFaxInboundRule`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**inboundRuleId** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiUpdateFaxInboundRuleRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **contentType** | **string** |  | 
 **createFaxInboundRuleRequest** | [**CreateFaxInboundRuleRequest**](CreateFaxInboundRuleRequest.md) |  | 

### Return type

[**UpdateFaxInboundRule**](UpdateFaxInboundRule.md)

### Authorization

[basicAuth](../README.md#basicAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## ViewFaxDeliveryReceiptRule

> ViewFaxDeliveryReceiptRule ViewFaxDeliveryReceiptRule(ctx, receiptRuleId).ContentType(contentType).Execute()

View FAX Delivery Receipt Rule



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
	receiptRuleId := "receiptRuleId_example" // string | 
	contentType := "application/json" // string |  (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.FaxAPI.ViewFaxDeliveryReceiptRule(context.Background(), receiptRuleId).ContentType(contentType).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `FaxAPI.ViewFaxDeliveryReceiptRule``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ViewFaxDeliveryReceiptRule`: ViewFaxDeliveryReceiptRule
	fmt.Fprintf(os.Stdout, "Response from `FaxAPI.ViewFaxDeliveryReceiptRule`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**receiptRuleId** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiViewFaxDeliveryReceiptRuleRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **contentType** | **string** |  | 

### Return type

[**ViewFaxDeliveryReceiptRule**](ViewFaxDeliveryReceiptRule.md)

### Authorization

[basicAuth](../README.md#basicAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## ViewFaxDeliveryReceiptRules

> ViewFaxDeliveryReceiptRules ViewFaxDeliveryReceiptRules(ctx).ContentType(contentType).Execute()

View FAX Delivery Receipt Rules



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
	resp, r, err := apiClient.FaxAPI.ViewFaxDeliveryReceiptRules(context.Background()).ContentType(contentType).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `FaxAPI.ViewFaxDeliveryReceiptRules``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ViewFaxDeliveryReceiptRules`: ViewFaxDeliveryReceiptRules
	fmt.Fprintf(os.Stdout, "Response from `FaxAPI.ViewFaxDeliveryReceiptRules`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiViewFaxDeliveryReceiptRulesRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **contentType** | **string** |  | 

### Return type

[**ViewFaxDeliveryReceiptRules**](ViewFaxDeliveryReceiptRules.md)

### Authorization

[basicAuth](../README.md#basicAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## ViewFaxHistory

> ViewFaxHistory ViewFaxHistory(ctx).ContentType(contentType).Execute()

View Fax History



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
	resp, r, err := apiClient.FaxAPI.ViewFaxHistory(context.Background()).ContentType(contentType).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `FaxAPI.ViewFaxHistory``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ViewFaxHistory`: ViewFaxHistory
	fmt.Fprintf(os.Stdout, "Response from `FaxAPI.ViewFaxHistory`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiViewFaxHistoryRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **contentType** | **string** |  | 

### Return type

[**ViewFaxHistory**](ViewFaxHistory.md)

### Authorization

[basicAuth](../README.md#basicAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## ViewFaxInboundRule

> ViewFaxInboundRule ViewFaxInboundRule(ctx, inboundRuleId).ContentType(contentType).Execute()

View Fax Inbound Rule



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
	inboundRuleId := "inboundRuleId_example" // string | 
	contentType := "application/json" // string |  (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.FaxAPI.ViewFaxInboundRule(context.Background(), inboundRuleId).ContentType(contentType).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `FaxAPI.ViewFaxInboundRule``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ViewFaxInboundRule`: ViewFaxInboundRule
	fmt.Fprintf(os.Stdout, "Response from `FaxAPI.ViewFaxInboundRule`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**inboundRuleId** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiViewFaxInboundRuleRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **contentType** | **string** |  | 

### Return type

[**ViewFaxInboundRule**](ViewFaxInboundRule.md)

### Authorization

[basicAuth](../README.md#basicAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## ViewFaxInboundRules

> ViewFaxInboundRules ViewFaxInboundRules(ctx).ContentType(contentType).Execute()

View Fax Inbound Rules



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
	resp, r, err := apiClient.FaxAPI.ViewFaxInboundRules(context.Background()).ContentType(contentType).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `FaxAPI.ViewFaxInboundRules``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ViewFaxInboundRules`: ViewFaxInboundRules
	fmt.Fprintf(os.Stdout, "Response from `FaxAPI.ViewFaxInboundRules`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiViewFaxInboundRulesRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **contentType** | **string** |  | 

### Return type

[**ViewFaxInboundRules**](ViewFaxInboundRules.md)

### Authorization

[basicAuth](../README.md#basicAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## ViewFaxReceipts

> ViewFaxReceipts ViewFaxReceipts(ctx).ContentType(contentType).Execute()

View Fax Receipts



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
	resp, r, err := apiClient.FaxAPI.ViewFaxReceipts(context.Background()).ContentType(contentType).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `FaxAPI.ViewFaxReceipts``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ViewFaxReceipts`: ViewFaxReceipts
	fmt.Fprintf(os.Stdout, "Response from `FaxAPI.ViewFaxReceipts`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiViewFaxReceiptsRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **contentType** | **string** |  | 

### Return type

[**ViewFaxReceipts**](ViewFaxReceipts.md)

### Authorization

[basicAuth](../README.md#basicAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## ViewSpecificFaxReceipt

> ViewSpecificFaxReceipt ViewSpecificFaxReceipt(ctx, messageId).ContentType(contentType).Execute()

View Specific Fax Receipt



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
	messageId := "messageId_example" // string | 
	contentType := "application/json" // string |  (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.FaxAPI.ViewSpecificFaxReceipt(context.Background(), messageId).ContentType(contentType).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `FaxAPI.ViewSpecificFaxReceipt``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ViewSpecificFaxReceipt`: ViewSpecificFaxReceipt
	fmt.Fprintf(os.Stdout, "Response from `FaxAPI.ViewSpecificFaxReceipt`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**messageId** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiViewSpecificFaxReceiptRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **contentType** | **string** |  | 

### Return type

[**ViewSpecificFaxReceipt**](ViewSpecificFaxReceipt.md)

### Authorization

[basicAuth](../README.md#basicAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)

