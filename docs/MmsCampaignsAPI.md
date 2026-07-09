# \MmsCampaignsAPI

All URIs are relative to *https://rest.clicksend.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**CalculateMmsCampaignPrice**](MmsCampaignsAPI.md#CalculateMmsCampaignPrice) | **Post** /v3/mms-campaigns/price | Calculate MMS Campaign Price
[**CancelMmsCampaign**](MmsCampaignsAPI.md#CancelMmsCampaign) | **Put** /v3/mms-campaigns/{mms_campaign_id}/cancel | Cancel MMS Campaign
[**SendMmsCampaign**](MmsCampaignsAPI.md#SendMmsCampaign) | **Post** /v3/mms-campaigns/send | Send MMS Campaign
[**UpdateMmsCampaign**](MmsCampaignsAPI.md#UpdateMmsCampaign) | **Put** /v3/mms-campaigns/{mms_campaign_id} | Update MMS Campaign
[**ViewAllMmsCampaigns**](MmsCampaignsAPI.md#ViewAllMmsCampaigns) | **Get** /v3/mms-campaigns | View All MMS Campaigns
[**ViewMmsCampaign**](MmsCampaignsAPI.md#ViewMmsCampaign) | **Get** /v3/mms-campaigns/{mms_campaign_id} | View MMS Campaign



## CalculateMmsCampaignPrice

> CalculateMmsCampaignPrice CalculateMmsCampaignPrice(ctx).ContentType(contentType).Body(body).Execute()

Calculate MMS Campaign Price



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
	body := map[string]interface{}{ ... } // map[string]interface{} |  (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.MmsCampaignsAPI.CalculateMmsCampaignPrice(context.Background()).ContentType(contentType).Body(body).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `MmsCampaignsAPI.CalculateMmsCampaignPrice``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `CalculateMmsCampaignPrice`: CalculateMmsCampaignPrice
	fmt.Fprintf(os.Stdout, "Response from `MmsCampaignsAPI.CalculateMmsCampaignPrice`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiCalculateMmsCampaignPriceRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **contentType** | **string** |  | 
 **body** | **map[string]interface{}** |  | 

### Return type

[**CalculateMmsCampaignPrice**](CalculateMmsCampaignPrice.md)

### Authorization

[basicAuth](../README.md#basicAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## CancelMmsCampaign

> CancelMmsCampaign CancelMmsCampaign(ctx, mmsCampaignId).ContentType(contentType).CalculateSmsCampaignPriceRequest(calculateSmsCampaignPriceRequest).Execute()

Cancel MMS Campaign



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
	mmsCampaignId := "mmsCampaignId_example" // string | 
	contentType := "application/json" // string |  (optional)
	calculateSmsCampaignPriceRequest := *openapiclient.NewCalculateSmsCampaignPriceRequest() // CalculateSmsCampaignPriceRequest |  (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.MmsCampaignsAPI.CancelMmsCampaign(context.Background(), mmsCampaignId).ContentType(contentType).CalculateSmsCampaignPriceRequest(calculateSmsCampaignPriceRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `MmsCampaignsAPI.CancelMmsCampaign``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `CancelMmsCampaign`: CancelMmsCampaign
	fmt.Fprintf(os.Stdout, "Response from `MmsCampaignsAPI.CancelMmsCampaign`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**mmsCampaignId** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiCancelMmsCampaignRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **contentType** | **string** |  | 
 **calculateSmsCampaignPriceRequest** | [**CalculateSmsCampaignPriceRequest**](CalculateSmsCampaignPriceRequest.md) |  | 

### Return type

[**CancelMmsCampaign**](CancelMmsCampaign.md)

### Authorization

[basicAuth](../README.md#basicAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## SendMmsCampaign

> SendMmsCampaign SendMmsCampaign(ctx).ContentType(contentType).SendMmsCampaignRequest(sendMmsCampaignRequest).Execute()

Send MMS Campaign



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
	sendMmsCampaignRequest := *openapiclient.NewSendMmsCampaignRequest() // SendMmsCampaignRequest |  (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.MmsCampaignsAPI.SendMmsCampaign(context.Background()).ContentType(contentType).SendMmsCampaignRequest(sendMmsCampaignRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `MmsCampaignsAPI.SendMmsCampaign``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `SendMmsCampaign`: SendMmsCampaign
	fmt.Fprintf(os.Stdout, "Response from `MmsCampaignsAPI.SendMmsCampaign`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiSendMmsCampaignRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **contentType** | **string** |  | 
 **sendMmsCampaignRequest** | [**SendMmsCampaignRequest**](SendMmsCampaignRequest.md) |  | 

### Return type

[**SendMmsCampaign**](SendMmsCampaign.md)

### Authorization

[basicAuth](../README.md#basicAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## UpdateMmsCampaign

> UpdateMmsCampaign UpdateMmsCampaign(ctx, mmsCampaignId).ContentType(contentType).CalculateSmsCampaignPriceRequest(calculateSmsCampaignPriceRequest).Execute()

Update MMS Campaign



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
	mmsCampaignId := "mmsCampaignId_example" // string | 
	contentType := "application/json" // string |  (optional)
	calculateSmsCampaignPriceRequest := *openapiclient.NewCalculateSmsCampaignPriceRequest() // CalculateSmsCampaignPriceRequest |  (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.MmsCampaignsAPI.UpdateMmsCampaign(context.Background(), mmsCampaignId).ContentType(contentType).CalculateSmsCampaignPriceRequest(calculateSmsCampaignPriceRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `MmsCampaignsAPI.UpdateMmsCampaign``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `UpdateMmsCampaign`: UpdateMmsCampaign
	fmt.Fprintf(os.Stdout, "Response from `MmsCampaignsAPI.UpdateMmsCampaign`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**mmsCampaignId** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiUpdateMmsCampaignRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **contentType** | **string** |  | 
 **calculateSmsCampaignPriceRequest** | [**CalculateSmsCampaignPriceRequest**](CalculateSmsCampaignPriceRequest.md) |  | 

### Return type

[**UpdateMmsCampaign**](UpdateMmsCampaign.md)

### Authorization

[basicAuth](../README.md#basicAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## ViewAllMmsCampaigns

> ViewAllMmsCampaigns ViewAllMmsCampaigns(ctx).ContentType(contentType).Execute()

View All MMS Campaigns



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
	resp, r, err := apiClient.MmsCampaignsAPI.ViewAllMmsCampaigns(context.Background()).ContentType(contentType).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `MmsCampaignsAPI.ViewAllMmsCampaigns``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ViewAllMmsCampaigns`: ViewAllMmsCampaigns
	fmt.Fprintf(os.Stdout, "Response from `MmsCampaignsAPI.ViewAllMmsCampaigns`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiViewAllMmsCampaignsRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **contentType** | **string** |  | 

### Return type

[**ViewAllMmsCampaigns**](ViewAllMmsCampaigns.md)

### Authorization

[basicAuth](../README.md#basicAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## ViewMmsCampaign

> ViewMmsCampaign ViewMmsCampaign(ctx, mmsCampaignId).ContentType(contentType).Execute()

View MMS Campaign



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
	mmsCampaignId := "mmsCampaignId_example" // string | 
	contentType := "application/json" // string |  (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.MmsCampaignsAPI.ViewMmsCampaign(context.Background(), mmsCampaignId).ContentType(contentType).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `MmsCampaignsAPI.ViewMmsCampaign``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ViewMmsCampaign`: ViewMmsCampaign
	fmt.Fprintf(os.Stdout, "Response from `MmsCampaignsAPI.ViewMmsCampaign`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**mmsCampaignId** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiViewMmsCampaignRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **contentType** | **string** |  | 

### Return type

[**ViewMmsCampaign**](ViewMmsCampaign.md)

### Authorization

[basicAuth](../README.md#basicAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)

