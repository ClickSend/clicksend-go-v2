# ViewEmailTemplatesData

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Total** | Pointer to **int32** | The total number of records in the response. | [optional] 
**PerPage** | Pointer to **int32** | The number of records per page. | [optional] 
**CurrentPage** | Pointer to **int32** | The current page number. | [optional] 
**LastPage** | Pointer to **int32** | The last page number. | [optional] 
**NextPageUrl** | Pointer to **NullableString** | The URL of the next page of records. | [optional] 
**PrevPageUrl** | Pointer to **NullableString** | The URL of the previous page of records. | [optional] 
**From** | Pointer to **int32** | The index of the first record in the page. | [optional] 
**To** | Pointer to **int32** | The index of the last record in the page. | [optional] 
**Data** | Pointer to [**[]ViewEmailTemplatesDataDataInner**](ViewEmailTemplatesDataDataInner.md) |  | [optional] 

## Methods

### NewViewEmailTemplatesData

`func NewViewEmailTemplatesData() *ViewEmailTemplatesData`

NewViewEmailTemplatesData instantiates a new ViewEmailTemplatesData object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewViewEmailTemplatesDataWithDefaults

`func NewViewEmailTemplatesDataWithDefaults() *ViewEmailTemplatesData`

NewViewEmailTemplatesDataWithDefaults instantiates a new ViewEmailTemplatesData object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetTotal

`func (o *ViewEmailTemplatesData) GetTotal() int32`

GetTotal returns the Total field if non-nil, zero value otherwise.

### GetTotalOk

`func (o *ViewEmailTemplatesData) GetTotalOk() (*int32, bool)`

GetTotalOk returns a tuple with the Total field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTotal

`func (o *ViewEmailTemplatesData) SetTotal(v int32)`

SetTotal sets Total field to given value.

### HasTotal

`func (o *ViewEmailTemplatesData) HasTotal() bool`

HasTotal returns a boolean if a field has been set.

### GetPerPage

`func (o *ViewEmailTemplatesData) GetPerPage() int32`

GetPerPage returns the PerPage field if non-nil, zero value otherwise.

### GetPerPageOk

`func (o *ViewEmailTemplatesData) GetPerPageOk() (*int32, bool)`

GetPerPageOk returns a tuple with the PerPage field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetPerPage

`func (o *ViewEmailTemplatesData) SetPerPage(v int32)`

SetPerPage sets PerPage field to given value.

### HasPerPage

`func (o *ViewEmailTemplatesData) HasPerPage() bool`

HasPerPage returns a boolean if a field has been set.

### GetCurrentPage

`func (o *ViewEmailTemplatesData) GetCurrentPage() int32`

GetCurrentPage returns the CurrentPage field if non-nil, zero value otherwise.

### GetCurrentPageOk

`func (o *ViewEmailTemplatesData) GetCurrentPageOk() (*int32, bool)`

GetCurrentPageOk returns a tuple with the CurrentPage field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCurrentPage

`func (o *ViewEmailTemplatesData) SetCurrentPage(v int32)`

SetCurrentPage sets CurrentPage field to given value.

### HasCurrentPage

`func (o *ViewEmailTemplatesData) HasCurrentPage() bool`

HasCurrentPage returns a boolean if a field has been set.

### GetLastPage

`func (o *ViewEmailTemplatesData) GetLastPage() int32`

GetLastPage returns the LastPage field if non-nil, zero value otherwise.

### GetLastPageOk

`func (o *ViewEmailTemplatesData) GetLastPageOk() (*int32, bool)`

GetLastPageOk returns a tuple with the LastPage field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetLastPage

`func (o *ViewEmailTemplatesData) SetLastPage(v int32)`

SetLastPage sets LastPage field to given value.

### HasLastPage

`func (o *ViewEmailTemplatesData) HasLastPage() bool`

HasLastPage returns a boolean if a field has been set.

### GetNextPageUrl

`func (o *ViewEmailTemplatesData) GetNextPageUrl() string`

GetNextPageUrl returns the NextPageUrl field if non-nil, zero value otherwise.

### GetNextPageUrlOk

`func (o *ViewEmailTemplatesData) GetNextPageUrlOk() (*string, bool)`

GetNextPageUrlOk returns a tuple with the NextPageUrl field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetNextPageUrl

`func (o *ViewEmailTemplatesData) SetNextPageUrl(v string)`

SetNextPageUrl sets NextPageUrl field to given value.

### HasNextPageUrl

`func (o *ViewEmailTemplatesData) HasNextPageUrl() bool`

HasNextPageUrl returns a boolean if a field has been set.

### SetNextPageUrlNil

`func (o *ViewEmailTemplatesData) SetNextPageUrlNil(b bool)`

 SetNextPageUrlNil sets the value for NextPageUrl to be an explicit nil

### UnsetNextPageUrl
`func (o *ViewEmailTemplatesData) UnsetNextPageUrl()`

UnsetNextPageUrl ensures that no value is present for NextPageUrl, not even an explicit nil
### GetPrevPageUrl

`func (o *ViewEmailTemplatesData) GetPrevPageUrl() string`

GetPrevPageUrl returns the PrevPageUrl field if non-nil, zero value otherwise.

### GetPrevPageUrlOk

`func (o *ViewEmailTemplatesData) GetPrevPageUrlOk() (*string, bool)`

GetPrevPageUrlOk returns a tuple with the PrevPageUrl field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetPrevPageUrl

`func (o *ViewEmailTemplatesData) SetPrevPageUrl(v string)`

SetPrevPageUrl sets PrevPageUrl field to given value.

### HasPrevPageUrl

`func (o *ViewEmailTemplatesData) HasPrevPageUrl() bool`

HasPrevPageUrl returns a boolean if a field has been set.

### SetPrevPageUrlNil

`func (o *ViewEmailTemplatesData) SetPrevPageUrlNil(b bool)`

 SetPrevPageUrlNil sets the value for PrevPageUrl to be an explicit nil

### UnsetPrevPageUrl
`func (o *ViewEmailTemplatesData) UnsetPrevPageUrl()`

UnsetPrevPageUrl ensures that no value is present for PrevPageUrl, not even an explicit nil
### GetFrom

`func (o *ViewEmailTemplatesData) GetFrom() int32`

GetFrom returns the From field if non-nil, zero value otherwise.

### GetFromOk

`func (o *ViewEmailTemplatesData) GetFromOk() (*int32, bool)`

GetFromOk returns a tuple with the From field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetFrom

`func (o *ViewEmailTemplatesData) SetFrom(v int32)`

SetFrom sets From field to given value.

### HasFrom

`func (o *ViewEmailTemplatesData) HasFrom() bool`

HasFrom returns a boolean if a field has been set.

### GetTo

`func (o *ViewEmailTemplatesData) GetTo() int32`

GetTo returns the To field if non-nil, zero value otherwise.

### GetToOk

`func (o *ViewEmailTemplatesData) GetToOk() (*int32, bool)`

GetToOk returns a tuple with the To field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTo

`func (o *ViewEmailTemplatesData) SetTo(v int32)`

SetTo sets To field to given value.

### HasTo

`func (o *ViewEmailTemplatesData) HasTo() bool`

HasTo returns a boolean if a field has been set.

### GetData

`func (o *ViewEmailTemplatesData) GetData() []ViewEmailTemplatesDataDataInner`

GetData returns the Data field if non-nil, zero value otherwise.

### GetDataOk

`func (o *ViewEmailTemplatesData) GetDataOk() (*[]ViewEmailTemplatesDataDataInner, bool)`

GetDataOk returns a tuple with the Data field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetData

`func (o *ViewEmailTemplatesData) SetData(v []ViewEmailTemplatesDataDataInner)`

SetData sets Data field to given value.

### HasData

`func (o *ViewEmailTemplatesData) HasData() bool`

HasData returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


