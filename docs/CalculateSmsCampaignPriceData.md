# CalculateSmsCampaignPriceData

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**TotalCount** | Pointer to **int32** | The total number of records. | [optional] 
**TotalPrice** | Pointer to **string** | The total price of the SMS campaign. | [optional] 
**Data** | Pointer to [**CalculateSmsCampaignPriceDataData**](CalculateSmsCampaignPriceDataData.md) |  | [optional] 
**Currency** | Pointer to [**Currency**](Currency.md) |  | [optional] 

## Methods

### NewCalculateSmsCampaignPriceData

`func NewCalculateSmsCampaignPriceData() *CalculateSmsCampaignPriceData`

NewCalculateSmsCampaignPriceData instantiates a new CalculateSmsCampaignPriceData object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewCalculateSmsCampaignPriceDataWithDefaults

`func NewCalculateSmsCampaignPriceDataWithDefaults() *CalculateSmsCampaignPriceData`

NewCalculateSmsCampaignPriceDataWithDefaults instantiates a new CalculateSmsCampaignPriceData object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetTotalCount

`func (o *CalculateSmsCampaignPriceData) GetTotalCount() int32`

GetTotalCount returns the TotalCount field if non-nil, zero value otherwise.

### GetTotalCountOk

`func (o *CalculateSmsCampaignPriceData) GetTotalCountOk() (*int32, bool)`

GetTotalCountOk returns a tuple with the TotalCount field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTotalCount

`func (o *CalculateSmsCampaignPriceData) SetTotalCount(v int32)`

SetTotalCount sets TotalCount field to given value.

### HasTotalCount

`func (o *CalculateSmsCampaignPriceData) HasTotalCount() bool`

HasTotalCount returns a boolean if a field has been set.

### GetTotalPrice

`func (o *CalculateSmsCampaignPriceData) GetTotalPrice() string`

GetTotalPrice returns the TotalPrice field if non-nil, zero value otherwise.

### GetTotalPriceOk

`func (o *CalculateSmsCampaignPriceData) GetTotalPriceOk() (*string, bool)`

GetTotalPriceOk returns a tuple with the TotalPrice field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTotalPrice

`func (o *CalculateSmsCampaignPriceData) SetTotalPrice(v string)`

SetTotalPrice sets TotalPrice field to given value.

### HasTotalPrice

`func (o *CalculateSmsCampaignPriceData) HasTotalPrice() bool`

HasTotalPrice returns a boolean if a field has been set.

### GetData

`func (o *CalculateSmsCampaignPriceData) GetData() CalculateSmsCampaignPriceDataData`

GetData returns the Data field if non-nil, zero value otherwise.

### GetDataOk

`func (o *CalculateSmsCampaignPriceData) GetDataOk() (*CalculateSmsCampaignPriceDataData, bool)`

GetDataOk returns a tuple with the Data field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetData

`func (o *CalculateSmsCampaignPriceData) SetData(v CalculateSmsCampaignPriceDataData)`

SetData sets Data field to given value.

### HasData

`func (o *CalculateSmsCampaignPriceData) HasData() bool`

HasData returns a boolean if a field has been set.

### GetCurrency

`func (o *CalculateSmsCampaignPriceData) GetCurrency() Currency`

GetCurrency returns the Currency field if non-nil, zero value otherwise.

### GetCurrencyOk

`func (o *CalculateSmsCampaignPriceData) GetCurrencyOk() (*Currency, bool)`

GetCurrencyOk returns a tuple with the Currency field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCurrency

`func (o *CalculateSmsCampaignPriceData) SetCurrency(v Currency)`

SetCurrency sets Currency field to given value.

### HasCurrency

`func (o *CalculateSmsCampaignPriceData) HasCurrency() bool`

HasCurrency returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


