# ViewYourNumbersData

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Total** | Pointer to **int32** | The total number of items available for viewing. | [optional] 
**PerPage** | Pointer to **int32** | The number of items returned per page. This is specified in the limit parameter. You can have 100 items at maximum, and 15 at minimum. | [optional] 
**CurrentPage** | Pointer to **int32** | The current page number. | [optional] 
**LastPage** | Pointer to **int32** | The last page number. | [optional] 
**NextPageUrl** | Pointer to **NullableString** | A URL of the next page. It will return **null** if there’s no next page. | [optional] 
**PrevPageUrl** | Pointer to **NullableString** | A URL of the previous page. It will return **null** if there’s no previous page. | [optional] 
**From** | Pointer to **int32** | The number of the first result in the current page. | [optional] 
**To** | Pointer to **int32** | The number of the last result in the current page. | [optional] 
**Data** | Pointer to [**[]ViewYourNumbersDataAllOfDataInner**](ViewYourNumbersDataAllOfDataInner.md) |  | [optional] 
**Currency** | Pointer to [**Currency**](Currency.md) |  | [optional] 

## Methods

### NewViewYourNumbersData

`func NewViewYourNumbersData() *ViewYourNumbersData`

NewViewYourNumbersData instantiates a new ViewYourNumbersData object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewViewYourNumbersDataWithDefaults

`func NewViewYourNumbersDataWithDefaults() *ViewYourNumbersData`

NewViewYourNumbersDataWithDefaults instantiates a new ViewYourNumbersData object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetTotal

`func (o *ViewYourNumbersData) GetTotal() int32`

GetTotal returns the Total field if non-nil, zero value otherwise.

### GetTotalOk

`func (o *ViewYourNumbersData) GetTotalOk() (*int32, bool)`

GetTotalOk returns a tuple with the Total field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTotal

`func (o *ViewYourNumbersData) SetTotal(v int32)`

SetTotal sets Total field to given value.

### HasTotal

`func (o *ViewYourNumbersData) HasTotal() bool`

HasTotal returns a boolean if a field has been set.

### GetPerPage

`func (o *ViewYourNumbersData) GetPerPage() int32`

GetPerPage returns the PerPage field if non-nil, zero value otherwise.

### GetPerPageOk

`func (o *ViewYourNumbersData) GetPerPageOk() (*int32, bool)`

GetPerPageOk returns a tuple with the PerPage field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetPerPage

`func (o *ViewYourNumbersData) SetPerPage(v int32)`

SetPerPage sets PerPage field to given value.

### HasPerPage

`func (o *ViewYourNumbersData) HasPerPage() bool`

HasPerPage returns a boolean if a field has been set.

### GetCurrentPage

`func (o *ViewYourNumbersData) GetCurrentPage() int32`

GetCurrentPage returns the CurrentPage field if non-nil, zero value otherwise.

### GetCurrentPageOk

`func (o *ViewYourNumbersData) GetCurrentPageOk() (*int32, bool)`

GetCurrentPageOk returns a tuple with the CurrentPage field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCurrentPage

`func (o *ViewYourNumbersData) SetCurrentPage(v int32)`

SetCurrentPage sets CurrentPage field to given value.

### HasCurrentPage

`func (o *ViewYourNumbersData) HasCurrentPage() bool`

HasCurrentPage returns a boolean if a field has been set.

### GetLastPage

`func (o *ViewYourNumbersData) GetLastPage() int32`

GetLastPage returns the LastPage field if non-nil, zero value otherwise.

### GetLastPageOk

`func (o *ViewYourNumbersData) GetLastPageOk() (*int32, bool)`

GetLastPageOk returns a tuple with the LastPage field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetLastPage

`func (o *ViewYourNumbersData) SetLastPage(v int32)`

SetLastPage sets LastPage field to given value.

### HasLastPage

`func (o *ViewYourNumbersData) HasLastPage() bool`

HasLastPage returns a boolean if a field has been set.

### GetNextPageUrl

`func (o *ViewYourNumbersData) GetNextPageUrl() string`

GetNextPageUrl returns the NextPageUrl field if non-nil, zero value otherwise.

### GetNextPageUrlOk

`func (o *ViewYourNumbersData) GetNextPageUrlOk() (*string, bool)`

GetNextPageUrlOk returns a tuple with the NextPageUrl field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetNextPageUrl

`func (o *ViewYourNumbersData) SetNextPageUrl(v string)`

SetNextPageUrl sets NextPageUrl field to given value.

### HasNextPageUrl

`func (o *ViewYourNumbersData) HasNextPageUrl() bool`

HasNextPageUrl returns a boolean if a field has been set.

### SetNextPageUrlNil

`func (o *ViewYourNumbersData) SetNextPageUrlNil(b bool)`

 SetNextPageUrlNil sets the value for NextPageUrl to be an explicit nil

### UnsetNextPageUrl
`func (o *ViewYourNumbersData) UnsetNextPageUrl()`

UnsetNextPageUrl ensures that no value is present for NextPageUrl, not even an explicit nil
### GetPrevPageUrl

`func (o *ViewYourNumbersData) GetPrevPageUrl() string`

GetPrevPageUrl returns the PrevPageUrl field if non-nil, zero value otherwise.

### GetPrevPageUrlOk

`func (o *ViewYourNumbersData) GetPrevPageUrlOk() (*string, bool)`

GetPrevPageUrlOk returns a tuple with the PrevPageUrl field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetPrevPageUrl

`func (o *ViewYourNumbersData) SetPrevPageUrl(v string)`

SetPrevPageUrl sets PrevPageUrl field to given value.

### HasPrevPageUrl

`func (o *ViewYourNumbersData) HasPrevPageUrl() bool`

HasPrevPageUrl returns a boolean if a field has been set.

### SetPrevPageUrlNil

`func (o *ViewYourNumbersData) SetPrevPageUrlNil(b bool)`

 SetPrevPageUrlNil sets the value for PrevPageUrl to be an explicit nil

### UnsetPrevPageUrl
`func (o *ViewYourNumbersData) UnsetPrevPageUrl()`

UnsetPrevPageUrl ensures that no value is present for PrevPageUrl, not even an explicit nil
### GetFrom

`func (o *ViewYourNumbersData) GetFrom() int32`

GetFrom returns the From field if non-nil, zero value otherwise.

### GetFromOk

`func (o *ViewYourNumbersData) GetFromOk() (*int32, bool)`

GetFromOk returns a tuple with the From field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetFrom

`func (o *ViewYourNumbersData) SetFrom(v int32)`

SetFrom sets From field to given value.

### HasFrom

`func (o *ViewYourNumbersData) HasFrom() bool`

HasFrom returns a boolean if a field has been set.

### GetTo

`func (o *ViewYourNumbersData) GetTo() int32`

GetTo returns the To field if non-nil, zero value otherwise.

### GetToOk

`func (o *ViewYourNumbersData) GetToOk() (*int32, bool)`

GetToOk returns a tuple with the To field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTo

`func (o *ViewYourNumbersData) SetTo(v int32)`

SetTo sets To field to given value.

### HasTo

`func (o *ViewYourNumbersData) HasTo() bool`

HasTo returns a boolean if a field has been set.

### GetData

`func (o *ViewYourNumbersData) GetData() []ViewYourNumbersDataAllOfDataInner`

GetData returns the Data field if non-nil, zero value otherwise.

### GetDataOk

`func (o *ViewYourNumbersData) GetDataOk() (*[]ViewYourNumbersDataAllOfDataInner, bool)`

GetDataOk returns a tuple with the Data field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetData

`func (o *ViewYourNumbersData) SetData(v []ViewYourNumbersDataAllOfDataInner)`

SetData sets Data field to given value.

### HasData

`func (o *ViewYourNumbersData) HasData() bool`

HasData returns a boolean if a field has been set.

### GetCurrency

`func (o *ViewYourNumbersData) GetCurrency() Currency`

GetCurrency returns the Currency field if non-nil, zero value otherwise.

### GetCurrencyOk

`func (o *ViewYourNumbersData) GetCurrencyOk() (*Currency, bool)`

GetCurrencyOk returns a tuple with the Currency field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCurrency

`func (o *ViewYourNumbersData) SetCurrency(v Currency)`

SetCurrency sets Currency field to given value.

### HasCurrency

`func (o *ViewYourNumbersData) HasCurrency() bool`

HasCurrency returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


