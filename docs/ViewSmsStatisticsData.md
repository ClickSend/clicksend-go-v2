# ViewSmsStatisticsData

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Total** | Pointer to [**ViewSmsStatisticsDataTotal**](ViewSmsStatisticsDataTotal.md) |  | [optional] 
**Stat** | Pointer to [**[]ViewSmsStatisticsDataStatInner**](ViewSmsStatisticsDataStatInner.md) |  | [optional] 
**Currency** | Pointer to [**Currency**](Currency.md) |  | [optional] 

## Methods

### NewViewSmsStatisticsData

`func NewViewSmsStatisticsData() *ViewSmsStatisticsData`

NewViewSmsStatisticsData instantiates a new ViewSmsStatisticsData object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewViewSmsStatisticsDataWithDefaults

`func NewViewSmsStatisticsDataWithDefaults() *ViewSmsStatisticsData`

NewViewSmsStatisticsDataWithDefaults instantiates a new ViewSmsStatisticsData object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetTotal

`func (o *ViewSmsStatisticsData) GetTotal() ViewSmsStatisticsDataTotal`

GetTotal returns the Total field if non-nil, zero value otherwise.

### GetTotalOk

`func (o *ViewSmsStatisticsData) GetTotalOk() (*ViewSmsStatisticsDataTotal, bool)`

GetTotalOk returns a tuple with the Total field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTotal

`func (o *ViewSmsStatisticsData) SetTotal(v ViewSmsStatisticsDataTotal)`

SetTotal sets Total field to given value.

### HasTotal

`func (o *ViewSmsStatisticsData) HasTotal() bool`

HasTotal returns a boolean if a field has been set.

### GetStat

`func (o *ViewSmsStatisticsData) GetStat() []ViewSmsStatisticsDataStatInner`

GetStat returns the Stat field if non-nil, zero value otherwise.

### GetStatOk

`func (o *ViewSmsStatisticsData) GetStatOk() (*[]ViewSmsStatisticsDataStatInner, bool)`

GetStatOk returns a tuple with the Stat field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetStat

`func (o *ViewSmsStatisticsData) SetStat(v []ViewSmsStatisticsDataStatInner)`

SetStat sets Stat field to given value.

### HasStat

`func (o *ViewSmsStatisticsData) HasStat() bool`

HasStat returns a boolean if a field has been set.

### GetCurrency

`func (o *ViewSmsStatisticsData) GetCurrency() Currency`

GetCurrency returns the Currency field if non-nil, zero value otherwise.

### GetCurrencyOk

`func (o *ViewSmsStatisticsData) GetCurrencyOk() (*Currency, bool)`

GetCurrencyOk returns a tuple with the Currency field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCurrency

`func (o *ViewSmsStatisticsData) SetCurrency(v Currency)`

SetCurrency sets Currency field to given value.

### HasCurrency

`func (o *ViewSmsStatisticsData) HasCurrency() bool`

HasCurrency returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


