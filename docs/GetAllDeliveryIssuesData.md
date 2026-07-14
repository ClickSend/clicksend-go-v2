# GetAllDeliveryIssuesData

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
**Data** | Pointer to [**[]DeliveryIssue**](DeliveryIssue.md) |  | [optional] 

## Methods

### NewGetAllDeliveryIssuesData

`func NewGetAllDeliveryIssuesData() *GetAllDeliveryIssuesData`

NewGetAllDeliveryIssuesData instantiates a new GetAllDeliveryIssuesData object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewGetAllDeliveryIssuesDataWithDefaults

`func NewGetAllDeliveryIssuesDataWithDefaults() *GetAllDeliveryIssuesData`

NewGetAllDeliveryIssuesDataWithDefaults instantiates a new GetAllDeliveryIssuesData object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetTotal

`func (o *GetAllDeliveryIssuesData) GetTotal() int32`

GetTotal returns the Total field if non-nil, zero value otherwise.

### GetTotalOk

`func (o *GetAllDeliveryIssuesData) GetTotalOk() (*int32, bool)`

GetTotalOk returns a tuple with the Total field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTotal

`func (o *GetAllDeliveryIssuesData) SetTotal(v int32)`

SetTotal sets Total field to given value.

### HasTotal

`func (o *GetAllDeliveryIssuesData) HasTotal() bool`

HasTotal returns a boolean if a field has been set.

### GetPerPage

`func (o *GetAllDeliveryIssuesData) GetPerPage() int32`

GetPerPage returns the PerPage field if non-nil, zero value otherwise.

### GetPerPageOk

`func (o *GetAllDeliveryIssuesData) GetPerPageOk() (*int32, bool)`

GetPerPageOk returns a tuple with the PerPage field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetPerPage

`func (o *GetAllDeliveryIssuesData) SetPerPage(v int32)`

SetPerPage sets PerPage field to given value.

### HasPerPage

`func (o *GetAllDeliveryIssuesData) HasPerPage() bool`

HasPerPage returns a boolean if a field has been set.

### GetCurrentPage

`func (o *GetAllDeliveryIssuesData) GetCurrentPage() int32`

GetCurrentPage returns the CurrentPage field if non-nil, zero value otherwise.

### GetCurrentPageOk

`func (o *GetAllDeliveryIssuesData) GetCurrentPageOk() (*int32, bool)`

GetCurrentPageOk returns a tuple with the CurrentPage field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCurrentPage

`func (o *GetAllDeliveryIssuesData) SetCurrentPage(v int32)`

SetCurrentPage sets CurrentPage field to given value.

### HasCurrentPage

`func (o *GetAllDeliveryIssuesData) HasCurrentPage() bool`

HasCurrentPage returns a boolean if a field has been set.

### GetLastPage

`func (o *GetAllDeliveryIssuesData) GetLastPage() int32`

GetLastPage returns the LastPage field if non-nil, zero value otherwise.

### GetLastPageOk

`func (o *GetAllDeliveryIssuesData) GetLastPageOk() (*int32, bool)`

GetLastPageOk returns a tuple with the LastPage field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetLastPage

`func (o *GetAllDeliveryIssuesData) SetLastPage(v int32)`

SetLastPage sets LastPage field to given value.

### HasLastPage

`func (o *GetAllDeliveryIssuesData) HasLastPage() bool`

HasLastPage returns a boolean if a field has been set.

### GetNextPageUrl

`func (o *GetAllDeliveryIssuesData) GetNextPageUrl() string`

GetNextPageUrl returns the NextPageUrl field if non-nil, zero value otherwise.

### GetNextPageUrlOk

`func (o *GetAllDeliveryIssuesData) GetNextPageUrlOk() (*string, bool)`

GetNextPageUrlOk returns a tuple with the NextPageUrl field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetNextPageUrl

`func (o *GetAllDeliveryIssuesData) SetNextPageUrl(v string)`

SetNextPageUrl sets NextPageUrl field to given value.

### HasNextPageUrl

`func (o *GetAllDeliveryIssuesData) HasNextPageUrl() bool`

HasNextPageUrl returns a boolean if a field has been set.

### SetNextPageUrlNil

`func (o *GetAllDeliveryIssuesData) SetNextPageUrlNil(b bool)`

 SetNextPageUrlNil sets the value for NextPageUrl to be an explicit nil

### UnsetNextPageUrl
`func (o *GetAllDeliveryIssuesData) UnsetNextPageUrl()`

UnsetNextPageUrl ensures that no value is present for NextPageUrl, not even an explicit nil
### GetPrevPageUrl

`func (o *GetAllDeliveryIssuesData) GetPrevPageUrl() string`

GetPrevPageUrl returns the PrevPageUrl field if non-nil, zero value otherwise.

### GetPrevPageUrlOk

`func (o *GetAllDeliveryIssuesData) GetPrevPageUrlOk() (*string, bool)`

GetPrevPageUrlOk returns a tuple with the PrevPageUrl field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetPrevPageUrl

`func (o *GetAllDeliveryIssuesData) SetPrevPageUrl(v string)`

SetPrevPageUrl sets PrevPageUrl field to given value.

### HasPrevPageUrl

`func (o *GetAllDeliveryIssuesData) HasPrevPageUrl() bool`

HasPrevPageUrl returns a boolean if a field has been set.

### SetPrevPageUrlNil

`func (o *GetAllDeliveryIssuesData) SetPrevPageUrlNil(b bool)`

 SetPrevPageUrlNil sets the value for PrevPageUrl to be an explicit nil

### UnsetPrevPageUrl
`func (o *GetAllDeliveryIssuesData) UnsetPrevPageUrl()`

UnsetPrevPageUrl ensures that no value is present for PrevPageUrl, not even an explicit nil
### GetFrom

`func (o *GetAllDeliveryIssuesData) GetFrom() int32`

GetFrom returns the From field if non-nil, zero value otherwise.

### GetFromOk

`func (o *GetAllDeliveryIssuesData) GetFromOk() (*int32, bool)`

GetFromOk returns a tuple with the From field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetFrom

`func (o *GetAllDeliveryIssuesData) SetFrom(v int32)`

SetFrom sets From field to given value.

### HasFrom

`func (o *GetAllDeliveryIssuesData) HasFrom() bool`

HasFrom returns a boolean if a field has been set.

### GetTo

`func (o *GetAllDeliveryIssuesData) GetTo() int32`

GetTo returns the To field if non-nil, zero value otherwise.

### GetToOk

`func (o *GetAllDeliveryIssuesData) GetToOk() (*int32, bool)`

GetToOk returns a tuple with the To field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTo

`func (o *GetAllDeliveryIssuesData) SetTo(v int32)`

SetTo sets To field to given value.

### HasTo

`func (o *GetAllDeliveryIssuesData) HasTo() bool`

HasTo returns a boolean if a field has been set.

### GetData

`func (o *GetAllDeliveryIssuesData) GetData() []DeliveryIssue`

GetData returns the Data field if non-nil, zero value otherwise.

### GetDataOk

`func (o *GetAllDeliveryIssuesData) GetDataOk() (*[]DeliveryIssue, bool)`

GetDataOk returns a tuple with the Data field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetData

`func (o *GetAllDeliveryIssuesData) SetData(v []DeliveryIssue)`

SetData sets Data field to given value.

### HasData

`func (o *GetAllDeliveryIssuesData) HasData() bool`

HasData returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


