# SendEmailCampaignData

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**TotlalCount** | Pointer to **float32** | The total count of the email campaigns. | [optional] 
**TotalPrice** | Pointer to **string** | The total price of the email campaigns. | [optional] 
**QueuedCount** | Pointer to **float32** | The count of the queued email campaigns. | [optional] 
**Data** | Pointer to [**EmailCampaign**](EmailCampaign.md) |  | [optional] 
**Currency** | Pointer to [**Currency**](Currency.md) |  | [optional] 

## Methods

### NewSendEmailCampaignData

`func NewSendEmailCampaignData() *SendEmailCampaignData`

NewSendEmailCampaignData instantiates a new SendEmailCampaignData object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewSendEmailCampaignDataWithDefaults

`func NewSendEmailCampaignDataWithDefaults() *SendEmailCampaignData`

NewSendEmailCampaignDataWithDefaults instantiates a new SendEmailCampaignData object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetTotlalCount

`func (o *SendEmailCampaignData) GetTotlalCount() float32`

GetTotlalCount returns the TotlalCount field if non-nil, zero value otherwise.

### GetTotlalCountOk

`func (o *SendEmailCampaignData) GetTotlalCountOk() (*float32, bool)`

GetTotlalCountOk returns a tuple with the TotlalCount field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTotlalCount

`func (o *SendEmailCampaignData) SetTotlalCount(v float32)`

SetTotlalCount sets TotlalCount field to given value.

### HasTotlalCount

`func (o *SendEmailCampaignData) HasTotlalCount() bool`

HasTotlalCount returns a boolean if a field has been set.

### GetTotalPrice

`func (o *SendEmailCampaignData) GetTotalPrice() string`

GetTotalPrice returns the TotalPrice field if non-nil, zero value otherwise.

### GetTotalPriceOk

`func (o *SendEmailCampaignData) GetTotalPriceOk() (*string, bool)`

GetTotalPriceOk returns a tuple with the TotalPrice field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTotalPrice

`func (o *SendEmailCampaignData) SetTotalPrice(v string)`

SetTotalPrice sets TotalPrice field to given value.

### HasTotalPrice

`func (o *SendEmailCampaignData) HasTotalPrice() bool`

HasTotalPrice returns a boolean if a field has been set.

### GetQueuedCount

`func (o *SendEmailCampaignData) GetQueuedCount() float32`

GetQueuedCount returns the QueuedCount field if non-nil, zero value otherwise.

### GetQueuedCountOk

`func (o *SendEmailCampaignData) GetQueuedCountOk() (*float32, bool)`

GetQueuedCountOk returns a tuple with the QueuedCount field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetQueuedCount

`func (o *SendEmailCampaignData) SetQueuedCount(v float32)`

SetQueuedCount sets QueuedCount field to given value.

### HasQueuedCount

`func (o *SendEmailCampaignData) HasQueuedCount() bool`

HasQueuedCount returns a boolean if a field has been set.

### GetData

`func (o *SendEmailCampaignData) GetData() EmailCampaign`

GetData returns the Data field if non-nil, zero value otherwise.

### GetDataOk

`func (o *SendEmailCampaignData) GetDataOk() (*EmailCampaign, bool)`

GetDataOk returns a tuple with the Data field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetData

`func (o *SendEmailCampaignData) SetData(v EmailCampaign)`

SetData sets Data field to given value.

### HasData

`func (o *SendEmailCampaignData) HasData() bool`

HasData returns a boolean if a field has been set.

### GetCurrency

`func (o *SendEmailCampaignData) GetCurrency() Currency`

GetCurrency returns the Currency field if non-nil, zero value otherwise.

### GetCurrencyOk

`func (o *SendEmailCampaignData) GetCurrencyOk() (*Currency, bool)`

GetCurrencyOk returns a tuple with the Currency field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCurrency

`func (o *SendEmailCampaignData) SetCurrency(v Currency)`

SetCurrency sets Currency field to given value.

### HasCurrency

`func (o *SendEmailCampaignData) HasCurrency() bool`

HasCurrency returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


