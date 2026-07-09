# \NumbersAPI

All URIs are relative to *https://rest.clicksend.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**PurchaseDedicatedNumber**](NumbersAPI.md#PurchaseDedicatedNumber) | **Post** /v3/numbers/buy/{dedicated_number} | Purchase Dedicated Number
[**RegisterNumbers**](NumbersAPI.md#RegisterNumbers) | **Post** /v3/numbers/registrations/number-types/{number_type}/country/{country_code} | Register Numbers
[**ViewAvailableNumbers**](NumbersAPI.md#ViewAvailableNumbers) | **Get** /v3/numbers/search/{country} | View Available Numbers
[**ViewYourNumbers**](NumbersAPI.md#ViewYourNumbers) | **Get** /v3/numbers | View Your Numbers



## PurchaseDedicatedNumber

> PurchaseDedicatedNumber PurchaseDedicatedNumber(ctx, dedicatedNumber).BuyNumberRequest(buyNumberRequest).ContentType(contentType).Type_(type_).Execute()

Purchase Dedicated Number



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
	dedicatedNumber := "+614197651956" // string | Phone number to purchase
	buyNumberRequest := *openapiclient.NewBuyNumberRequest("+614197651956", "sms") // BuyNumberRequest | 
	contentType := "application/json" // string |  (optional)
	type_ := "sms" // string |  (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.NumbersAPI.PurchaseDedicatedNumber(context.Background(), dedicatedNumber).BuyNumberRequest(buyNumberRequest).ContentType(contentType).Type_(type_).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `NumbersAPI.PurchaseDedicatedNumber``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `PurchaseDedicatedNumber`: PurchaseDedicatedNumber
	fmt.Fprintf(os.Stdout, "Response from `NumbersAPI.PurchaseDedicatedNumber`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**dedicatedNumber** | **string** | Phone number to purchase | 

### Other Parameters

Other parameters are passed through a pointer to a apiPurchaseDedicatedNumberRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **buyNumberRequest** | [**BuyNumberRequest**](BuyNumberRequest.md) |  | 
 **contentType** | **string** |  | 
 **type_** | **string** |  | 

### Return type

[**PurchaseDedicatedNumber**](PurchaseDedicatedNumber.md)

### Authorization

[basicAuth](../README.md#basicAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## RegisterNumbers

> RegisterNumbers RegisterNumbers(ctx, numberType, countryCode).ContentType(contentType).RegisterNumbersRequest(registerNumbersRequest).Execute()

Register Numbers



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
	numberType := "10dlc" // string | The type of number being registered
	countryCode := "US, CA" // string | Two-character ISO country code
	contentType := "application/json" // string |  (optional)
	registerNumbersRequest := *openapiclient.NewRegisterNumbersRequest("John Doe", "ClickSend", "john.doe@clicksend.com", "https://clicksend.com", "Get 20% off on your next purchase! Visit our website for details.", "Marketing", "+1-800-555-0199", "416, 647, 905") // RegisterNumbersRequest |  (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.NumbersAPI.RegisterNumbers(context.Background(), numberType, countryCode).ContentType(contentType).RegisterNumbersRequest(registerNumbersRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `NumbersAPI.RegisterNumbers``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `RegisterNumbers`: RegisterNumbers
	fmt.Fprintf(os.Stdout, "Response from `NumbersAPI.RegisterNumbers`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**numberType** | **string** | The type of number being registered | 
**countryCode** | **string** | Two-character ISO country code | 

### Other Parameters

Other parameters are passed through a pointer to a apiRegisterNumbersRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


 **contentType** | **string** |  | 
 **registerNumbersRequest** | [**RegisterNumbersRequest**](RegisterNumbersRequest.md) |  | 

### Return type

[**RegisterNumbers**](RegisterNumbers.md)

### Authorization

[basicAuth](../README.md#basicAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## ViewAvailableNumbers

> ViewAvailableNumbers ViewAvailableNumbers(ctx, country).ContentType(contentType).Execute()

View Available Numbers



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
	country := "country_example" // string | 
	contentType := "application/json" // string |  (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.NumbersAPI.ViewAvailableNumbers(context.Background(), country).ContentType(contentType).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `NumbersAPI.ViewAvailableNumbers``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ViewAvailableNumbers`: ViewAvailableNumbers
	fmt.Fprintf(os.Stdout, "Response from `NumbersAPI.ViewAvailableNumbers`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**country** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiViewAvailableNumbersRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **contentType** | **string** |  | 

### Return type

[**ViewAvailableNumbers**](ViewAvailableNumbers.md)

### Authorization

[basicAuth](../README.md#basicAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## ViewYourNumbers

> ViewYourNumbers ViewYourNumbers(ctx).ContentType(contentType).Page(page).Limit(limit).Q(q).Q2(q2).ExcludingNumberType(excludingNumberType).Exclude10dlcCampaign(exclude10dlcCampaign).Execute()

View Your Numbers



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
	page := int32(1) // int32 | Page number (optional) (default to 1)
	limit := int32(100) // int32 | Number of records per page (optional) (default to 15)
	q := "type:sms,number_type:longcode,country:AU" // string | Filter numbers based on multiple criteria. The query string should be formatted as key-value pairs separated by commas. Available filter keys: - `type`: Message type (e.g., `SMS`, `MMS`) - `number_type`: Number classification (e.g., `longcode`, `shortcode`, `tollfree`, `10DLC`) - `country`: Two-letter country code (e.g., `AU`, `US`)  (optional)
	q2 := "type:mms" // string |  (optional)
	excludingNumberType := "10DLC" // string | Exclude specific number types from the results. Available number types: - `shortcode` - `tollfree` - `10DLC`  (optional)
	exclude10dlcCampaign := true // bool | When set to true, excludes all numbers that are associated with 10DLC campaigns (optional) (default to false)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.NumbersAPI.ViewYourNumbers(context.Background()).ContentType(contentType).Page(page).Limit(limit).Q(q).Q2(q2).ExcludingNumberType(excludingNumberType).Exclude10dlcCampaign(exclude10dlcCampaign).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `NumbersAPI.ViewYourNumbers``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ViewYourNumbers`: ViewYourNumbers
	fmt.Fprintf(os.Stdout, "Response from `NumbersAPI.ViewYourNumbers`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiViewYourNumbersRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **contentType** | **string** |  | 
 **page** | **int32** | Page number | [default to 1]
 **limit** | **int32** | Number of records per page | [default to 15]
 **q** | **string** | Filter numbers based on multiple criteria. The query string should be formatted as key-value pairs separated by commas. Available filter keys: - &#x60;type&#x60;: Message type (e.g., &#x60;SMS&#x60;, &#x60;MMS&#x60;) - &#x60;number_type&#x60;: Number classification (e.g., &#x60;longcode&#x60;, &#x60;shortcode&#x60;, &#x60;tollfree&#x60;, &#x60;10DLC&#x60;) - &#x60;country&#x60;: Two-letter country code (e.g., &#x60;AU&#x60;, &#x60;US&#x60;)  | 
 **q2** | **string** |  | 
 **excludingNumberType** | **string** | Exclude specific number types from the results. Available number types: - &#x60;shortcode&#x60; - &#x60;tollfree&#x60; - &#x60;10DLC&#x60;  | 
 **exclude10dlcCampaign** | **bool** | When set to true, excludes all numbers that are associated with 10DLC campaigns | [default to false]

### Return type

[**ViewYourNumbers**](ViewYourNumbers.md)

### Authorization

[basicAuth](../README.md#basicAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)

