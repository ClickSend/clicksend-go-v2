# ViewVoiceStatisticsData

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Total** | Pointer to [**ViewVoiceStatisticsDataTotal**](ViewVoiceStatisticsDataTotal.md) |  | [optional] 
**Stats** | Pointer to [**[]ViewVoiceStatisticsDataStatsInner**](ViewVoiceStatisticsDataStatsInner.md) |  | [optional] 
**Currency** | Pointer to [**Currency**](Currency.md) |  | [optional] 

## Methods

### NewViewVoiceStatisticsData

`func NewViewVoiceStatisticsData() *ViewVoiceStatisticsData`

NewViewVoiceStatisticsData instantiates a new ViewVoiceStatisticsData object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewViewVoiceStatisticsDataWithDefaults

`func NewViewVoiceStatisticsDataWithDefaults() *ViewVoiceStatisticsData`

NewViewVoiceStatisticsDataWithDefaults instantiates a new ViewVoiceStatisticsData object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetTotal

`func (o *ViewVoiceStatisticsData) GetTotal() ViewVoiceStatisticsDataTotal`

GetTotal returns the Total field if non-nil, zero value otherwise.

### GetTotalOk

`func (o *ViewVoiceStatisticsData) GetTotalOk() (*ViewVoiceStatisticsDataTotal, bool)`

GetTotalOk returns a tuple with the Total field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTotal

`func (o *ViewVoiceStatisticsData) SetTotal(v ViewVoiceStatisticsDataTotal)`

SetTotal sets Total field to given value.

### HasTotal

`func (o *ViewVoiceStatisticsData) HasTotal() bool`

HasTotal returns a boolean if a field has been set.

### GetStats

`func (o *ViewVoiceStatisticsData) GetStats() []ViewVoiceStatisticsDataStatsInner`

GetStats returns the Stats field if non-nil, zero value otherwise.

### GetStatsOk

`func (o *ViewVoiceStatisticsData) GetStatsOk() (*[]ViewVoiceStatisticsDataStatsInner, bool)`

GetStatsOk returns a tuple with the Stats field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetStats

`func (o *ViewVoiceStatisticsData) SetStats(v []ViewVoiceStatisticsDataStatsInner)`

SetStats sets Stats field to given value.

### HasStats

`func (o *ViewVoiceStatisticsData) HasStats() bool`

HasStats returns a boolean if a field has been set.

### GetCurrency

`func (o *ViewVoiceStatisticsData) GetCurrency() Currency`

GetCurrency returns the Currency field if non-nil, zero value otherwise.

### GetCurrencyOk

`func (o *ViewVoiceStatisticsData) GetCurrencyOk() (*Currency, bool)`

GetCurrencyOk returns a tuple with the Currency field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCurrency

`func (o *ViewVoiceStatisticsData) SetCurrency(v Currency)`

SetCurrency sets Currency field to given value.

### HasCurrency

`func (o *ViewVoiceStatisticsData) HasCurrency() bool`

HasCurrency returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


