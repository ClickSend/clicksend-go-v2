# \SmsCampaignsAPI

All URIs are relative to *https://rest.clicksend.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**CalculateSmsCampaignPrice**](SmsCampaignsAPI.md#CalculateSmsCampaignPrice) | **Post** /v3/sms-campaigns/price | Calculate SMS Campaign Price
[**CancelSmsCampaign**](SmsCampaignsAPI.md#CancelSmsCampaign) | **Put** /v3/sms-campaigns/{sms_campaign_id}/cancel | Cancel SMS Campaign
[**SendSmsCampaign**](SmsCampaignsAPI.md#SendSmsCampaign) | **Post** /v3/sms-campaigns/send | Send SMS Campaign
[**UpdateSmsCampaign**](SmsCampaignsAPI.md#UpdateSmsCampaign) | **Put** /v3/sms-campaigns/{sms_campaign_id} | Update SMS Campaign
[**ViewSmsCampaigns**](SmsCampaignsAPI.md#ViewSmsCampaigns) | **Get** /v3/sms-campaigns | View SMS Campaigns
[**ViewSpecificSmsCampaign**](SmsCampaignsAPI.md#ViewSpecificSmsCampaign) | **Get** /v3/sms-campaigns/{sms_campaign_id} | View Specific SMS Campaign



## CalculateSmsCampaignPrice

> CalculateSmsCampaignPrice CalculateSmsCampaignPrice(ctx).ContentType(contentType).CalculateSmsCampaignPriceRequest(calculateSmsCampaignPriceRequest).Execute()

Calculate SMS Campaign Price



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
	calculateSmsCampaignPriceRequest := *openapiclient.NewCalculateSmsCampaignPriceRequest() // CalculateSmsCampaignPriceRequest |  (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.SmsCampaignsAPI.CalculateSmsCampaignPrice(context.Background()).ContentType(contentType).CalculateSmsCampaignPriceRequest(calculateSmsCampaignPriceRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `SmsCampaignsAPI.CalculateSmsCampaignPrice``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `CalculateSmsCampaignPrice`: CalculateSmsCampaignPrice
	fmt.Fprintf(os.Stdout, "Response from `SmsCampaignsAPI.CalculateSmsCampaignPrice`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiCalculateSmsCampaignPriceRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **contentType** | **string** |  | 
 **calculateSmsCampaignPriceRequest** | [**CalculateSmsCampaignPriceRequest**](CalculateSmsCampaignPriceRequest.md) |  | 

### Return type

[**CalculateSmsCampaignPrice**](CalculateSmsCampaignPrice.md)

### Authorization

[basicAuth](../README.md#basicAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## CancelSmsCampaign

> CancelSmsCampaign CancelSmsCampaign(ctx, smsCampaignId).ContentType(contentType).Execute()

Cancel SMS Campaign



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
	smsCampaignId := "smsCampaignId_example" // string | ID of the scheduled SMS campaign to cancel.
	contentType := "application/json" // string |  (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.SmsCampaignsAPI.CancelSmsCampaign(context.Background(), smsCampaignId).ContentType(contentType).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `SmsCampaignsAPI.CancelSmsCampaign``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `CancelSmsCampaign`: CancelSmsCampaign
	fmt.Fprintf(os.Stdout, "Response from `SmsCampaignsAPI.CancelSmsCampaign`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**smsCampaignId** | **string** | ID of the scheduled SMS campaign to cancel. | 

### Other Parameters

Other parameters are passed through a pointer to a apiCancelSmsCampaignRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **contentType** | **string** |  | 

### Return type

[**CancelSmsCampaign**](CancelSmsCampaign.md)

### Authorization

[basicAuth](../README.md#basicAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## SendSmsCampaign

> SendSmsCampaign SendSmsCampaign(ctx).ContentType(contentType).SendSmsCampaignRequest(sendSmsCampaignRequest).Execute()

Send SMS Campaign



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
	sendSmsCampaignRequest := *openapiclient.NewSendSmsCampaignRequest(int32(1), "My Campaign", "From_example", "Body_example", []openapiclient.SendersInner{*openapiclient.NewSendersInner("RecipientCountryCode_example")}) // SendSmsCampaignRequest |  (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.SmsCampaignsAPI.SendSmsCampaign(context.Background()).ContentType(contentType).SendSmsCampaignRequest(sendSmsCampaignRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `SmsCampaignsAPI.SendSmsCampaign``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `SendSmsCampaign`: SendSmsCampaign
	fmt.Fprintf(os.Stdout, "Response from `SmsCampaignsAPI.SendSmsCampaign`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiSendSmsCampaignRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **contentType** | **string** |  | 
 **sendSmsCampaignRequest** | [**SendSmsCampaignRequest**](SendSmsCampaignRequest.md) |  | 

### Return type

[**SendSmsCampaign**](SendSmsCampaign.md)

### Authorization

[basicAuth](../README.md#basicAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## UpdateSmsCampaign

> UpdateSmsCampaign UpdateSmsCampaign(ctx, smsCampaignId).ContentType(contentType).CalculateSmsCampaignPriceRequest(calculateSmsCampaignPriceRequest).Execute()

Update SMS Campaign



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
	smsCampaignId := "smsCampaignId_example" // string | 
	contentType := "application/json" // string |  (optional)
	calculateSmsCampaignPriceRequest := *openapiclient.NewCalculateSmsCampaignPriceRequest() // CalculateSmsCampaignPriceRequest |  (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.SmsCampaignsAPI.UpdateSmsCampaign(context.Background(), smsCampaignId).ContentType(contentType).CalculateSmsCampaignPriceRequest(calculateSmsCampaignPriceRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `SmsCampaignsAPI.UpdateSmsCampaign``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `UpdateSmsCampaign`: UpdateSmsCampaign
	fmt.Fprintf(os.Stdout, "Response from `SmsCampaignsAPI.UpdateSmsCampaign`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**smsCampaignId** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiUpdateSmsCampaignRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **contentType** | **string** |  | 
 **calculateSmsCampaignPriceRequest** | [**CalculateSmsCampaignPriceRequest**](CalculateSmsCampaignPriceRequest.md) |  | 

### Return type

[**UpdateSmsCampaign**](UpdateSmsCampaign.md)

### Authorization

[basicAuth](../README.md#basicAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## ViewSmsCampaigns

> ViewSmsCampaigns ViewSmsCampaigns(ctx).ContentType(contentType).Page(page).Limit(limit).Q(q).OrderBy(orderBy).DateFrom(dateFrom).DateTo(dateTo).Execute()

View SMS Campaigns



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
	page := int32(1) // int32 | The page number to retrieve. Use this parameter to navigate through the [pagination]/#pagination) results. The default value is 1. (optional) (default to 1)
	limit := int32(56) // int32 | The number of items to return per page. This parameter controls the size of each page of results. The default value is 15. (optional) (default to 15)
	q := "q_example" // string | Allows filtering of results based on your search criteria. The query should be in the format `field_name:value`.  1. **Field Name**: The field within the SMS campaign you want to filter by. You can use the following fields:      - sms_campaign_id,name,user_id,subaccount_id,list_id,from,body,schedule,status,date_added,custom_string,url_to_shorten,unsubscribe_link,source   2. **Value**: The text or keyword you're searching for within the specified field. If left empty after the colon, the filter will look for all templates with any value in the **Field Name**.  For example, if you are searching for a SMS campaign with the status of _Scheduled_, the final query would look like this:    - `q=status:Scheduled`  <div class=\"info-box\">   <h4><i class=\"fas fa-info-circle\"></i> Note:</h4>   <p>   Some characters have to be encoded. For example, if you are searching for SMS sent from the phone number +61437085284, your search query q would be:<br/>    <ul>     <li>q=from:%2B61437085284</li>   </ul>    You can use the <a href=\"https://www.urlencoder.org/\" target=\"_blank\">URL encoder</a> to encode the text. If a character is not an alphanumeric character (A-Z, a-z, 0-9), it is typically either reserved or unsafe and should be encoded.      </p> </div> (optional)
	orderBy := "orderBy_example" // string | Specifies the field and order to sort the results by. The value is composed of the field name followed by a colon and the sort direction (_asc_ for ascending or _desc_ for descending).  The default sort order is by _date_added_ in ascending order. You can use the following fields:    - _name_: The name of the SMS campaign.   - _status_: The status of the SMS campaign.   - _schedule_: The schedule send date of the SMS campaign in the <a href=\"http://help.clicksend.com/what-is-a-unix-timestamp\" target=\"_blank\">Unix format</a>.   - _from_: The sender of the SMS campaign.   - _date_added_: This is the date you created or updated the SMS campaign in the <a href=\"http://help.clicksend.com/what-is-a-unix-timestamp\" target=\"_blank\">Unix format</a>.  For example, if you want to order by the most recently sent or scheduled SMS, you should sort by date in descending order. The query would look like this:    - `order_by=schedule:desc`  <div class=\"info-box\">   <h4><i class=\"fas fa-info-circle\"></i> Note:</h4>   <p>     You can also sort by these fields: <br/>     <ul>     <li>sms_campaign_id,user_id,subaccount_id,list_id,body,custom_string,url_to_shorten,unsubscribe_link, and source.</li>   </ul>   <br/>   But this is less common in practice.   </p> </div> (optional)
	dateFrom := int32(56) // int32 | Start date to filter results. It should be in <a href=\"http://help.clicksend.com/what-is-a-unix-timestamp\" target=\"_blank\">Unix format</a>. (optional)
	dateTo := int32(56) // int32 | End date to filter results. It should be in <a href=\"http://help.clicksend.com/what-is-a-unix-timestamp\" target=\"_blank\">Unix format</a>. (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.SmsCampaignsAPI.ViewSmsCampaigns(context.Background()).ContentType(contentType).Page(page).Limit(limit).Q(q).OrderBy(orderBy).DateFrom(dateFrom).DateTo(dateTo).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `SmsCampaignsAPI.ViewSmsCampaigns``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ViewSmsCampaigns`: ViewSmsCampaigns
	fmt.Fprintf(os.Stdout, "Response from `SmsCampaignsAPI.ViewSmsCampaigns`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiViewSmsCampaignsRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **contentType** | **string** |  | 
 **page** | **int32** | The page number to retrieve. Use this parameter to navigate through the [pagination]/#pagination) results. The default value is 1. | [default to 1]
 **limit** | **int32** | The number of items to return per page. This parameter controls the size of each page of results. The default value is 15. | [default to 15]
 **q** | **string** | Allows filtering of results based on your search criteria. The query should be in the format &#x60;field_name:value&#x60;.  1. **Field Name**: The field within the SMS campaign you want to filter by. You can use the following fields:      - sms_campaign_id,name,user_id,subaccount_id,list_id,from,body,schedule,status,date_added,custom_string,url_to_shorten,unsubscribe_link,source   2. **Value**: The text or keyword you&#39;re searching for within the specified field. If left empty after the colon, the filter will look for all templates with any value in the **Field Name**.  For example, if you are searching for a SMS campaign with the status of _Scheduled_, the final query would look like this:    - &#x60;q&#x3D;status:Scheduled&#x60;  &lt;div class&#x3D;\&quot;info-box\&quot;&gt;   &lt;h4&gt;&lt;i class&#x3D;\&quot;fas fa-info-circle\&quot;&gt;&lt;/i&gt; Note:&lt;/h4&gt;   &lt;p&gt;   Some characters have to be encoded. For example, if you are searching for SMS sent from the phone number +61437085284, your search query q would be:&lt;br/&gt;    &lt;ul&gt;     &lt;li&gt;q&#x3D;from:%2B61437085284&lt;/li&gt;   &lt;/ul&gt;    You can use the &lt;a href&#x3D;\&quot;https://www.urlencoder.org/\&quot; target&#x3D;\&quot;_blank\&quot;&gt;URL encoder&lt;/a&gt; to encode the text. If a character is not an alphanumeric character (A-Z, a-z, 0-9), it is typically either reserved or unsafe and should be encoded.      &lt;/p&gt; &lt;/div&gt; | 
 **orderBy** | **string** | Specifies the field and order to sort the results by. The value is composed of the field name followed by a colon and the sort direction (_asc_ for ascending or _desc_ for descending).  The default sort order is by _date_added_ in ascending order. You can use the following fields:    - _name_: The name of the SMS campaign.   - _status_: The status of the SMS campaign.   - _schedule_: The schedule send date of the SMS campaign in the &lt;a href&#x3D;\&quot;http://help.clicksend.com/what-is-a-unix-timestamp\&quot; target&#x3D;\&quot;_blank\&quot;&gt;Unix format&lt;/a&gt;.   - _from_: The sender of the SMS campaign.   - _date_added_: This is the date you created or updated the SMS campaign in the &lt;a href&#x3D;\&quot;http://help.clicksend.com/what-is-a-unix-timestamp\&quot; target&#x3D;\&quot;_blank\&quot;&gt;Unix format&lt;/a&gt;.  For example, if you want to order by the most recently sent or scheduled SMS, you should sort by date in descending order. The query would look like this:    - &#x60;order_by&#x3D;schedule:desc&#x60;  &lt;div class&#x3D;\&quot;info-box\&quot;&gt;   &lt;h4&gt;&lt;i class&#x3D;\&quot;fas fa-info-circle\&quot;&gt;&lt;/i&gt; Note:&lt;/h4&gt;   &lt;p&gt;     You can also sort by these fields: &lt;br/&gt;     &lt;ul&gt;     &lt;li&gt;sms_campaign_id,user_id,subaccount_id,list_id,body,custom_string,url_to_shorten,unsubscribe_link, and source.&lt;/li&gt;   &lt;/ul&gt;   &lt;br/&gt;   But this is less common in practice.   &lt;/p&gt; &lt;/div&gt; | 
 **dateFrom** | **int32** | Start date to filter results. It should be in &lt;a href&#x3D;\&quot;http://help.clicksend.com/what-is-a-unix-timestamp\&quot; target&#x3D;\&quot;_blank\&quot;&gt;Unix format&lt;/a&gt;. | 
 **dateTo** | **int32** | End date to filter results. It should be in &lt;a href&#x3D;\&quot;http://help.clicksend.com/what-is-a-unix-timestamp\&quot; target&#x3D;\&quot;_blank\&quot;&gt;Unix format&lt;/a&gt;. | 

### Return type

[**ViewSmsCampaigns**](ViewSmsCampaigns.md)

### Authorization

[basicAuth](../README.md#basicAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## ViewSpecificSmsCampaign

> ViewSpecificSmsCampaign ViewSpecificSmsCampaign(ctx, smsCampaignId).ContentType(contentType).Execute()

View Specific SMS Campaign



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
	smsCampaignId := "smsCampaignId_example" // string | ID of SMS campaign to get
	contentType := "application/json" // string |  (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.SmsCampaignsAPI.ViewSpecificSmsCampaign(context.Background(), smsCampaignId).ContentType(contentType).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `SmsCampaignsAPI.ViewSpecificSmsCampaign``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ViewSpecificSmsCampaign`: ViewSpecificSmsCampaign
	fmt.Fprintf(os.Stdout, "Response from `SmsCampaignsAPI.ViewSpecificSmsCampaign`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**smsCampaignId** | **string** | ID of SMS campaign to get | 

### Other Parameters

Other parameters are passed through a pointer to a apiViewSpecificSmsCampaignRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **contentType** | **string** |  | 

### Return type

[**ViewSpecificSmsCampaign**](ViewSpecificSmsCampaign.md)

### Authorization

[basicAuth](../README.md#basicAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)

