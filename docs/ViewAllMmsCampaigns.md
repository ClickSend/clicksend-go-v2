# ViewAllMmsCampaigns

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
**Data** | Pointer to [**[]MmsCampaign**](MmsCampaign.md) |  | [optional] 

## Methods

### NewViewAllMmsCampaigns

`func NewViewAllMmsCampaigns() *ViewAllMmsCampaigns`

NewViewAllMmsCampaigns instantiates a new ViewAllMmsCampaigns object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewViewAllMmsCampaignsWithDefaults

`func NewViewAllMmsCampaignsWithDefaults() *ViewAllMmsCampaigns`

NewViewAllMmsCampaignsWithDefaults instantiates a new ViewAllMmsCampaigns object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetTotal

`func (o *ViewAllMmsCampaigns) GetTotal() int32`

GetTotal returns the Total field if non-nil, zero value otherwise.

### GetTotalOk

`func (o *ViewAllMmsCampaigns) GetTotalOk() (*int32, bool)`

GetTotalOk returns a tuple with the Total field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTotal

`func (o *ViewAllMmsCampaigns) SetTotal(v int32)`

SetTotal sets Total field to given value.

### HasTotal

`func (o *ViewAllMmsCampaigns) HasTotal() bool`

HasTotal returns a boolean if a field has been set.

### GetPerPage

`func (o *ViewAllMmsCampaigns) GetPerPage() int32`

GetPerPage returns the PerPage field if non-nil, zero value otherwise.

### GetPerPageOk

`func (o *ViewAllMmsCampaigns) GetPerPageOk() (*int32, bool)`

GetPerPageOk returns a tuple with the PerPage field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetPerPage

`func (o *ViewAllMmsCampaigns) SetPerPage(v int32)`

SetPerPage sets PerPage field to given value.

### HasPerPage

`func (o *ViewAllMmsCampaigns) HasPerPage() bool`

HasPerPage returns a boolean if a field has been set.

### GetCurrentPage

`func (o *ViewAllMmsCampaigns) GetCurrentPage() int32`

GetCurrentPage returns the CurrentPage field if non-nil, zero value otherwise.

### GetCurrentPageOk

`func (o *ViewAllMmsCampaigns) GetCurrentPageOk() (*int32, bool)`

GetCurrentPageOk returns a tuple with the CurrentPage field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCurrentPage

`func (o *ViewAllMmsCampaigns) SetCurrentPage(v int32)`

SetCurrentPage sets CurrentPage field to given value.

### HasCurrentPage

`func (o *ViewAllMmsCampaigns) HasCurrentPage() bool`

HasCurrentPage returns a boolean if a field has been set.

### GetLastPage

`func (o *ViewAllMmsCampaigns) GetLastPage() int32`

GetLastPage returns the LastPage field if non-nil, zero value otherwise.

### GetLastPageOk

`func (o *ViewAllMmsCampaigns) GetLastPageOk() (*int32, bool)`

GetLastPageOk returns a tuple with the LastPage field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetLastPage

`func (o *ViewAllMmsCampaigns) SetLastPage(v int32)`

SetLastPage sets LastPage field to given value.

### HasLastPage

`func (o *ViewAllMmsCampaigns) HasLastPage() bool`

HasLastPage returns a boolean if a field has been set.

### GetNextPageUrl

`func (o *ViewAllMmsCampaigns) GetNextPageUrl() string`

GetNextPageUrl returns the NextPageUrl field if non-nil, zero value otherwise.

### GetNextPageUrlOk

`func (o *ViewAllMmsCampaigns) GetNextPageUrlOk() (*string, bool)`

GetNextPageUrlOk returns a tuple with the NextPageUrl field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetNextPageUrl

`func (o *ViewAllMmsCampaigns) SetNextPageUrl(v string)`

SetNextPageUrl sets NextPageUrl field to given value.

### HasNextPageUrl

`func (o *ViewAllMmsCampaigns) HasNextPageUrl() bool`

HasNextPageUrl returns a boolean if a field has been set.

### SetNextPageUrlNil

`func (o *ViewAllMmsCampaigns) SetNextPageUrlNil(b bool)`

 SetNextPageUrlNil sets the value for NextPageUrl to be an explicit nil

### UnsetNextPageUrl
`func (o *ViewAllMmsCampaigns) UnsetNextPageUrl()`

UnsetNextPageUrl ensures that no value is present for NextPageUrl, not even an explicit nil
### GetPrevPageUrl

`func (o *ViewAllMmsCampaigns) GetPrevPageUrl() string`

GetPrevPageUrl returns the PrevPageUrl field if non-nil, zero value otherwise.

### GetPrevPageUrlOk

`func (o *ViewAllMmsCampaigns) GetPrevPageUrlOk() (*string, bool)`

GetPrevPageUrlOk returns a tuple with the PrevPageUrl field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetPrevPageUrl

`func (o *ViewAllMmsCampaigns) SetPrevPageUrl(v string)`

SetPrevPageUrl sets PrevPageUrl field to given value.

### HasPrevPageUrl

`func (o *ViewAllMmsCampaigns) HasPrevPageUrl() bool`

HasPrevPageUrl returns a boolean if a field has been set.

### SetPrevPageUrlNil

`func (o *ViewAllMmsCampaigns) SetPrevPageUrlNil(b bool)`

 SetPrevPageUrlNil sets the value for PrevPageUrl to be an explicit nil

### UnsetPrevPageUrl
`func (o *ViewAllMmsCampaigns) UnsetPrevPageUrl()`

UnsetPrevPageUrl ensures that no value is present for PrevPageUrl, not even an explicit nil
### GetFrom

`func (o *ViewAllMmsCampaigns) GetFrom() int32`

GetFrom returns the From field if non-nil, zero value otherwise.

### GetFromOk

`func (o *ViewAllMmsCampaigns) GetFromOk() (*int32, bool)`

GetFromOk returns a tuple with the From field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetFrom

`func (o *ViewAllMmsCampaigns) SetFrom(v int32)`

SetFrom sets From field to given value.

### HasFrom

`func (o *ViewAllMmsCampaigns) HasFrom() bool`

HasFrom returns a boolean if a field has been set.

### GetTo

`func (o *ViewAllMmsCampaigns) GetTo() int32`

GetTo returns the To field if non-nil, zero value otherwise.

### GetToOk

`func (o *ViewAllMmsCampaigns) GetToOk() (*int32, bool)`

GetToOk returns a tuple with the To field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTo

`func (o *ViewAllMmsCampaigns) SetTo(v int32)`

SetTo sets To field to given value.

### HasTo

`func (o *ViewAllMmsCampaigns) HasTo() bool`

HasTo returns a boolean if a field has been set.

### GetData

`func (o *ViewAllMmsCampaigns) GetData() []MmsCampaign`

GetData returns the Data field if non-nil, zero value otherwise.

### GetDataOk

`func (o *ViewAllMmsCampaigns) GetDataOk() (*[]MmsCampaign, bool)`

GetDataOk returns a tuple with the Data field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetData

`func (o *ViewAllMmsCampaigns) SetData(v []MmsCampaign)`

SetData sets Data field to given value.

### HasData

`func (o *ViewAllMmsCampaigns) HasData() bool`

HasData returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


