# ViewAllowedEmailsData

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
**Data** | Pointer to [**[]ViewAllowedEmailsDataAllOfDataInner**](ViewAllowedEmailsDataAllOfDataInner.md) |  | [optional] 

## Methods

### NewViewAllowedEmailsData

`func NewViewAllowedEmailsData() *ViewAllowedEmailsData`

NewViewAllowedEmailsData instantiates a new ViewAllowedEmailsData object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewViewAllowedEmailsDataWithDefaults

`func NewViewAllowedEmailsDataWithDefaults() *ViewAllowedEmailsData`

NewViewAllowedEmailsDataWithDefaults instantiates a new ViewAllowedEmailsData object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetTotal

`func (o *ViewAllowedEmailsData) GetTotal() int32`

GetTotal returns the Total field if non-nil, zero value otherwise.

### GetTotalOk

`func (o *ViewAllowedEmailsData) GetTotalOk() (*int32, bool)`

GetTotalOk returns a tuple with the Total field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTotal

`func (o *ViewAllowedEmailsData) SetTotal(v int32)`

SetTotal sets Total field to given value.

### HasTotal

`func (o *ViewAllowedEmailsData) HasTotal() bool`

HasTotal returns a boolean if a field has been set.

### GetPerPage

`func (o *ViewAllowedEmailsData) GetPerPage() int32`

GetPerPage returns the PerPage field if non-nil, zero value otherwise.

### GetPerPageOk

`func (o *ViewAllowedEmailsData) GetPerPageOk() (*int32, bool)`

GetPerPageOk returns a tuple with the PerPage field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetPerPage

`func (o *ViewAllowedEmailsData) SetPerPage(v int32)`

SetPerPage sets PerPage field to given value.

### HasPerPage

`func (o *ViewAllowedEmailsData) HasPerPage() bool`

HasPerPage returns a boolean if a field has been set.

### GetCurrentPage

`func (o *ViewAllowedEmailsData) GetCurrentPage() int32`

GetCurrentPage returns the CurrentPage field if non-nil, zero value otherwise.

### GetCurrentPageOk

`func (o *ViewAllowedEmailsData) GetCurrentPageOk() (*int32, bool)`

GetCurrentPageOk returns a tuple with the CurrentPage field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCurrentPage

`func (o *ViewAllowedEmailsData) SetCurrentPage(v int32)`

SetCurrentPage sets CurrentPage field to given value.

### HasCurrentPage

`func (o *ViewAllowedEmailsData) HasCurrentPage() bool`

HasCurrentPage returns a boolean if a field has been set.

### GetLastPage

`func (o *ViewAllowedEmailsData) GetLastPage() int32`

GetLastPage returns the LastPage field if non-nil, zero value otherwise.

### GetLastPageOk

`func (o *ViewAllowedEmailsData) GetLastPageOk() (*int32, bool)`

GetLastPageOk returns a tuple with the LastPage field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetLastPage

`func (o *ViewAllowedEmailsData) SetLastPage(v int32)`

SetLastPage sets LastPage field to given value.

### HasLastPage

`func (o *ViewAllowedEmailsData) HasLastPage() bool`

HasLastPage returns a boolean if a field has been set.

### GetNextPageUrl

`func (o *ViewAllowedEmailsData) GetNextPageUrl() string`

GetNextPageUrl returns the NextPageUrl field if non-nil, zero value otherwise.

### GetNextPageUrlOk

`func (o *ViewAllowedEmailsData) GetNextPageUrlOk() (*string, bool)`

GetNextPageUrlOk returns a tuple with the NextPageUrl field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetNextPageUrl

`func (o *ViewAllowedEmailsData) SetNextPageUrl(v string)`

SetNextPageUrl sets NextPageUrl field to given value.

### HasNextPageUrl

`func (o *ViewAllowedEmailsData) HasNextPageUrl() bool`

HasNextPageUrl returns a boolean if a field has been set.

### SetNextPageUrlNil

`func (o *ViewAllowedEmailsData) SetNextPageUrlNil(b bool)`

 SetNextPageUrlNil sets the value for NextPageUrl to be an explicit nil

### UnsetNextPageUrl
`func (o *ViewAllowedEmailsData) UnsetNextPageUrl()`

UnsetNextPageUrl ensures that no value is present for NextPageUrl, not even an explicit nil
### GetPrevPageUrl

`func (o *ViewAllowedEmailsData) GetPrevPageUrl() string`

GetPrevPageUrl returns the PrevPageUrl field if non-nil, zero value otherwise.

### GetPrevPageUrlOk

`func (o *ViewAllowedEmailsData) GetPrevPageUrlOk() (*string, bool)`

GetPrevPageUrlOk returns a tuple with the PrevPageUrl field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetPrevPageUrl

`func (o *ViewAllowedEmailsData) SetPrevPageUrl(v string)`

SetPrevPageUrl sets PrevPageUrl field to given value.

### HasPrevPageUrl

`func (o *ViewAllowedEmailsData) HasPrevPageUrl() bool`

HasPrevPageUrl returns a boolean if a field has been set.

### SetPrevPageUrlNil

`func (o *ViewAllowedEmailsData) SetPrevPageUrlNil(b bool)`

 SetPrevPageUrlNil sets the value for PrevPageUrl to be an explicit nil

### UnsetPrevPageUrl
`func (o *ViewAllowedEmailsData) UnsetPrevPageUrl()`

UnsetPrevPageUrl ensures that no value is present for PrevPageUrl, not even an explicit nil
### GetFrom

`func (o *ViewAllowedEmailsData) GetFrom() int32`

GetFrom returns the From field if non-nil, zero value otherwise.

### GetFromOk

`func (o *ViewAllowedEmailsData) GetFromOk() (*int32, bool)`

GetFromOk returns a tuple with the From field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetFrom

`func (o *ViewAllowedEmailsData) SetFrom(v int32)`

SetFrom sets From field to given value.

### HasFrom

`func (o *ViewAllowedEmailsData) HasFrom() bool`

HasFrom returns a boolean if a field has been set.

### GetTo

`func (o *ViewAllowedEmailsData) GetTo() int32`

GetTo returns the To field if non-nil, zero value otherwise.

### GetToOk

`func (o *ViewAllowedEmailsData) GetToOk() (*int32, bool)`

GetToOk returns a tuple with the To field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTo

`func (o *ViewAllowedEmailsData) SetTo(v int32)`

SetTo sets To field to given value.

### HasTo

`func (o *ViewAllowedEmailsData) HasTo() bool`

HasTo returns a boolean if a field has been set.

### GetData

`func (o *ViewAllowedEmailsData) GetData() []ViewAllowedEmailsDataAllOfDataInner`

GetData returns the Data field if non-nil, zero value otherwise.

### GetDataOk

`func (o *ViewAllowedEmailsData) GetDataOk() (*[]ViewAllowedEmailsDataAllOfDataInner, bool)`

GetDataOk returns a tuple with the Data field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetData

`func (o *ViewAllowedEmailsData) SetData(v []ViewAllowedEmailsDataAllOfDataInner)`

SetData sets Data field to given value.

### HasData

`func (o *ViewAllowedEmailsData) HasData() bool`

HasData returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


