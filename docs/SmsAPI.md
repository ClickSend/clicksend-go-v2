# \SmsAPI

All URIs are relative to *https://rest.clicksend.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**CalculateSmsPrice**](SmsAPI.md#CalculateSmsPrice) | **Post** /v3/sms/price | Calculate SMS Price
[**CancelAllSms**](SmsAPI.md#CancelAllSms) | **Put** /v3/sms/cancel-all | Cancel All SMS
[**CancelSms**](SmsAPI.md#CancelSms) | **Put** /v3/sms/{message_id}/cancel | Cancel SMS
[**CreateSmsDeliveryReceiptRule**](SmsAPI.md#CreateSmsDeliveryReceiptRule) | **Post** /v3/automations/sms/receipts | Create SMS Delivery Receipt Rule
[**CreateSmsInboundAutomation**](SmsAPI.md#CreateSmsInboundAutomation) | **Post** /v3/automations/sms/inbound | Create SMS Inbound Automation
[**CreateSmsTemplate**](SmsAPI.md#CreateSmsTemplate) | **Post** /v3/sms/templates | Create SMS Template
[**CreateTestInboundSms**](SmsAPI.md#CreateTestInboundSms) | **Post** /v3/sms/inbound | Create Test Inbound SMS
[**CreateTestSmsReceipt**](SmsAPI.md#CreateTestSmsReceipt) | **Post** /v3/sms/receipts | Create Test SMS Receipt
[**DeleteSmsDeliveryReceiptRule**](SmsAPI.md#DeleteSmsDeliveryReceiptRule) | **Delete** /v3/automations/sms/receipts/{receipt_rule_id} | Delete SMS Delivery Receipt Rule
[**DeleteSmsInboundAutomation**](SmsAPI.md#DeleteSmsInboundAutomation) | **Delete** /v3/automations/sms/inbound/{inbound_rule_id} | Delete SMS Inbound Automation
[**DeleteSmsTemplate**](SmsAPI.md#DeleteSmsTemplate) | **Delete** /v3/sms/templates/{template_id} | Delete SMS Template
[**ExportSmsHistory**](SmsAPI.md#ExportSmsHistory) | **Get** /v3/sms/history/export | Export SMS History
[**MarkInboundSmsAsRead**](SmsAPI.md#MarkInboundSmsAsRead) | **Put** /v3/sms/inbound-read | Mark Inbound SMS as Read
[**MarkSmsReceiptAsRead**](SmsAPI.md#MarkSmsReceiptAsRead) | **Put** /v3/sms/receipts-read | Mark SMS Receipt As Read
[**MarkSpecificInboundSmsMessageAsRead**](SmsAPI.md#MarkSpecificInboundSmsMessageAsRead) | **Put** /v3/sms/inbound-read/{message_id} | Mark Specific Inbound SMS Message As Read
[**SendSms**](SmsAPI.md#SendSms) | **Post** /v3/sms/send | Send SMS
[**UpdateSmsDeliveryReceiptRule**](SmsAPI.md#UpdateSmsDeliveryReceiptRule) | **Put** /v3/automations/sms/receipts/{receipt_rule_id} | Update SMS Delivery Receipt Rule
[**UpdateSmsInboundAutomation**](SmsAPI.md#UpdateSmsInboundAutomation) | **Put** /v3/automations/sms/inbound/{inbound_rule_id} | Update SMS Inbound Automation
[**UpdateSmsTemplate**](SmsAPI.md#UpdateSmsTemplate) | **Put** /v3/sms/templates/{template_id} | Update SMS Template
[**ViewASpecificInboundSmsMessage**](SmsAPI.md#ViewASpecificInboundSmsMessage) | **Get** /v3/sms/inbound/{original_message_id} | View a specific inbound SMS message
[**ViewASpecificSmsTemplate**](SmsAPI.md#ViewASpecificSmsTemplate) | **Get** /v3/sms/templates/{template_id} | View a Specific SMS Template
[**ViewInboundSms**](SmsAPI.md#ViewInboundSms) | **Get** /v3/sms/inbound | View Inbound SMS
[**ViewSmsDeliveryReceiptRule**](SmsAPI.md#ViewSmsDeliveryReceiptRule) | **Get** /v3/automations/sms/receipts/{receipt_rule_id} | View SMS Delivery Receipt Rule
[**ViewSmsDeliveryReceiptRules**](SmsAPI.md#ViewSmsDeliveryReceiptRules) | **Get** /v3/automations/sms/receipts | View SMS Delivery Receipt Rules
[**ViewSmsHistory**](SmsAPI.md#ViewSmsHistory) | **Get** /v3/sms/history | View SMS History
[**ViewSmsInboundAutomation**](SmsAPI.md#ViewSmsInboundAutomation) | **Get** /v3/automations/sms/inbound/{inbound_rule_id} | View SMS Inbound Automation
[**ViewSmsInboundAutomations**](SmsAPI.md#ViewSmsInboundAutomations) | **Get** /v3/automations/sms/inbound | View SMS Inbound Automations
[**ViewSmsReceipts**](SmsAPI.md#ViewSmsReceipts) | **Get** /v3/sms/receipts | View SMS Receipts
[**ViewSmsTemplates**](SmsAPI.md#ViewSmsTemplates) | **Get** /v3/sms/templates | View SMS Templates
[**ViewSpecificSmsReceipt**](SmsAPI.md#ViewSpecificSmsReceipt) | **Get** /v3/sms/receipts/{message_id} | View Specific SMS Receipt



## CalculateSmsPrice

> CalculateSmsPrice CalculateSmsPrice(ctx).ContentType(contentType).CalculateSmsPriceRequest(calculateSmsPriceRequest).Execute()

Calculate SMS Price



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
	calculateSmsPriceRequest := *openapiclient.NewCalculateSmsPriceRequest() // CalculateSmsPriceRequest |  (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.SmsAPI.CalculateSmsPrice(context.Background()).ContentType(contentType).CalculateSmsPriceRequest(calculateSmsPriceRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `SmsAPI.CalculateSmsPrice``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `CalculateSmsPrice`: CalculateSmsPrice
	fmt.Fprintf(os.Stdout, "Response from `SmsAPI.CalculateSmsPrice`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiCalculateSmsPriceRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **contentType** | **string** |  | 
 **calculateSmsPriceRequest** | [**CalculateSmsPriceRequest**](CalculateSmsPriceRequest.md) |  | 

### Return type

[**CalculateSmsPrice**](CalculateSmsPrice.md)

### Authorization

[basicAuth](../README.md#basicAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## CancelAllSms

> CancelAllSms CancelAllSms(ctx).ContentType(contentType).CancelAllSmsRequest(cancelAllSmsRequest).Execute()

Cancel All SMS



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
	cancelAllSmsRequest := *openapiclient.NewCancelAllSmsRequest() // CancelAllSmsRequest |  (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.SmsAPI.CancelAllSms(context.Background()).ContentType(contentType).CancelAllSmsRequest(cancelAllSmsRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `SmsAPI.CancelAllSms``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `CancelAllSms`: CancelAllSms
	fmt.Fprintf(os.Stdout, "Response from `SmsAPI.CancelAllSms`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiCancelAllSmsRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **contentType** | **string** |  | 
 **cancelAllSmsRequest** | [**CancelAllSmsRequest**](CancelAllSmsRequest.md) |  | 

### Return type

[**CancelAllSms**](CancelAllSms.md)

### Authorization

[basicAuth](../README.md#basicAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## CancelSms

> CancelSms CancelSms(ctx, messageId).ContentType(contentType).Execute()

Cancel SMS



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
	messageId := "messageId_example" // string | The _message_id_ of the scheduled SMS to cancel.
	contentType := "application/json" // string |  (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.SmsAPI.CancelSms(context.Background(), messageId).ContentType(contentType).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `SmsAPI.CancelSms``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `CancelSms`: CancelSms
	fmt.Fprintf(os.Stdout, "Response from `SmsAPI.CancelSms`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**messageId** | **string** | The _message_id_ of the scheduled SMS to cancel. | 

### Other Parameters

Other parameters are passed through a pointer to a apiCancelSmsRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **contentType** | **string** |  | 

### Return type

[**CancelSms**](CancelSms.md)

### Authorization

[basicAuth](../README.md#basicAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## CreateSmsDeliveryReceiptRule

> CreateSmsDeliveryReceiptRule CreateSmsDeliveryReceiptRule(ctx).ContentType(contentType).CreateSmsDeliveryReceiptRuleRequest(createSmsDeliveryReceiptRuleRequest).Execute()

Create SMS Delivery Receipt Rule



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
	createSmsDeliveryReceiptRuleRequest := *openapiclient.NewCreateSmsDeliveryReceiptRuleRequest() // CreateSmsDeliveryReceiptRuleRequest |  (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.SmsAPI.CreateSmsDeliveryReceiptRule(context.Background()).ContentType(contentType).CreateSmsDeliveryReceiptRuleRequest(createSmsDeliveryReceiptRuleRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `SmsAPI.CreateSmsDeliveryReceiptRule``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `CreateSmsDeliveryReceiptRule`: CreateSmsDeliveryReceiptRule
	fmt.Fprintf(os.Stdout, "Response from `SmsAPI.CreateSmsDeliveryReceiptRule`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiCreateSmsDeliveryReceiptRuleRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **contentType** | **string** |  | 
 **createSmsDeliveryReceiptRuleRequest** | [**CreateSmsDeliveryReceiptRuleRequest**](CreateSmsDeliveryReceiptRuleRequest.md) |  | 

### Return type

[**CreateSmsDeliveryReceiptRule**](CreateSmsDeliveryReceiptRule.md)

### Authorization

[basicAuth](../README.md#basicAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## CreateSmsInboundAutomation

> CreateSmsInboundAutomation CreateSmsInboundAutomation(ctx).ContentType(contentType).CreateSmsInboundAutomationRequest(createSmsInboundAutomationRequest).Execute()

Create SMS Inbound Automation



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
	createSmsInboundAutomationRequest := *openapiclient.NewCreateSmsInboundAutomationRequest() // CreateSmsInboundAutomationRequest |  (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.SmsAPI.CreateSmsInboundAutomation(context.Background()).ContentType(contentType).CreateSmsInboundAutomationRequest(createSmsInboundAutomationRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `SmsAPI.CreateSmsInboundAutomation``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `CreateSmsInboundAutomation`: CreateSmsInboundAutomation
	fmt.Fprintf(os.Stdout, "Response from `SmsAPI.CreateSmsInboundAutomation`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiCreateSmsInboundAutomationRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **contentType** | **string** |  | 
 **createSmsInboundAutomationRequest** | [**CreateSmsInboundAutomationRequest**](CreateSmsInboundAutomationRequest.md) |  | 

### Return type

[**CreateSmsInboundAutomation**](CreateSmsInboundAutomation.md)

### Authorization

[basicAuth](../README.md#basicAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## CreateSmsTemplate

> CreateSmsTemplate CreateSmsTemplate(ctx).ContentType(contentType).CreateSmsTemplateRequest(createSmsTemplateRequest).Execute()

Create SMS Template



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
	createSmsTemplateRequest := *openapiclient.NewCreateSmsTemplateRequest() // CreateSmsTemplateRequest |  (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.SmsAPI.CreateSmsTemplate(context.Background()).ContentType(contentType).CreateSmsTemplateRequest(createSmsTemplateRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `SmsAPI.CreateSmsTemplate``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `CreateSmsTemplate`: CreateSmsTemplate
	fmt.Fprintf(os.Stdout, "Response from `SmsAPI.CreateSmsTemplate`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiCreateSmsTemplateRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **contentType** | **string** |  | 
 **createSmsTemplateRequest** | [**CreateSmsTemplateRequest**](CreateSmsTemplateRequest.md) |  | 

### Return type

[**CreateSmsTemplate**](CreateSmsTemplate.md)

### Authorization

[basicAuth](../README.md#basicAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## CreateTestInboundSms

> CreateTestInboundSms CreateTestInboundSms(ctx).ContentType(contentType).CreateTestInboundSmsRequest(createTestInboundSmsRequest).Execute()

Create Test Inbound SMS



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
	createTestInboundSmsRequest := *openapiclient.NewCreateTestInboundSmsRequest("Url_example") // CreateTestInboundSmsRequest |  (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.SmsAPI.CreateTestInboundSms(context.Background()).ContentType(contentType).CreateTestInboundSmsRequest(createTestInboundSmsRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `SmsAPI.CreateTestInboundSms``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `CreateTestInboundSms`: CreateTestInboundSms
	fmt.Fprintf(os.Stdout, "Response from `SmsAPI.CreateTestInboundSms`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiCreateTestInboundSmsRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **contentType** | **string** |  | 
 **createTestInboundSmsRequest** | [**CreateTestInboundSmsRequest**](CreateTestInboundSmsRequest.md) |  | 

### Return type

[**CreateTestInboundSms**](CreateTestInboundSms.md)

### Authorization

[basicAuth](../README.md#basicAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## CreateTestSmsReceipt

> CreateTestSmsReceipt CreateTestSmsReceipt(ctx).ContentType(contentType).CreateTestSmsReceiptRequest(createTestSmsReceiptRequest).Execute()

Create Test SMS Receipt



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
	createTestSmsReceiptRequest := *openapiclient.NewCreateTestSmsReceiptRequest("Url_example") // CreateTestSmsReceiptRequest |  (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.SmsAPI.CreateTestSmsReceipt(context.Background()).ContentType(contentType).CreateTestSmsReceiptRequest(createTestSmsReceiptRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `SmsAPI.CreateTestSmsReceipt``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `CreateTestSmsReceipt`: CreateTestSmsReceipt
	fmt.Fprintf(os.Stdout, "Response from `SmsAPI.CreateTestSmsReceipt`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiCreateTestSmsReceiptRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **contentType** | **string** |  | 
 **createTestSmsReceiptRequest** | [**CreateTestSmsReceiptRequest**](CreateTestSmsReceiptRequest.md) |  | 

### Return type

[**CreateTestSmsReceipt**](CreateTestSmsReceipt.md)

### Authorization

[basicAuth](../README.md#basicAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## DeleteSmsDeliveryReceiptRule

> DeleteSmsDeliveryReceiptRule DeleteSmsDeliveryReceiptRule(ctx, receiptRuleId).ContentType(contentType).Execute()

Delete SMS Delivery Receipt Rule



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
	resp, r, err := apiClient.SmsAPI.DeleteSmsDeliveryReceiptRule(context.Background(), receiptRuleId).ContentType(contentType).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `SmsAPI.DeleteSmsDeliveryReceiptRule``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `DeleteSmsDeliveryReceiptRule`: DeleteSmsDeliveryReceiptRule
	fmt.Fprintf(os.Stdout, "Response from `SmsAPI.DeleteSmsDeliveryReceiptRule`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**receiptRuleId** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiDeleteSmsDeliveryReceiptRuleRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **contentType** | **string** |  | 

### Return type

[**DeleteSmsDeliveryReceiptRule**](DeleteSmsDeliveryReceiptRule.md)

### Authorization

[basicAuth](../README.md#basicAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## DeleteSmsInboundAutomation

> DeleteSmsInboundAutomation DeleteSmsInboundAutomation(ctx, inboundRuleId).ContentType(contentType).Execute()

Delete SMS Inbound Automation



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
	resp, r, err := apiClient.SmsAPI.DeleteSmsInboundAutomation(context.Background(), inboundRuleId).ContentType(contentType).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `SmsAPI.DeleteSmsInboundAutomation``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `DeleteSmsInboundAutomation`: DeleteSmsInboundAutomation
	fmt.Fprintf(os.Stdout, "Response from `SmsAPI.DeleteSmsInboundAutomation`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**inboundRuleId** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiDeleteSmsInboundAutomationRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **contentType** | **string** |  | 

### Return type

[**DeleteSmsInboundAutomation**](DeleteSmsInboundAutomation.md)

### Authorization

[basicAuth](../README.md#basicAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## DeleteSmsTemplate

> DeleteSmsTemplate DeleteSmsTemplate(ctx, templateId).ContentType(contentType).Execute()

Delete SMS Template



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
	templateId := "templateId_example" // string | The ID of the template to delete.
	contentType := "application/json" // string |  (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.SmsAPI.DeleteSmsTemplate(context.Background(), templateId).ContentType(contentType).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `SmsAPI.DeleteSmsTemplate``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `DeleteSmsTemplate`: DeleteSmsTemplate
	fmt.Fprintf(os.Stdout, "Response from `SmsAPI.DeleteSmsTemplate`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**templateId** | **string** | The ID of the template to delete. | 

### Other Parameters

Other parameters are passed through a pointer to a apiDeleteSmsTemplateRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **contentType** | **string** |  | 

### Return type

[**DeleteSmsTemplate**](DeleteSmsTemplate.md)

### Authorization

[basicAuth](../README.md#basicAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## ExportSmsHistory

> ExportSmsHistory ExportSmsHistory(ctx).ContentType(contentType).Filename(filename).Page(page).Limit(limit).Q(q).OrderBy(orderBy).DateFrom(dateFrom).DateTo(dateTo).Execute()

Export SMS History



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
	filename := "filename_example" // string | The filename of the result. It should be in the .csv format. (optional) (default to "export.csv")
	page := int32(1) // int32 | The page number to retrieve. Use this parameter to navigate through the [pagination](/#pagination) results. The default value is 1. (optional) (default to 1)
	limit := int32(15) // int32 | The number of items to return per page. This parameter controls the size of each page of results. The default value is 15. (optional) (default to 15)
	q := "q_example" // string | Allows filtering of results based on your search criteria. The query should be in the format `field_name:value`.  1. **Field Name**: The field within the SMS history you want to filter by. You can use the following fields:          - _Status_: The status of the SMS. Available values for status are: Queued, Completed, Scheduled, WaitApproval, Failed, Cancelled, CancelledAfterReview, Received, Sent.              - _To_: The recipient of the SMS.              - _from_: The sender of the SMS.              - _subaccount_id_: The sub-account identifier.              - _message_id_: The ID of your SMS.          2. **Value**: The text or keyword you're searching for within the specified field. If left empty after the colon, the filter will look for all templates with any value in the **Field Name**.             For example, if you are searching for a SMS with the status of _Scheduled_, the final query would look like this:    `q=status:Scheduled`  <div class=\"info-box\">   <h4><i class=\"fas fa-info-circle\"></i> Note:</h4>   <div>   <p>Some characters have to be encoded. For example, if you are searching for SMS sent from the phone number +61437085284, your search query q would be:<br/></p>     <ul>       <li>q=from:%2B61437085284</li>     </ul>     <p>You can use the <a href=\"https://www.urlencoder.org/\" target=\"_blank\">URL encoder</a> to encode the text. If a character is not an alphanumeric character (A-Z, a-z, 0-9), it is typically either reserved or unsafe and should be encoded.</p>   </div> </div> (optional) (default to "field_name")
	orderBy := "orderBy_example" // string | Specifies the field and order to sort the results by. The value is composed of the field name followed by a colon and the sort direction (asc for ascending or desc for descending).  The default sort order is by date in ascending order. You can use the following fields:    - _date_    - _username_   - _from_    - _to_   - _status_    - _body_  For example, if you want to order by the most recently sent SMS, you should sort by date in descending order. The query would look like this:    `order_by=date:desc` (optional) (default to "date:asc")
	dateFrom := int32(56) // int32 | Start date to filter results. It should be in <a href=\"http://help.clicksend.com/what-is-a-unix-timestamp\" target=\"_blank\">Unix format</a>. (optional)
	dateTo := int32(56) // int32 | End date to filter results. It should be in <a href=\"http://help.clicksend.com/what-is-a-unix-timestamp\" target=\"_blank\">Unix format</a>. (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.SmsAPI.ExportSmsHistory(context.Background()).ContentType(contentType).Filename(filename).Page(page).Limit(limit).Q(q).OrderBy(orderBy).DateFrom(dateFrom).DateTo(dateTo).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `SmsAPI.ExportSmsHistory``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ExportSmsHistory`: ExportSmsHistory
	fmt.Fprintf(os.Stdout, "Response from `SmsAPI.ExportSmsHistory`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiExportSmsHistoryRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **contentType** | **string** |  | 
 **filename** | **string** | The filename of the result. It should be in the .csv format. | [default to &quot;export.csv&quot;]
 **page** | **int32** | The page number to retrieve. Use this parameter to navigate through the [pagination](/#pagination) results. The default value is 1. | [default to 1]
 **limit** | **int32** | The number of items to return per page. This parameter controls the size of each page of results. The default value is 15. | [default to 15]
 **q** | **string** | Allows filtering of results based on your search criteria. The query should be in the format &#x60;field_name:value&#x60;.  1. **Field Name**: The field within the SMS history you want to filter by. You can use the following fields:          - _Status_: The status of the SMS. Available values for status are: Queued, Completed, Scheduled, WaitApproval, Failed, Cancelled, CancelledAfterReview, Received, Sent.              - _To_: The recipient of the SMS.              - _from_: The sender of the SMS.              - _subaccount_id_: The sub-account identifier.              - _message_id_: The ID of your SMS.          2. **Value**: The text or keyword you&#39;re searching for within the specified field. If left empty after the colon, the filter will look for all templates with any value in the **Field Name**.             For example, if you are searching for a SMS with the status of _Scheduled_, the final query would look like this:    &#x60;q&#x3D;status:Scheduled&#x60;  &lt;div class&#x3D;\&quot;info-box\&quot;&gt;   &lt;h4&gt;&lt;i class&#x3D;\&quot;fas fa-info-circle\&quot;&gt;&lt;/i&gt; Note:&lt;/h4&gt;   &lt;div&gt;   &lt;p&gt;Some characters have to be encoded. For example, if you are searching for SMS sent from the phone number +61437085284, your search query q would be:&lt;br/&gt;&lt;/p&gt;     &lt;ul&gt;       &lt;li&gt;q&#x3D;from:%2B61437085284&lt;/li&gt;     &lt;/ul&gt;     &lt;p&gt;You can use the &lt;a href&#x3D;\&quot;https://www.urlencoder.org/\&quot; target&#x3D;\&quot;_blank\&quot;&gt;URL encoder&lt;/a&gt; to encode the text. If a character is not an alphanumeric character (A-Z, a-z, 0-9), it is typically either reserved or unsafe and should be encoded.&lt;/p&gt;   &lt;/div&gt; &lt;/div&gt; | [default to &quot;field_name&quot;]
 **orderBy** | **string** | Specifies the field and order to sort the results by. The value is composed of the field name followed by a colon and the sort direction (asc for ascending or desc for descending).  The default sort order is by date in ascending order. You can use the following fields:    - _date_    - _username_   - _from_    - _to_   - _status_    - _body_  For example, if you want to order by the most recently sent SMS, you should sort by date in descending order. The query would look like this:    &#x60;order_by&#x3D;date:desc&#x60; | [default to &quot;date:asc&quot;]
 **dateFrom** | **int32** | Start date to filter results. It should be in &lt;a href&#x3D;\&quot;http://help.clicksend.com/what-is-a-unix-timestamp\&quot; target&#x3D;\&quot;_blank\&quot;&gt;Unix format&lt;/a&gt;. | 
 **dateTo** | **int32** | End date to filter results. It should be in &lt;a href&#x3D;\&quot;http://help.clicksend.com/what-is-a-unix-timestamp\&quot; target&#x3D;\&quot;_blank\&quot;&gt;Unix format&lt;/a&gt;. | 

### Return type

[**ExportSmsHistory**](ExportSmsHistory.md)

### Authorization

[basicAuth](../README.md#basicAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## MarkInboundSmsAsRead

> MarkInboundSmsAsRead MarkInboundSmsAsRead(ctx).ContentType(contentType).MarkSmsReceiptAsReadRequest(markSmsReceiptAsReadRequest).Execute()

Mark Inbound SMS as Read



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
	markSmsReceiptAsReadRequest := *openapiclient.NewMarkSmsReceiptAsReadRequest() // MarkSmsReceiptAsReadRequest |  (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.SmsAPI.MarkInboundSmsAsRead(context.Background()).ContentType(contentType).MarkSmsReceiptAsReadRequest(markSmsReceiptAsReadRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `SmsAPI.MarkInboundSmsAsRead``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `MarkInboundSmsAsRead`: MarkInboundSmsAsRead
	fmt.Fprintf(os.Stdout, "Response from `SmsAPI.MarkInboundSmsAsRead`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiMarkInboundSmsAsReadRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **contentType** | **string** |  | 
 **markSmsReceiptAsReadRequest** | [**MarkSmsReceiptAsReadRequest**](MarkSmsReceiptAsReadRequest.md) |  | 

### Return type

[**MarkInboundSmsAsRead**](MarkInboundSmsAsRead.md)

### Authorization

[basicAuth](../README.md#basicAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## MarkSmsReceiptAsRead

> MarkSmsReceiptAsRead MarkSmsReceiptAsRead(ctx).ContentType(contentType).MarkSmsReceiptAsReadRequest(markSmsReceiptAsReadRequest).Execute()

Mark SMS Receipt As Read



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
	markSmsReceiptAsReadRequest := *openapiclient.NewMarkSmsReceiptAsReadRequest() // MarkSmsReceiptAsReadRequest |  (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.SmsAPI.MarkSmsReceiptAsRead(context.Background()).ContentType(contentType).MarkSmsReceiptAsReadRequest(markSmsReceiptAsReadRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `SmsAPI.MarkSmsReceiptAsRead``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `MarkSmsReceiptAsRead`: MarkSmsReceiptAsRead
	fmt.Fprintf(os.Stdout, "Response from `SmsAPI.MarkSmsReceiptAsRead`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiMarkSmsReceiptAsReadRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **contentType** | **string** |  | 
 **markSmsReceiptAsReadRequest** | [**MarkSmsReceiptAsReadRequest**](MarkSmsReceiptAsReadRequest.md) |  | 

### Return type

[**MarkSmsReceiptAsRead**](MarkSmsReceiptAsRead.md)

### Authorization

[basicAuth](../README.md#basicAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## MarkSpecificInboundSmsMessageAsRead

> MarkSpecificInboundSmsMessageAsRead MarkSpecificInboundSmsMessageAsRead(ctx, messageId).ContentType(contentType).Execute()

Mark Specific Inbound SMS Message As Read



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
	messageId := "messageId_example" // string | The message_id of the inbound SMS to mark as read.  <div class=\"info-box\">   <h4><i class=\"fas fa-info-circle\"></i> Note:</h4>   <p>     When you receive an inbound message, you will get two parameters: <em>original_message_id</em> and <em>message_id</em>:   </p>   <ul>     <li><em>original_message_id</em>: This is the ID of the outbound message sent to the recipient</li>     <li><em>message_id</em>: This is the ID of the inbound message sent by the recipient.</li>   </ul> </div>
	contentType := "application/json" // string |  (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.SmsAPI.MarkSpecificInboundSmsMessageAsRead(context.Background(), messageId).ContentType(contentType).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `SmsAPI.MarkSpecificInboundSmsMessageAsRead``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `MarkSpecificInboundSmsMessageAsRead`: MarkSpecificInboundSmsMessageAsRead
	fmt.Fprintf(os.Stdout, "Response from `SmsAPI.MarkSpecificInboundSmsMessageAsRead`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**messageId** | **string** | The message_id of the inbound SMS to mark as read.  &lt;div class&#x3D;\&quot;info-box\&quot;&gt;   &lt;h4&gt;&lt;i class&#x3D;\&quot;fas fa-info-circle\&quot;&gt;&lt;/i&gt; Note:&lt;/h4&gt;   &lt;p&gt;     When you receive an inbound message, you will get two parameters: &lt;em&gt;original_message_id&lt;/em&gt; and &lt;em&gt;message_id&lt;/em&gt;:   &lt;/p&gt;   &lt;ul&gt;     &lt;li&gt;&lt;em&gt;original_message_id&lt;/em&gt;: This is the ID of the outbound message sent to the recipient&lt;/li&gt;     &lt;li&gt;&lt;em&gt;message_id&lt;/em&gt;: This is the ID of the inbound message sent by the recipient.&lt;/li&gt;   &lt;/ul&gt; &lt;/div&gt; | 

### Other Parameters

Other parameters are passed through a pointer to a apiMarkSpecificInboundSmsMessageAsReadRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **contentType** | **string** |  | 

### Return type

[**MarkSpecificInboundSmsMessageAsRead**](MarkSpecificInboundSmsMessageAsRead.md)

### Authorization

[basicAuth](../README.md#basicAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## SendSms

> SendSms SendSms(ctx).ContentType(contentType).SendSmsRequest(sendSmsRequest).Execute()

Send SMS



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
	sendSmsRequest := *openapiclient.NewSendSmsRequest() // SendSmsRequest |  (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.SmsAPI.SendSms(context.Background()).ContentType(contentType).SendSmsRequest(sendSmsRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `SmsAPI.SendSms``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `SendSms`: SendSms
	fmt.Fprintf(os.Stdout, "Response from `SmsAPI.SendSms`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiSendSmsRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **contentType** | **string** |  | 
 **sendSmsRequest** | [**SendSmsRequest**](SendSmsRequest.md) |  | 

### Return type

[**SendSms**](SendSms.md)

### Authorization

[basicAuth](../README.md#basicAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## UpdateSmsDeliveryReceiptRule

> UpdateSmsDeliveryReceiptRule UpdateSmsDeliveryReceiptRule(ctx, receiptRuleId).ContentType(contentType).CreateSmsDeliveryReceiptRuleRequest(createSmsDeliveryReceiptRuleRequest).Execute()

Update SMS Delivery Receipt Rule



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
	createSmsDeliveryReceiptRuleRequest := *openapiclient.NewCreateSmsDeliveryReceiptRuleRequest() // CreateSmsDeliveryReceiptRuleRequest |  (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.SmsAPI.UpdateSmsDeliveryReceiptRule(context.Background(), receiptRuleId).ContentType(contentType).CreateSmsDeliveryReceiptRuleRequest(createSmsDeliveryReceiptRuleRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `SmsAPI.UpdateSmsDeliveryReceiptRule``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `UpdateSmsDeliveryReceiptRule`: UpdateSmsDeliveryReceiptRule
	fmt.Fprintf(os.Stdout, "Response from `SmsAPI.UpdateSmsDeliveryReceiptRule`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**receiptRuleId** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiUpdateSmsDeliveryReceiptRuleRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **contentType** | **string** |  | 
 **createSmsDeliveryReceiptRuleRequest** | [**CreateSmsDeliveryReceiptRuleRequest**](CreateSmsDeliveryReceiptRuleRequest.md) |  | 

### Return type

[**UpdateSmsDeliveryReceiptRule**](UpdateSmsDeliveryReceiptRule.md)

### Authorization

[basicAuth](../README.md#basicAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## UpdateSmsInboundAutomation

> UpdateSmsInboundAutomation UpdateSmsInboundAutomation(ctx, inboundRuleId).ContentType(contentType).UpdateSmsInboundAutomationRequest(updateSmsInboundAutomationRequest).Execute()

Update SMS Inbound Automation



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
	updateSmsInboundAutomationRequest := *openapiclient.NewUpdateSmsInboundAutomationRequest() // UpdateSmsInboundAutomationRequest |  (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.SmsAPI.UpdateSmsInboundAutomation(context.Background(), inboundRuleId).ContentType(contentType).UpdateSmsInboundAutomationRequest(updateSmsInboundAutomationRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `SmsAPI.UpdateSmsInboundAutomation``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `UpdateSmsInboundAutomation`: UpdateSmsInboundAutomation
	fmt.Fprintf(os.Stdout, "Response from `SmsAPI.UpdateSmsInboundAutomation`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**inboundRuleId** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiUpdateSmsInboundAutomationRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **contentType** | **string** |  | 
 **updateSmsInboundAutomationRequest** | [**UpdateSmsInboundAutomationRequest**](UpdateSmsInboundAutomationRequest.md) |  | 

### Return type

[**UpdateSmsInboundAutomation**](UpdateSmsInboundAutomation.md)

### Authorization

[basicAuth](../README.md#basicAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## UpdateSmsTemplate

> UpdateSmsTemplate UpdateSmsTemplate(ctx, templateId).ContentType(contentType).CreateSmsTemplateRequest(createSmsTemplateRequest).Execute()

Update SMS Template



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
	templateId := "templateId_example" // string | The ID of the template to update.
	contentType := "application/json" // string |  (optional)
	createSmsTemplateRequest := *openapiclient.NewCreateSmsTemplateRequest() // CreateSmsTemplateRequest |  (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.SmsAPI.UpdateSmsTemplate(context.Background(), templateId).ContentType(contentType).CreateSmsTemplateRequest(createSmsTemplateRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `SmsAPI.UpdateSmsTemplate``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `UpdateSmsTemplate`: UpdateSmsTemplate
	fmt.Fprintf(os.Stdout, "Response from `SmsAPI.UpdateSmsTemplate`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**templateId** | **string** | The ID of the template to update. | 

### Other Parameters

Other parameters are passed through a pointer to a apiUpdateSmsTemplateRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **contentType** | **string** |  | 
 **createSmsTemplateRequest** | [**CreateSmsTemplateRequest**](CreateSmsTemplateRequest.md) |  | 

### Return type

[**UpdateSmsTemplate**](UpdateSmsTemplate.md)

### Authorization

[basicAuth](../README.md#basicAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## ViewASpecificInboundSmsMessage

> ViewASpecificInboundSmsMessage ViewASpecificInboundSmsMessage(ctx, originalMessageId).ContentType(contentType).Execute()

View a specific inbound SMS message



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
	originalMessageId := "originalMessageId_example" // string | The _original_message_id_ of the inbound SMS to view. If the recipient replied with multiple messages, this endpoint returns the first inbound SMS received.  <div class=\"info-box\">   <h4><i class=\"fas fa-info-circle\"></i> Note:</h4>   <p>     When you receive an inbound message, you will get two parameters: <em>original_message_id</em> and <em>message_id</em>:   </p>   <ul>     <li><em>original_message_id</em>: This is the ID of the outbound message sent to the recipient</li>     <li><em>message_id</em>: This is the ID of the inbound message sent by the recipient.</li>   </ul> </div>
	contentType := "application/json" // string |  (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.SmsAPI.ViewASpecificInboundSmsMessage(context.Background(), originalMessageId).ContentType(contentType).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `SmsAPI.ViewASpecificInboundSmsMessage``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ViewASpecificInboundSmsMessage`: ViewASpecificInboundSmsMessage
	fmt.Fprintf(os.Stdout, "Response from `SmsAPI.ViewASpecificInboundSmsMessage`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**originalMessageId** | **string** | The _original_message_id_ of the inbound SMS to view. If the recipient replied with multiple messages, this endpoint returns the first inbound SMS received.  &lt;div class&#x3D;\&quot;info-box\&quot;&gt;   &lt;h4&gt;&lt;i class&#x3D;\&quot;fas fa-info-circle\&quot;&gt;&lt;/i&gt; Note:&lt;/h4&gt;   &lt;p&gt;     When you receive an inbound message, you will get two parameters: &lt;em&gt;original_message_id&lt;/em&gt; and &lt;em&gt;message_id&lt;/em&gt;:   &lt;/p&gt;   &lt;ul&gt;     &lt;li&gt;&lt;em&gt;original_message_id&lt;/em&gt;: This is the ID of the outbound message sent to the recipient&lt;/li&gt;     &lt;li&gt;&lt;em&gt;message_id&lt;/em&gt;: This is the ID of the inbound message sent by the recipient.&lt;/li&gt;   &lt;/ul&gt; &lt;/div&gt; | 

### Other Parameters

Other parameters are passed through a pointer to a apiViewASpecificInboundSmsMessageRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **contentType** | **string** |  | 

### Return type

[**ViewASpecificInboundSmsMessage**](ViewASpecificInboundSmsMessage.md)

### Authorization

[basicAuth](../README.md#basicAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## ViewASpecificSmsTemplate

> ViewASpecificSmsTemplate ViewASpecificSmsTemplate(ctx, templateId).ContentType(contentType).Execute()

View a Specific SMS Template



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
	templateId := "templateId_example" // string | The ID of the template to retrieve
	contentType := "application/json" // string |  (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.SmsAPI.ViewASpecificSmsTemplate(context.Background(), templateId).ContentType(contentType).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `SmsAPI.ViewASpecificSmsTemplate``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ViewASpecificSmsTemplate`: ViewASpecificSmsTemplate
	fmt.Fprintf(os.Stdout, "Response from `SmsAPI.ViewASpecificSmsTemplate`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**templateId** | **string** | The ID of the template to retrieve | 

### Other Parameters

Other parameters are passed through a pointer to a apiViewASpecificSmsTemplateRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **contentType** | **string** |  | 

### Return type

[**ViewASpecificSmsTemplate**](ViewASpecificSmsTemplate.md)

### Authorization

[basicAuth](../README.md#basicAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## ViewInboundSms

> ViewInboundSms ViewInboundSms(ctx).ContentType(contentType).Page(page).Limit(limit).Execute()

View Inbound SMS



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
	page := int32(1) // int32 | The page number to retrieve. Use this parameter to navigate through the [pagination](/#pagination) results. The default value is 1. (optional) (default to 1)
	limit := int32(15) // int32 | The number of items to return per page. This parameter controls the size of each page of results. The default value is 15. (optional) (default to 15)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.SmsAPI.ViewInboundSms(context.Background()).ContentType(contentType).Page(page).Limit(limit).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `SmsAPI.ViewInboundSms``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ViewInboundSms`: ViewInboundSms
	fmt.Fprintf(os.Stdout, "Response from `SmsAPI.ViewInboundSms`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiViewInboundSmsRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **contentType** | **string** |  | 
 **page** | **int32** | The page number to retrieve. Use this parameter to navigate through the [pagination](/#pagination) results. The default value is 1. | [default to 1]
 **limit** | **int32** | The number of items to return per page. This parameter controls the size of each page of results. The default value is 15. | [default to 15]

### Return type

[**ViewInboundSms**](ViewInboundSms.md)

### Authorization

[basicAuth](../README.md#basicAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## ViewSmsDeliveryReceiptRule

> ViewSmsDeliveryReceiptRule ViewSmsDeliveryReceiptRule(ctx, receiptRuleId).ContentType(contentType).Execute()

View SMS Delivery Receipt Rule



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
	resp, r, err := apiClient.SmsAPI.ViewSmsDeliveryReceiptRule(context.Background(), receiptRuleId).ContentType(contentType).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `SmsAPI.ViewSmsDeliveryReceiptRule``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ViewSmsDeliveryReceiptRule`: ViewSmsDeliveryReceiptRule
	fmt.Fprintf(os.Stdout, "Response from `SmsAPI.ViewSmsDeliveryReceiptRule`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**receiptRuleId** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiViewSmsDeliveryReceiptRuleRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **contentType** | **string** |  | 

### Return type

[**ViewSmsDeliveryReceiptRule**](ViewSmsDeliveryReceiptRule.md)

### Authorization

[basicAuth](../README.md#basicAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## ViewSmsDeliveryReceiptRules

> ViewSmsDeliveryReceiptRules ViewSmsDeliveryReceiptRules(ctx).ContentType(contentType).Execute()

View SMS Delivery Receipt Rules



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
	resp, r, err := apiClient.SmsAPI.ViewSmsDeliveryReceiptRules(context.Background()).ContentType(contentType).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `SmsAPI.ViewSmsDeliveryReceiptRules``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ViewSmsDeliveryReceiptRules`: ViewSmsDeliveryReceiptRules
	fmt.Fprintf(os.Stdout, "Response from `SmsAPI.ViewSmsDeliveryReceiptRules`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiViewSmsDeliveryReceiptRulesRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **contentType** | **string** |  | 

### Return type

[**ViewSmsDeliveryReceiptRules**](ViewSmsDeliveryReceiptRules.md)

### Authorization

[basicAuth](../README.md#basicAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## ViewSmsHistory

> ViewSmsHistory ViewSmsHistory(ctx).ContentType(contentType).Page(page).Limit(limit).Q(q).OrderBy(orderBy).DateFrom(dateFrom).DateTo(dateTo).Execute()

View SMS History



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
	page := int32(1) // int32 | The page number to retrieve. Use this parameter to navigate through the [pagination](/#pagination) results. The default value is 1. (optional) (default to 1)
	limit := int32(15) // int32 | The number of items to return per page. This parameter controls the size of each page of results. The default value is 15. (optional) (default to 15)
	q := "q_example" // string | Allows filtering of results based on your search criteria. The query should be in the format `field_name:value`.  1. **Field Name**: The field within the SMS history you want to filter by. You can use the following fields:          - _Status_: The status of the SMS. Available values for status are: Queued, Completed, Scheduled, WaitApproval, Failed, Cancelled, CancelledAfterReview, Received, Sent.              - _To_: The recipient of the SMS.              - _from_: The sender of the SMS.              - _subaccount_id_: The sub-account identifier.              - _message_id_: The ID of your SMS.          2. **Value**: The text or keyword you're searching for within the specified field. If left empty after the colon, the filter will look for all templates with any value in the **Field Name**.             For example, if you are searching for a SMS with the status of Scheduled, the final query would look like this:    `q=status:Scheduled`  <div class=\"info-box\">   <h4><i class=\"fas fa-info-circle\"></i> Note:</h4>   <div>    <p>Some characters have to be encoded. For example, if you are searching for SMS sent from the phone number +61437085284, your search query q would be:<br/></p>     <ul>       <li>q=from:%2B61437085284</li>     </ul>     <p>You can use the <a href=\"https://www.urlencoder.org/\" target=\"_blank\">URL encoder</a> to encode the text. If a character is not an alphanumeric character (A-Z, a-z, 0-9), it is typically either reserved or unsafe and should be encoded.</p>   </div> </div> (optional) (default to "field_name")
	orderBy := "orderBy_example" // string | Specifies the field and order to sort the results by. The value is composed of the field name followed by a colon and the sort direction (_asc_ for ascending or _desc_ for descending).  The default sort order is by _date_ in ascending order. You can use the following fields:    - _date_   - _username_   - _from_    - _to_   - _status_   - _body_  For example, if you want to order by the most recently sent SMS, you should sort by date in descending order. The query would look like this:    `order_by=date:desc` (optional) (default to "date:asc")
	dateFrom := int32(56) // int32 | Start date to filter results. It should be in <a href=\"http://help.clicksend.com/what-is-a-unix-timestamp\" target=\"_blank\">Unix format</a>. (optional)
	dateTo := int32(56) // int32 | End date to filter results. It should be in <a href=\"http://help.clicksend.com/what-is-a-unix-timestamp\" target=\"_blank\">Unix format</a>. (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.SmsAPI.ViewSmsHistory(context.Background()).ContentType(contentType).Page(page).Limit(limit).Q(q).OrderBy(orderBy).DateFrom(dateFrom).DateTo(dateTo).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `SmsAPI.ViewSmsHistory``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ViewSmsHistory`: ViewSmsHistory
	fmt.Fprintf(os.Stdout, "Response from `SmsAPI.ViewSmsHistory`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiViewSmsHistoryRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **contentType** | **string** |  | 
 **page** | **int32** | The page number to retrieve. Use this parameter to navigate through the [pagination](/#pagination) results. The default value is 1. | [default to 1]
 **limit** | **int32** | The number of items to return per page. This parameter controls the size of each page of results. The default value is 15. | [default to 15]
 **q** | **string** | Allows filtering of results based on your search criteria. The query should be in the format &#x60;field_name:value&#x60;.  1. **Field Name**: The field within the SMS history you want to filter by. You can use the following fields:          - _Status_: The status of the SMS. Available values for status are: Queued, Completed, Scheduled, WaitApproval, Failed, Cancelled, CancelledAfterReview, Received, Sent.              - _To_: The recipient of the SMS.              - _from_: The sender of the SMS.              - _subaccount_id_: The sub-account identifier.              - _message_id_: The ID of your SMS.          2. **Value**: The text or keyword you&#39;re searching for within the specified field. If left empty after the colon, the filter will look for all templates with any value in the **Field Name**.             For example, if you are searching for a SMS with the status of Scheduled, the final query would look like this:    &#x60;q&#x3D;status:Scheduled&#x60;  &lt;div class&#x3D;\&quot;info-box\&quot;&gt;   &lt;h4&gt;&lt;i class&#x3D;\&quot;fas fa-info-circle\&quot;&gt;&lt;/i&gt; Note:&lt;/h4&gt;   &lt;div&gt;    &lt;p&gt;Some characters have to be encoded. For example, if you are searching for SMS sent from the phone number +61437085284, your search query q would be:&lt;br/&gt;&lt;/p&gt;     &lt;ul&gt;       &lt;li&gt;q&#x3D;from:%2B61437085284&lt;/li&gt;     &lt;/ul&gt;     &lt;p&gt;You can use the &lt;a href&#x3D;\&quot;https://www.urlencoder.org/\&quot; target&#x3D;\&quot;_blank\&quot;&gt;URL encoder&lt;/a&gt; to encode the text. If a character is not an alphanumeric character (A-Z, a-z, 0-9), it is typically either reserved or unsafe and should be encoded.&lt;/p&gt;   &lt;/div&gt; &lt;/div&gt; | [default to &quot;field_name&quot;]
 **orderBy** | **string** | Specifies the field and order to sort the results by. The value is composed of the field name followed by a colon and the sort direction (_asc_ for ascending or _desc_ for descending).  The default sort order is by _date_ in ascending order. You can use the following fields:    - _date_   - _username_   - _from_    - _to_   - _status_   - _body_  For example, if you want to order by the most recently sent SMS, you should sort by date in descending order. The query would look like this:    &#x60;order_by&#x3D;date:desc&#x60; | [default to &quot;date:asc&quot;]
 **dateFrom** | **int32** | Start date to filter results. It should be in &lt;a href&#x3D;\&quot;http://help.clicksend.com/what-is-a-unix-timestamp\&quot; target&#x3D;\&quot;_blank\&quot;&gt;Unix format&lt;/a&gt;. | 
 **dateTo** | **int32** | End date to filter results. It should be in &lt;a href&#x3D;\&quot;http://help.clicksend.com/what-is-a-unix-timestamp\&quot; target&#x3D;\&quot;_blank\&quot;&gt;Unix format&lt;/a&gt;. | 

### Return type

[**ViewSmsHistory**](ViewSmsHistory.md)

### Authorization

[basicAuth](../README.md#basicAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## ViewSmsInboundAutomation

> ViewSmsInboundAutomation ViewSmsInboundAutomation(ctx, inboundRuleId).ContentType(contentType).Execute()

View SMS Inbound Automation



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
	resp, r, err := apiClient.SmsAPI.ViewSmsInboundAutomation(context.Background(), inboundRuleId).ContentType(contentType).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `SmsAPI.ViewSmsInboundAutomation``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ViewSmsInboundAutomation`: ViewSmsInboundAutomation
	fmt.Fprintf(os.Stdout, "Response from `SmsAPI.ViewSmsInboundAutomation`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**inboundRuleId** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiViewSmsInboundAutomationRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **contentType** | **string** |  | 

### Return type

[**ViewSmsInboundAutomation**](ViewSmsInboundAutomation.md)

### Authorization

[basicAuth](../README.md#basicAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## ViewSmsInboundAutomations

> ViewSmsInboundAutomations ViewSmsInboundAutomations(ctx).ContentType(contentType).Execute()

View SMS Inbound Automations



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
	resp, r, err := apiClient.SmsAPI.ViewSmsInboundAutomations(context.Background()).ContentType(contentType).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `SmsAPI.ViewSmsInboundAutomations``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ViewSmsInboundAutomations`: ViewSmsInboundAutomations
	fmt.Fprintf(os.Stdout, "Response from `SmsAPI.ViewSmsInboundAutomations`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiViewSmsInboundAutomationsRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **contentType** | **string** |  | 

### Return type

[**ViewSmsInboundAutomations**](ViewSmsInboundAutomations.md)

### Authorization

[basicAuth](../README.md#basicAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## ViewSmsReceipts

> ViewSmsReceipts ViewSmsReceipts(ctx).ContentType(contentType).Page(page).Limit(limit).Execute()

View SMS Receipts



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
	page := int32(1) // int32 | The page number to retrieve. Use this parameter to navigate through the [pagination](/#pagination) results. The default value is 1. (optional) (default to 1)
	limit := int32(15) // int32 | The number of items to return per page. This parameter controls the size of each page of results. The default value is 15. (optional) (default to 15)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.SmsAPI.ViewSmsReceipts(context.Background()).ContentType(contentType).Page(page).Limit(limit).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `SmsAPI.ViewSmsReceipts``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ViewSmsReceipts`: ViewSmsReceipts
	fmt.Fprintf(os.Stdout, "Response from `SmsAPI.ViewSmsReceipts`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiViewSmsReceiptsRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **contentType** | **string** |  | 
 **page** | **int32** | The page number to retrieve. Use this parameter to navigate through the [pagination](/#pagination) results. The default value is 1. | [default to 1]
 **limit** | **int32** | The number of items to return per page. This parameter controls the size of each page of results. The default value is 15. | [default to 15]

### Return type

[**ViewSmsReceipts**](ViewSmsReceipts.md)

### Authorization

[basicAuth](../README.md#basicAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## ViewSmsTemplates

> ViewSmsTemplates ViewSmsTemplates(ctx).ContentType(contentType).Page(page).Limit(limit).Q(q).OrderBy(orderBy).Execute()

View SMS Templates



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
	page := int32(1) // int32 | The page number to retrieve. Use this parameter to navigate through the [pagination](/#pagination) results. The default value is 1. (optional) (default to 1)
	limit := int32(15) // int32 | The number of items to return per page. This parameter controls the size of each page of results. The default value is 15. (optional) (default to 15)
	q := "q_example" // string | Allows filtering of results based on your search criteria. The query should be in the format `field_name:value`.  1. **Field Name**: The field within the SMS history you want to filter by. You can use the following fields:    - _template_id_ : The ID of the template   - _template_name_ : The name of the template   - _body_ : The body content of the template.          2. **Value**: The text or keyword you're searching for within the specified field. If left empty after the colon, the filter will look for all templates with any value in the **Field Name**.      For example, if you are searching for the template with the name of _sample_name_, the final query would look like this:     `q=template_name:sample_name`  <div class=\"info-box\">   <h4><i class=\"fas fa-info-circle\"></i> Note:</h4>   <div>    <p>Some characters have to be encoded. For example, if you are searching for SMS sent from the phone number +61437085284, your search query q would be:<br/></p>     <ul>       <li>q=from:%2B61437085284</li>     </ul>     <p>You can use the <a href=\"https://www.urlencoder.org/\" target=\"_blank\">URL encoder</a> to encode the text. If a character is not an alphanumeric character (A-Z, a-z, 0-9), it is typically either reserved or unsafe and should be encoded.</p>   </div> </div> (optional) (default to "field_name")
	orderBy := "orderBy_example" // string | Specifies the field and order to sort the results by.  The value is composed of the field name followed by a colon and the sort direction (_asc_ for ascending or _desc_ for descending).  The default sort order is by _template_id_ in ascending order. You can use the following fields:      - _template_id_ : The ID of the Template - _template_name_ : The name of the Template - _body_ : The body content of the Template  For example, if you want to order by the _template_id_ in descending order, the query would look like this:    `order_by=template_id:desc` (optional) (default to "template_id:asc")

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.SmsAPI.ViewSmsTemplates(context.Background()).ContentType(contentType).Page(page).Limit(limit).Q(q).OrderBy(orderBy).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `SmsAPI.ViewSmsTemplates``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ViewSmsTemplates`: ViewSmsTemplates
	fmt.Fprintf(os.Stdout, "Response from `SmsAPI.ViewSmsTemplates`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiViewSmsTemplatesRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **contentType** | **string** |  | 
 **page** | **int32** | The page number to retrieve. Use this parameter to navigate through the [pagination](/#pagination) results. The default value is 1. | [default to 1]
 **limit** | **int32** | The number of items to return per page. This parameter controls the size of each page of results. The default value is 15. | [default to 15]
 **q** | **string** | Allows filtering of results based on your search criteria. The query should be in the format &#x60;field_name:value&#x60;.  1. **Field Name**: The field within the SMS history you want to filter by. You can use the following fields:    - _template_id_ : The ID of the template   - _template_name_ : The name of the template   - _body_ : The body content of the template.          2. **Value**: The text or keyword you&#39;re searching for within the specified field. If left empty after the colon, the filter will look for all templates with any value in the **Field Name**.      For example, if you are searching for the template with the name of _sample_name_, the final query would look like this:     &#x60;q&#x3D;template_name:sample_name&#x60;  &lt;div class&#x3D;\&quot;info-box\&quot;&gt;   &lt;h4&gt;&lt;i class&#x3D;\&quot;fas fa-info-circle\&quot;&gt;&lt;/i&gt; Note:&lt;/h4&gt;   &lt;div&gt;    &lt;p&gt;Some characters have to be encoded. For example, if you are searching for SMS sent from the phone number +61437085284, your search query q would be:&lt;br/&gt;&lt;/p&gt;     &lt;ul&gt;       &lt;li&gt;q&#x3D;from:%2B61437085284&lt;/li&gt;     &lt;/ul&gt;     &lt;p&gt;You can use the &lt;a href&#x3D;\&quot;https://www.urlencoder.org/\&quot; target&#x3D;\&quot;_blank\&quot;&gt;URL encoder&lt;/a&gt; to encode the text. If a character is not an alphanumeric character (A-Z, a-z, 0-9), it is typically either reserved or unsafe and should be encoded.&lt;/p&gt;   &lt;/div&gt; &lt;/div&gt; | [default to &quot;field_name&quot;]
 **orderBy** | **string** | Specifies the field and order to sort the results by.  The value is composed of the field name followed by a colon and the sort direction (_asc_ for ascending or _desc_ for descending).  The default sort order is by _template_id_ in ascending order. You can use the following fields:      - _template_id_ : The ID of the Template - _template_name_ : The name of the Template - _body_ : The body content of the Template  For example, if you want to order by the _template_id_ in descending order, the query would look like this:    &#x60;order_by&#x3D;template_id:desc&#x60; | [default to &quot;template_id:asc&quot;]

### Return type

[**ViewSmsTemplates**](ViewSmsTemplates.md)

### Authorization

[basicAuth](../README.md#basicAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## ViewSpecificSmsReceipt

> ViewSpecificSmsReceipt ViewSpecificSmsReceipt(ctx, messageId).ContentType(contentType).Execute()

View Specific SMS Receipt



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
	messageId := "messageId_example" // string | The _message_id_ of the SMS delivery receipt to retrieve
	contentType := "application/json" // string |  (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.SmsAPI.ViewSpecificSmsReceipt(context.Background(), messageId).ContentType(contentType).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `SmsAPI.ViewSpecificSmsReceipt``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ViewSpecificSmsReceipt`: ViewSpecificSmsReceipt
	fmt.Fprintf(os.Stdout, "Response from `SmsAPI.ViewSpecificSmsReceipt`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**messageId** | **string** | The _message_id_ of the SMS delivery receipt to retrieve | 

### Other Parameters

Other parameters are passed through a pointer to a apiViewSpecificSmsReceiptRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **contentType** | **string** |  | 

### Return type

[**ViewSpecificSmsReceipt**](ViewSpecificSmsReceipt.md)

### Authorization

[basicAuth](../README.md#basicAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)

