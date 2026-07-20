# \EmailAPI

All URIs are relative to *https://rest.clicksend.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**CalculateEmailCampaignPrice**](EmailAPI.md#CalculateEmailCampaignPrice) | **Post** /v3/email-campaigns/price | Calculate Email Campaign Price
[**CalculateEmailPrice**](EmailAPI.md#CalculateEmailPrice) | **Post** /v3/email/price | Calculate Email Price
[**CancelEmailCampaign**](EmailAPI.md#CancelEmailCampaign) | **Put** /v3/email-campaigns/{email_campaign_id}/cancel | Cancel Email Campaign
[**CreateAllowedEmailAddress**](EmailAPI.md#CreateAllowedEmailAddress) | **Post** /v3/email/addresses | Create Allowed Email Address
[**CreateEmailDeliveryReceiptRule**](EmailAPI.md#CreateEmailDeliveryReceiptRule) | **Post** /v3/automations/email/receipts | Create Email Delivery Receipt Rule
[**CreateEmailTemplate**](EmailAPI.md#CreateEmailTemplate) | **Post** /v3/email/templates | Create Email Template
[**DeleteAllowedEmailAddress**](EmailAPI.md#DeleteAllowedEmailAddress) | **Delete** /v3/email/addresses/{email_address_id} | Delete Allowed Email Address
[**DeleteEmailDeliveryReceiptRule**](EmailAPI.md#DeleteEmailDeliveryReceiptRule) | **Delete** /v3/automations/email/receipts/{receipt_rule_id} | Delete Email Delivery Receipt Rule
[**DeleteEmailTemplate**](EmailAPI.md#DeleteEmailTemplate) | **Delete** /v3/email/templates/{template_id} | Delete Email Template
[**ExportEmailCampaignHistory**](EmailAPI.md#ExportEmailCampaignHistory) | **Get** /v3/email-campaigns/{email_campaign_id}/history/export | Export Email Campaign History
[**ExportEmailHistory**](EmailAPI.md#ExportEmailHistory) | **Get** /v3/email/history/export | Export Email History
[**SendEmail**](EmailAPI.md#SendEmail) | **Post** /v3/email/send | Send Email
[**SendEmailCampaign**](EmailAPI.md#SendEmailCampaign) | **Post** /v3/email-campaigns/send | Send Email Campaign
[**SendEmailVerificationToken**](EmailAPI.md#SendEmailVerificationToken) | **Put** /v3/email/address-verify/{email_address_id}/send | Send Email Verification Token
[**UpdateEmailCampaign**](EmailAPI.md#UpdateEmailCampaign) | **Put** /v3/email-campaigns/{email_campaign_id} | Update Email Campaign
[**UpdateEmailDeliveryReceiptRule**](EmailAPI.md#UpdateEmailDeliveryReceiptRule) | **Put** /v3/automations/email/receipts/{receipt_rule_id} | Update Email Delivery Receipt Rule
[**UpdateEmailTemplate**](EmailAPI.md#UpdateEmailTemplate) | **Put** /v3/email/templates/{template_id} | Update Email Template
[**VerifyAllowedEmailAddress**](EmailAPI.md#VerifyAllowedEmailAddress) | **Put** /v3/email/address-verify/{email_address_id}/verify/{activation_token} | Verify Allowed Email Address
[**ViewAllEmailCampaigns**](EmailAPI.md#ViewAllEmailCampaigns) | **Get** /v3/email-campaigns | View All Email Campaigns
[**ViewAllowedEmailAddress**](EmailAPI.md#ViewAllowedEmailAddress) | **Get** /v3/email/addresses/{email_address_id} | View Allowed Email Address
[**ViewAllowedEmailAddresses**](EmailAPI.md#ViewAllowedEmailAddresses) | **Get** /v3/email/addresses | View Allowed Email Addresses
[**ViewEmailCampaign**](EmailAPI.md#ViewEmailCampaign) | **Get** /v3/email-campaigns/{email_campaign_id} | View Email Campaign
[**ViewEmailCampaignHistory**](EmailAPI.md#ViewEmailCampaignHistory) | **Get** /v3/email-campaigns/{email_campaign_id}/history | View Email Campaign History
[**ViewEmailDeliveryReceiptRule**](EmailAPI.md#ViewEmailDeliveryReceiptRule) | **Get** /v3/automations/email/receipts/{receipt_rule_id} | View Email Delivery Receipt Rule
[**ViewEmailDeliveryReceiptRules**](EmailAPI.md#ViewEmailDeliveryReceiptRules) | **Get** /v3/automations/email/receipts | View Email Delivery Receipt Rules
[**ViewEmailHistory**](EmailAPI.md#ViewEmailHistory) | **Get** /v3/email/history | View Email History
[**ViewEmailTemplate**](EmailAPI.md#ViewEmailTemplate) | **Get** /v3/email/templates/{template_id} | View Email Template
[**ViewEmailTemplates**](EmailAPI.md#ViewEmailTemplates) | **Get** /v3/email/templates | View Email Templates
[**ViewMasterEmailTemplate**](EmailAPI.md#ViewMasterEmailTemplate) | **Get** /v3/email/master-templates/{template_id} | View Master Email Template
[**ViewMasterEmailTemplates**](EmailAPI.md#ViewMasterEmailTemplates) | **Get** /v3/email/master-templates | View Master Email Templates
[**ViewTemplateCategories**](EmailAPI.md#ViewTemplateCategories) | **Get** /v3/email/master-templates-categories | View Template Categories
[**ViewTemplateCategory**](EmailAPI.md#ViewTemplateCategory) | **Get** /v3/email/master-templates-categories/{category_id} | View Template Category
[**ViewTemplatesInCategory**](EmailAPI.md#ViewTemplatesInCategory) | **Get** /v3/email/master-templates-categories/{category_id}/master-templates | View Templates in Category



## CalculateEmailCampaignPrice

> CalculateEmailCampaignPrice CalculateEmailCampaignPrice(ctx).ContentType(contentType).CalculateEmailCampaignPriceRequest(calculateEmailCampaignPriceRequest).Execute()

Calculate Email Campaign Price



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
	calculateEmailCampaignPriceRequest := *openapiclient.NewCalculateEmailCampaignPriceRequest() // CalculateEmailCampaignPriceRequest |  (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.EmailAPI.CalculateEmailCampaignPrice(context.Background()).ContentType(contentType).CalculateEmailCampaignPriceRequest(calculateEmailCampaignPriceRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `EmailAPI.CalculateEmailCampaignPrice``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `CalculateEmailCampaignPrice`: CalculateEmailCampaignPrice
	fmt.Fprintf(os.Stdout, "Response from `EmailAPI.CalculateEmailCampaignPrice`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiCalculateEmailCampaignPriceRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **contentType** | **string** |  | 
 **calculateEmailCampaignPriceRequest** | [**CalculateEmailCampaignPriceRequest**](CalculateEmailCampaignPriceRequest.md) |  | 

### Return type

[**CalculateEmailCampaignPrice**](CalculateEmailCampaignPrice.md)

### Authorization

[basicAuth](../README.md#basicAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## CalculateEmailPrice

> CalculateEmailPrice CalculateEmailPrice(ctx).ContentType(contentType).CalculateEmailPriceRequest(calculateEmailPriceRequest).Execute()

Calculate Email Price



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
	calculateEmailPriceRequest := *openapiclient.NewCalculateEmailPriceRequest() // CalculateEmailPriceRequest |  (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.EmailAPI.CalculateEmailPrice(context.Background()).ContentType(contentType).CalculateEmailPriceRequest(calculateEmailPriceRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `EmailAPI.CalculateEmailPrice``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `CalculateEmailPrice`: CalculateEmailPrice
	fmt.Fprintf(os.Stdout, "Response from `EmailAPI.CalculateEmailPrice`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiCalculateEmailPriceRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **contentType** | **string** |  | 
 **calculateEmailPriceRequest** | [**CalculateEmailPriceRequest**](CalculateEmailPriceRequest.md) |  | 

### Return type

[**CalculateEmailPrice**](CalculateEmailPrice.md)

### Authorization

[basicAuth](../README.md#basicAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## CancelEmailCampaign

> CancelEmailCampaign CancelEmailCampaign(ctx, emailCampaignId).ContentType(contentType).CancelEmailCampaignRequest(cancelEmailCampaignRequest).Execute()

Cancel Email Campaign



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
	emailCampaignId := "emailCampaignId_example" // string | 
	contentType := "application/json" // string |  (optional)
	cancelEmailCampaignRequest := *openapiclient.NewCancelEmailCampaignRequest() // CancelEmailCampaignRequest |  (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.EmailAPI.CancelEmailCampaign(context.Background(), emailCampaignId).ContentType(contentType).CancelEmailCampaignRequest(cancelEmailCampaignRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `EmailAPI.CancelEmailCampaign``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `CancelEmailCampaign`: CancelEmailCampaign
	fmt.Fprintf(os.Stdout, "Response from `EmailAPI.CancelEmailCampaign`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**emailCampaignId** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiCancelEmailCampaignRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **contentType** | **string** |  | 
 **cancelEmailCampaignRequest** | [**CancelEmailCampaignRequest**](CancelEmailCampaignRequest.md) |  | 

### Return type

[**CancelEmailCampaign**](CancelEmailCampaign.md)

### Authorization

[basicAuth](../README.md#basicAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## CreateAllowedEmailAddress

> CreateAllowedEmailAddress CreateAllowedEmailAddress(ctx).ContentType(contentType).CreateAllowedEmailAddressRequest(createAllowedEmailAddressRequest).Execute()

Create Allowed Email Address



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
	createAllowedEmailAddressRequest := *openapiclient.NewCreateAllowedEmailAddressRequest() // CreateAllowedEmailAddressRequest |  (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.EmailAPI.CreateAllowedEmailAddress(context.Background()).ContentType(contentType).CreateAllowedEmailAddressRequest(createAllowedEmailAddressRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `EmailAPI.CreateAllowedEmailAddress``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `CreateAllowedEmailAddress`: CreateAllowedEmailAddress
	fmt.Fprintf(os.Stdout, "Response from `EmailAPI.CreateAllowedEmailAddress`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiCreateAllowedEmailAddressRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **contentType** | **string** |  | 
 **createAllowedEmailAddressRequest** | [**CreateAllowedEmailAddressRequest**](CreateAllowedEmailAddressRequest.md) |  | 

### Return type

[**CreateAllowedEmailAddress**](CreateAllowedEmailAddress.md)

### Authorization

[basicAuth](../README.md#basicAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## CreateEmailDeliveryReceiptRule

> CreateEmailDeliveryReceiptRule CreateEmailDeliveryReceiptRule(ctx).ContentType(contentType).CreateSmsDeliveryReceiptRuleRequest(createSmsDeliveryReceiptRuleRequest).Execute()

Create Email Delivery Receipt Rule



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
	resp, r, err := apiClient.EmailAPI.CreateEmailDeliveryReceiptRule(context.Background()).ContentType(contentType).CreateSmsDeliveryReceiptRuleRequest(createSmsDeliveryReceiptRuleRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `EmailAPI.CreateEmailDeliveryReceiptRule``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `CreateEmailDeliveryReceiptRule`: CreateEmailDeliveryReceiptRule
	fmt.Fprintf(os.Stdout, "Response from `EmailAPI.CreateEmailDeliveryReceiptRule`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiCreateEmailDeliveryReceiptRuleRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **contentType** | **string** |  | 
 **createSmsDeliveryReceiptRuleRequest** | [**CreateSmsDeliveryReceiptRuleRequest**](CreateSmsDeliveryReceiptRuleRequest.md) |  | 

### Return type

[**CreateEmailDeliveryReceiptRule**](CreateEmailDeliveryReceiptRule.md)

### Authorization

[basicAuth](../README.md#basicAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## CreateEmailTemplate

> CreateEmailTemplate CreateEmailTemplate(ctx).ContentType(contentType).CreateEmailTemplateRequest(createEmailTemplateRequest).Execute()

Create Email Template



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
	createEmailTemplateRequest := *openapiclient.NewCreateEmailTemplateRequest() // CreateEmailTemplateRequest |  (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.EmailAPI.CreateEmailTemplate(context.Background()).ContentType(contentType).CreateEmailTemplateRequest(createEmailTemplateRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `EmailAPI.CreateEmailTemplate``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `CreateEmailTemplate`: CreateEmailTemplate
	fmt.Fprintf(os.Stdout, "Response from `EmailAPI.CreateEmailTemplate`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiCreateEmailTemplateRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **contentType** | **string** |  | 
 **createEmailTemplateRequest** | [**CreateEmailTemplateRequest**](CreateEmailTemplateRequest.md) |  | 

### Return type

[**CreateEmailTemplate**](CreateEmailTemplate.md)

### Authorization

[basicAuth](../README.md#basicAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## DeleteAllowedEmailAddress

> DeleteAllowedEmailAddress DeleteAllowedEmailAddress(ctx, emailAddressId).ContentType(contentType).Execute()

Delete Allowed Email Address



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
	emailAddressId := "emailAddressId_example" // string | 
	contentType := "application/json" // string |  (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.EmailAPI.DeleteAllowedEmailAddress(context.Background(), emailAddressId).ContentType(contentType).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `EmailAPI.DeleteAllowedEmailAddress``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `DeleteAllowedEmailAddress`: DeleteAllowedEmailAddress
	fmt.Fprintf(os.Stdout, "Response from `EmailAPI.DeleteAllowedEmailAddress`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**emailAddressId** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiDeleteAllowedEmailAddressRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **contentType** | **string** |  | 

### Return type

[**DeleteAllowedEmailAddress**](DeleteAllowedEmailAddress.md)

### Authorization

[basicAuth](../README.md#basicAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## DeleteEmailDeliveryReceiptRule

> DeleteEmailDeliveryReceiptRule DeleteEmailDeliveryReceiptRule(ctx, receiptRuleId).ContentType(contentType).Execute()

Delete Email Delivery Receipt Rule



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
	resp, r, err := apiClient.EmailAPI.DeleteEmailDeliveryReceiptRule(context.Background(), receiptRuleId).ContentType(contentType).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `EmailAPI.DeleteEmailDeliveryReceiptRule``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `DeleteEmailDeliveryReceiptRule`: DeleteEmailDeliveryReceiptRule
	fmt.Fprintf(os.Stdout, "Response from `EmailAPI.DeleteEmailDeliveryReceiptRule`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**receiptRuleId** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiDeleteEmailDeliveryReceiptRuleRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **contentType** | **string** |  | 

### Return type

[**DeleteEmailDeliveryReceiptRule**](DeleteEmailDeliveryReceiptRule.md)

### Authorization

[basicAuth](../README.md#basicAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## DeleteEmailTemplate

> DeleteEmailTemplate DeleteEmailTemplate(ctx, templateId).ContentType(contentType).Execute()

Delete Email Template



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
	templateId := "templateId_example" // string | 
	contentType := "application/json" // string |  (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.EmailAPI.DeleteEmailTemplate(context.Background(), templateId).ContentType(contentType).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `EmailAPI.DeleteEmailTemplate``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `DeleteEmailTemplate`: DeleteEmailTemplate
	fmt.Fprintf(os.Stdout, "Response from `EmailAPI.DeleteEmailTemplate`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**templateId** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiDeleteEmailTemplateRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **contentType** | **string** |  | 

### Return type

[**DeleteEmailTemplate**](DeleteEmailTemplate.md)

### Authorization

[basicAuth](../README.md#basicAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## ExportEmailCampaignHistory

> ExportEmailCampaignHistory(ctx, emailCampaignId).ContentType(contentType).Execute()

Export Email Campaign History



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
	emailCampaignId := "emailCampaignId_example" // string | 
	contentType := "application/json" // string |  (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	r, err := apiClient.EmailAPI.ExportEmailCampaignHistory(context.Background(), emailCampaignId).ContentType(contentType).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `EmailAPI.ExportEmailCampaignHistory``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**emailCampaignId** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiExportEmailCampaignHistoryRequest struct via the builder pattern


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


## ExportEmailHistory

> ExportEmailHistory ExportEmailHistory(ctx).ContentType(contentType).Execute()

Export Email History



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
	resp, r, err := apiClient.EmailAPI.ExportEmailHistory(context.Background()).ContentType(contentType).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `EmailAPI.ExportEmailHistory``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ExportEmailHistory`: ExportEmailHistory
	fmt.Fprintf(os.Stdout, "Response from `EmailAPI.ExportEmailHistory`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiExportEmailHistoryRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **contentType** | **string** |  | 

### Return type

[**ExportEmailHistory**](ExportEmailHistory.md)

### Authorization

[basicAuth](../README.md#basicAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## SendEmail

> SendEmail SendEmail(ctx).ContentType(contentType).SendEmailRequest(sendEmailRequest).Execute()

Send Email



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
	sendEmailRequest := *openapiclient.NewSendEmailRequest() // SendEmailRequest |  (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.EmailAPI.SendEmail(context.Background()).ContentType(contentType).SendEmailRequest(sendEmailRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `EmailAPI.SendEmail``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `SendEmail`: SendEmail
	fmt.Fprintf(os.Stdout, "Response from `EmailAPI.SendEmail`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiSendEmailRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **contentType** | **string** |  | 
 **sendEmailRequest** | [**SendEmailRequest**](SendEmailRequest.md) |  | 

### Return type

[**SendEmail**](SendEmail.md)

### Authorization

[basicAuth](../README.md#basicAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## SendEmailCampaign

> SendEmailCampaign SendEmailCampaign(ctx).ContentType(contentType).SendEmailCampaignRequest(sendEmailCampaignRequest).Execute()

Send Email Campaign



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
	sendEmailCampaignRequest := *openapiclient.NewSendEmailCampaignRequest() // SendEmailCampaignRequest |  (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.EmailAPI.SendEmailCampaign(context.Background()).ContentType(contentType).SendEmailCampaignRequest(sendEmailCampaignRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `EmailAPI.SendEmailCampaign``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `SendEmailCampaign`: SendEmailCampaign
	fmt.Fprintf(os.Stdout, "Response from `EmailAPI.SendEmailCampaign`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiSendEmailCampaignRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **contentType** | **string** |  | 
 **sendEmailCampaignRequest** | [**SendEmailCampaignRequest**](SendEmailCampaignRequest.md) |  | 

### Return type

[**SendEmailCampaign**](SendEmailCampaign.md)

### Authorization

[basicAuth](../README.md#basicAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## SendEmailVerificationToken

> SendEmailVerificationToken SendEmailVerificationToken(ctx, emailAddressId).ContentType(contentType).SendEmailVerificationTokenRequest(sendEmailVerificationTokenRequest).Execute()

Send Email Verification Token



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
	emailAddressId := "emailAddressId_example" // string | 
	contentType := "application/json" // string |  (optional)
	sendEmailVerificationTokenRequest := *openapiclient.NewSendEmailVerificationTokenRequest() // SendEmailVerificationTokenRequest |  (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.EmailAPI.SendEmailVerificationToken(context.Background(), emailAddressId).ContentType(contentType).SendEmailVerificationTokenRequest(sendEmailVerificationTokenRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `EmailAPI.SendEmailVerificationToken``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `SendEmailVerificationToken`: SendEmailVerificationToken
	fmt.Fprintf(os.Stdout, "Response from `EmailAPI.SendEmailVerificationToken`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**emailAddressId** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiSendEmailVerificationTokenRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **contentType** | **string** |  | 
 **sendEmailVerificationTokenRequest** | [**SendEmailVerificationTokenRequest**](SendEmailVerificationTokenRequest.md) |  | 

### Return type

[**SendEmailVerificationToken**](SendEmailVerificationToken.md)

### Authorization

[basicAuth](../README.md#basicAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## UpdateEmailCampaign

> UpdateEmailCampaign UpdateEmailCampaign(ctx, emailCampaignId).ContentType(contentType).UpdateEmailCampaignRequest(updateEmailCampaignRequest).Execute()

Update Email Campaign



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
	emailCampaignId := "emailCampaignId_example" // string | 
	contentType := "application/json" // string |  (optional)
	updateEmailCampaignRequest := *openapiclient.NewUpdateEmailCampaignRequest() // UpdateEmailCampaignRequest |  (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.EmailAPI.UpdateEmailCampaign(context.Background(), emailCampaignId).ContentType(contentType).UpdateEmailCampaignRequest(updateEmailCampaignRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `EmailAPI.UpdateEmailCampaign``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `UpdateEmailCampaign`: UpdateEmailCampaign
	fmt.Fprintf(os.Stdout, "Response from `EmailAPI.UpdateEmailCampaign`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**emailCampaignId** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiUpdateEmailCampaignRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **contentType** | **string** |  | 
 **updateEmailCampaignRequest** | [**UpdateEmailCampaignRequest**](UpdateEmailCampaignRequest.md) |  | 

### Return type

[**UpdateEmailCampaign**](UpdateEmailCampaign.md)

### Authorization

[basicAuth](../README.md#basicAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## UpdateEmailDeliveryReceiptRule

> UpdateEmailDeliveryReceiptRule UpdateEmailDeliveryReceiptRule(ctx, receiptRuleId).ContentType(contentType).CreateSmsDeliveryReceiptRuleRequest(createSmsDeliveryReceiptRuleRequest).Execute()

Update Email Delivery Receipt Rule



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
	resp, r, err := apiClient.EmailAPI.UpdateEmailDeliveryReceiptRule(context.Background(), receiptRuleId).ContentType(contentType).CreateSmsDeliveryReceiptRuleRequest(createSmsDeliveryReceiptRuleRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `EmailAPI.UpdateEmailDeliveryReceiptRule``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `UpdateEmailDeliveryReceiptRule`: UpdateEmailDeliveryReceiptRule
	fmt.Fprintf(os.Stdout, "Response from `EmailAPI.UpdateEmailDeliveryReceiptRule`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**receiptRuleId** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiUpdateEmailDeliveryReceiptRuleRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **contentType** | **string** |  | 
 **createSmsDeliveryReceiptRuleRequest** | [**CreateSmsDeliveryReceiptRuleRequest**](CreateSmsDeliveryReceiptRuleRequest.md) |  | 

### Return type

[**UpdateEmailDeliveryReceiptRule**](UpdateEmailDeliveryReceiptRule.md)

### Authorization

[basicAuth](../README.md#basicAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## UpdateEmailTemplate

> UpdateEmailTemplate UpdateEmailTemplate(ctx, templateId).ContentType(contentType).UpdateEmailTemplateRequest(updateEmailTemplateRequest).Execute()

Update Email Template



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
	templateId := "templateId_example" // string | 
	contentType := "application/json" // string |  (optional)
	updateEmailTemplateRequest := *openapiclient.NewUpdateEmailTemplateRequest() // UpdateEmailTemplateRequest |  (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.EmailAPI.UpdateEmailTemplate(context.Background(), templateId).ContentType(contentType).UpdateEmailTemplateRequest(updateEmailTemplateRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `EmailAPI.UpdateEmailTemplate``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `UpdateEmailTemplate`: UpdateEmailTemplate
	fmt.Fprintf(os.Stdout, "Response from `EmailAPI.UpdateEmailTemplate`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**templateId** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiUpdateEmailTemplateRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **contentType** | **string** |  | 
 **updateEmailTemplateRequest** | [**UpdateEmailTemplateRequest**](UpdateEmailTemplateRequest.md) |  | 

### Return type

[**UpdateEmailTemplate**](UpdateEmailTemplate.md)

### Authorization

[basicAuth](../README.md#basicAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## VerifyAllowedEmailAddress

> VerifyAllowedEmailAddress VerifyAllowedEmailAddress(ctx, emailAddressId, activationToken).ContentType(contentType).VerifyAllowedEmailAddressRequest(verifyAllowedEmailAddressRequest).Execute()

Verify Allowed Email Address



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
	emailAddressId := "emailAddressId_example" // string | 
	activationToken := "activationToken_example" // string | 
	contentType := "application/json" // string |  (optional)
	verifyAllowedEmailAddressRequest := *openapiclient.NewVerifyAllowedEmailAddressRequest() // VerifyAllowedEmailAddressRequest |  (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.EmailAPI.VerifyAllowedEmailAddress(context.Background(), emailAddressId, activationToken).ContentType(contentType).VerifyAllowedEmailAddressRequest(verifyAllowedEmailAddressRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `EmailAPI.VerifyAllowedEmailAddress``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `VerifyAllowedEmailAddress`: VerifyAllowedEmailAddress
	fmt.Fprintf(os.Stdout, "Response from `EmailAPI.VerifyAllowedEmailAddress`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**emailAddressId** | **string** |  | 
**activationToken** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiVerifyAllowedEmailAddressRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


 **contentType** | **string** |  | 
 **verifyAllowedEmailAddressRequest** | [**VerifyAllowedEmailAddressRequest**](VerifyAllowedEmailAddressRequest.md) |  | 

### Return type

[**VerifyAllowedEmailAddress**](VerifyAllowedEmailAddress.md)

### Authorization

[basicAuth](../README.md#basicAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## ViewAllEmailCampaigns

> ViewAllEmailCampaigns ViewAllEmailCampaigns(ctx).ContentType(contentType).Execute()

View All Email Campaigns



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
	resp, r, err := apiClient.EmailAPI.ViewAllEmailCampaigns(context.Background()).ContentType(contentType).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `EmailAPI.ViewAllEmailCampaigns``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ViewAllEmailCampaigns`: ViewAllEmailCampaigns
	fmt.Fprintf(os.Stdout, "Response from `EmailAPI.ViewAllEmailCampaigns`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiViewAllEmailCampaignsRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **contentType** | **string** |  | 

### Return type

[**ViewAllEmailCampaigns**](ViewAllEmailCampaigns.md)

### Authorization

[basicAuth](../README.md#basicAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## ViewAllowedEmailAddress

> ViewAllowedEmailAddress ViewAllowedEmailAddress(ctx, emailAddressId).ContentType(contentType).Execute()

View Allowed Email Address



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
	emailAddressId := "emailAddressId_example" // string | 
	contentType := "application/json" // string |  (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.EmailAPI.ViewAllowedEmailAddress(context.Background(), emailAddressId).ContentType(contentType).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `EmailAPI.ViewAllowedEmailAddress``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ViewAllowedEmailAddress`: ViewAllowedEmailAddress
	fmt.Fprintf(os.Stdout, "Response from `EmailAPI.ViewAllowedEmailAddress`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**emailAddressId** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiViewAllowedEmailAddressRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **contentType** | **string** |  | 

### Return type

[**ViewAllowedEmailAddress**](ViewAllowedEmailAddress.md)

### Authorization

[basicAuth](../README.md#basicAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## ViewAllowedEmailAddresses

> ViewAllowedEmailAddresses ViewAllowedEmailAddresses(ctx).ContentType(contentType).Execute()

View Allowed Email Addresses



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
	resp, r, err := apiClient.EmailAPI.ViewAllowedEmailAddresses(context.Background()).ContentType(contentType).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `EmailAPI.ViewAllowedEmailAddresses``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ViewAllowedEmailAddresses`: ViewAllowedEmailAddresses
	fmt.Fprintf(os.Stdout, "Response from `EmailAPI.ViewAllowedEmailAddresses`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiViewAllowedEmailAddressesRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **contentType** | **string** |  | 

### Return type

[**ViewAllowedEmailAddresses**](ViewAllowedEmailAddresses.md)

### Authorization

[basicAuth](../README.md#basicAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## ViewEmailCampaign

> ViewEmailCampaign ViewEmailCampaign(ctx, emailCampaignId).ContentType(contentType).Execute()

View Email Campaign



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
	emailCampaignId := "emailCampaignId_example" // string | 
	contentType := "application/json" // string |  (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.EmailAPI.ViewEmailCampaign(context.Background(), emailCampaignId).ContentType(contentType).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `EmailAPI.ViewEmailCampaign``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ViewEmailCampaign`: ViewEmailCampaign
	fmt.Fprintf(os.Stdout, "Response from `EmailAPI.ViewEmailCampaign`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**emailCampaignId** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiViewEmailCampaignRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **contentType** | **string** |  | 

### Return type

[**ViewEmailCampaign**](ViewEmailCampaign.md)

### Authorization

[basicAuth](../README.md#basicAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## ViewEmailCampaignHistory

> ViewEmailCampaignHistory ViewEmailCampaignHistory(ctx, emailCampaignId).ContentType(contentType).Execute()

View Email Campaign History



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
	emailCampaignId := "emailCampaignId_example" // string | 
	contentType := "application/json" // string |  (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.EmailAPI.ViewEmailCampaignHistory(context.Background(), emailCampaignId).ContentType(contentType).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `EmailAPI.ViewEmailCampaignHistory``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ViewEmailCampaignHistory`: ViewEmailCampaignHistory
	fmt.Fprintf(os.Stdout, "Response from `EmailAPI.ViewEmailCampaignHistory`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**emailCampaignId** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiViewEmailCampaignHistoryRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **contentType** | **string** |  | 

### Return type

[**ViewEmailCampaignHistory**](ViewEmailCampaignHistory.md)

### Authorization

[basicAuth](../README.md#basicAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## ViewEmailDeliveryReceiptRule

> ViewEmailDeliveryReceiptRule ViewEmailDeliveryReceiptRule(ctx, receiptRuleId).ContentType(contentType).Execute()

View Email Delivery Receipt Rule



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
	resp, r, err := apiClient.EmailAPI.ViewEmailDeliveryReceiptRule(context.Background(), receiptRuleId).ContentType(contentType).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `EmailAPI.ViewEmailDeliveryReceiptRule``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ViewEmailDeliveryReceiptRule`: ViewEmailDeliveryReceiptRule
	fmt.Fprintf(os.Stdout, "Response from `EmailAPI.ViewEmailDeliveryReceiptRule`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**receiptRuleId** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiViewEmailDeliveryReceiptRuleRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **contentType** | **string** |  | 

### Return type

[**ViewEmailDeliveryReceiptRule**](ViewEmailDeliveryReceiptRule.md)

### Authorization

[basicAuth](../README.md#basicAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## ViewEmailDeliveryReceiptRules

> ViewEmailDeliveryReceiptRules ViewEmailDeliveryReceiptRules(ctx).ContentType(contentType).Execute()

View Email Delivery Receipt Rules



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
	resp, r, err := apiClient.EmailAPI.ViewEmailDeliveryReceiptRules(context.Background()).ContentType(contentType).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `EmailAPI.ViewEmailDeliveryReceiptRules``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ViewEmailDeliveryReceiptRules`: ViewEmailDeliveryReceiptRules
	fmt.Fprintf(os.Stdout, "Response from `EmailAPI.ViewEmailDeliveryReceiptRules`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiViewEmailDeliveryReceiptRulesRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **contentType** | **string** |  | 

### Return type

[**ViewEmailDeliveryReceiptRules**](ViewEmailDeliveryReceiptRules.md)

### Authorization

[basicAuth](../README.md#basicAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## ViewEmailHistory

> ViewEmailHistory ViewEmailHistory(ctx).ContentType(contentType).Execute()

View Email History



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
	resp, r, err := apiClient.EmailAPI.ViewEmailHistory(context.Background()).ContentType(contentType).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `EmailAPI.ViewEmailHistory``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ViewEmailHistory`: ViewEmailHistory
	fmt.Fprintf(os.Stdout, "Response from `EmailAPI.ViewEmailHistory`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiViewEmailHistoryRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **contentType** | **string** |  | 

### Return type

[**ViewEmailHistory**](ViewEmailHistory.md)

### Authorization

[basicAuth](../README.md#basicAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## ViewEmailTemplate

> ViewEmailTemplate ViewEmailTemplate(ctx, templateId).ContentType(contentType).Execute()

View Email Template



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
	templateId := "templateId_example" // string | 
	contentType := "application/json" // string |  (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.EmailAPI.ViewEmailTemplate(context.Background(), templateId).ContentType(contentType).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `EmailAPI.ViewEmailTemplate``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ViewEmailTemplate`: ViewEmailTemplate
	fmt.Fprintf(os.Stdout, "Response from `EmailAPI.ViewEmailTemplate`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**templateId** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiViewEmailTemplateRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **contentType** | **string** |  | 

### Return type

[**ViewEmailTemplate**](ViewEmailTemplate.md)

### Authorization

[basicAuth](../README.md#basicAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## ViewEmailTemplates

> ViewEmailTemplates ViewEmailTemplates(ctx).ContentType(contentType).Execute()

View Email Templates



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
	resp, r, err := apiClient.EmailAPI.ViewEmailTemplates(context.Background()).ContentType(contentType).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `EmailAPI.ViewEmailTemplates``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ViewEmailTemplates`: ViewEmailTemplates
	fmt.Fprintf(os.Stdout, "Response from `EmailAPI.ViewEmailTemplates`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiViewEmailTemplatesRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **contentType** | **string** |  | 

### Return type

[**ViewEmailTemplates**](ViewEmailTemplates.md)

### Authorization

[basicAuth](../README.md#basicAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## ViewMasterEmailTemplate

> ViewMasterEmailTemplate ViewMasterEmailTemplate(ctx, templateId).ContentType(contentType).Execute()

View Master Email Template



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
	templateId := "templateId_example" // string | 
	contentType := "application/json" // string |  (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.EmailAPI.ViewMasterEmailTemplate(context.Background(), templateId).ContentType(contentType).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `EmailAPI.ViewMasterEmailTemplate``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ViewMasterEmailTemplate`: ViewMasterEmailTemplate
	fmt.Fprintf(os.Stdout, "Response from `EmailAPI.ViewMasterEmailTemplate`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**templateId** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiViewMasterEmailTemplateRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **contentType** | **string** |  | 

### Return type

[**ViewMasterEmailTemplate**](ViewMasterEmailTemplate.md)

### Authorization

[basicAuth](../README.md#basicAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## ViewMasterEmailTemplates

> ViewMasterEmailTemplates ViewMasterEmailTemplates(ctx).ContentType(contentType).Execute()

View Master Email Templates



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
	resp, r, err := apiClient.EmailAPI.ViewMasterEmailTemplates(context.Background()).ContentType(contentType).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `EmailAPI.ViewMasterEmailTemplates``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ViewMasterEmailTemplates`: ViewMasterEmailTemplates
	fmt.Fprintf(os.Stdout, "Response from `EmailAPI.ViewMasterEmailTemplates`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiViewMasterEmailTemplatesRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **contentType** | **string** |  | 

### Return type

[**ViewMasterEmailTemplates**](ViewMasterEmailTemplates.md)

### Authorization

[basicAuth](../README.md#basicAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## ViewTemplateCategories

> ViewTemplateCategories ViewTemplateCategories(ctx).ContentType(contentType).Execute()

View Template Categories



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
	resp, r, err := apiClient.EmailAPI.ViewTemplateCategories(context.Background()).ContentType(contentType).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `EmailAPI.ViewTemplateCategories``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ViewTemplateCategories`: ViewTemplateCategories
	fmt.Fprintf(os.Stdout, "Response from `EmailAPI.ViewTemplateCategories`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiViewTemplateCategoriesRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **contentType** | **string** |  | 

### Return type

[**ViewTemplateCategories**](ViewTemplateCategories.md)

### Authorization

[basicAuth](../README.md#basicAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## ViewTemplateCategory

> ViewTemplateCategory ViewTemplateCategory(ctx, categoryId).ContentType(contentType).Execute()

View Template Category



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
	categoryId := "categoryId_example" // string | 
	contentType := "application/json" // string |  (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.EmailAPI.ViewTemplateCategory(context.Background(), categoryId).ContentType(contentType).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `EmailAPI.ViewTemplateCategory``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ViewTemplateCategory`: ViewTemplateCategory
	fmt.Fprintf(os.Stdout, "Response from `EmailAPI.ViewTemplateCategory`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**categoryId** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiViewTemplateCategoryRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **contentType** | **string** |  | 

### Return type

[**ViewTemplateCategory**](ViewTemplateCategory.md)

### Authorization

[basicAuth](../README.md#basicAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## ViewTemplatesInCategory

> ViewTemplatesInCategory ViewTemplatesInCategory(ctx, categoryId).ContentType(contentType).Execute()

View Templates in Category



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
	categoryId := "categoryId_example" // string | 
	contentType := "application/json" // string |  (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.EmailAPI.ViewTemplatesInCategory(context.Background(), categoryId).ContentType(contentType).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `EmailAPI.ViewTemplatesInCategory``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ViewTemplatesInCategory`: ViewTemplatesInCategory
	fmt.Fprintf(os.Stdout, "Response from `EmailAPI.ViewTemplatesInCategory`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**categoryId** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiViewTemplatesInCategoryRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **contentType** | **string** |  | 

### Return type

[**ViewTemplatesInCategory**](ViewTemplatesInCategory.md)

### Authorization

[basicAuth](../README.md#basicAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)

