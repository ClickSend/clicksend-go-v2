# ViewSmsInboundAutomationsData

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
**FirstPageUrl** | Pointer to **NullableString** | The URL of the first page of records. | [optional] 
**LastPageUrl** | Pointer to **NullableString** | The URL of the last page of records. | [optional] 
**Path** | Pointer to **string** | The base URL path used to build pagination links. | [optional] 
**Links** | Pointer to [**[]ViewSmsInboundAutomationsDataAllOfLinksInner**](ViewSmsInboundAutomationsDataAllOfLinksInner.md) | The list of pagination links. | [optional] 
**Data** | Pointer to [**[]SmsInboundRule**](SmsInboundRule.md) |  | [optional] 

## Methods

### NewViewSmsInboundAutomationsData

`func NewViewSmsInboundAutomationsData() *ViewSmsInboundAutomationsData`

NewViewSmsInboundAutomationsData instantiates a new ViewSmsInboundAutomationsData object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewViewSmsInboundAutomationsDataWithDefaults

`func NewViewSmsInboundAutomationsDataWithDefaults() *ViewSmsInboundAutomationsData`

NewViewSmsInboundAutomationsDataWithDefaults instantiates a new ViewSmsInboundAutomationsData object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetTotal

`func (o *ViewSmsInboundAutomationsData) GetTotal() int32`

GetTotal returns the Total field if non-nil, zero value otherwise.

### GetTotalOk

`func (o *ViewSmsInboundAutomationsData) GetTotalOk() (*int32, bool)`

GetTotalOk returns a tuple with the Total field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTotal

`func (o *ViewSmsInboundAutomationsData) SetTotal(v int32)`

SetTotal sets Total field to given value.

### HasTotal

`func (o *ViewSmsInboundAutomationsData) HasTotal() bool`

HasTotal returns a boolean if a field has been set.

### GetPerPage

`func (o *ViewSmsInboundAutomationsData) GetPerPage() int32`

GetPerPage returns the PerPage field if non-nil, zero value otherwise.

### GetPerPageOk

`func (o *ViewSmsInboundAutomationsData) GetPerPageOk() (*int32, bool)`

GetPerPageOk returns a tuple with the PerPage field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetPerPage

`func (o *ViewSmsInboundAutomationsData) SetPerPage(v int32)`

SetPerPage sets PerPage field to given value.

### HasPerPage

`func (o *ViewSmsInboundAutomationsData) HasPerPage() bool`

HasPerPage returns a boolean if a field has been set.

### GetCurrentPage

`func (o *ViewSmsInboundAutomationsData) GetCurrentPage() int32`

GetCurrentPage returns the CurrentPage field if non-nil, zero value otherwise.

### GetCurrentPageOk

`func (o *ViewSmsInboundAutomationsData) GetCurrentPageOk() (*int32, bool)`

GetCurrentPageOk returns a tuple with the CurrentPage field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCurrentPage

`func (o *ViewSmsInboundAutomationsData) SetCurrentPage(v int32)`

SetCurrentPage sets CurrentPage field to given value.

### HasCurrentPage

`func (o *ViewSmsInboundAutomationsData) HasCurrentPage() bool`

HasCurrentPage returns a boolean if a field has been set.

### GetLastPage

`func (o *ViewSmsInboundAutomationsData) GetLastPage() int32`

GetLastPage returns the LastPage field if non-nil, zero value otherwise.

### GetLastPageOk

`func (o *ViewSmsInboundAutomationsData) GetLastPageOk() (*int32, bool)`

GetLastPageOk returns a tuple with the LastPage field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetLastPage

`func (o *ViewSmsInboundAutomationsData) SetLastPage(v int32)`

SetLastPage sets LastPage field to given value.

### HasLastPage

`func (o *ViewSmsInboundAutomationsData) HasLastPage() bool`

HasLastPage returns a boolean if a field has been set.

### GetNextPageUrl

`func (o *ViewSmsInboundAutomationsData) GetNextPageUrl() string`

GetNextPageUrl returns the NextPageUrl field if non-nil, zero value otherwise.

### GetNextPageUrlOk

`func (o *ViewSmsInboundAutomationsData) GetNextPageUrlOk() (*string, bool)`

GetNextPageUrlOk returns a tuple with the NextPageUrl field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetNextPageUrl

`func (o *ViewSmsInboundAutomationsData) SetNextPageUrl(v string)`

SetNextPageUrl sets NextPageUrl field to given value.

### HasNextPageUrl

`func (o *ViewSmsInboundAutomationsData) HasNextPageUrl() bool`

HasNextPageUrl returns a boolean if a field has been set.

### SetNextPageUrlNil

`func (o *ViewSmsInboundAutomationsData) SetNextPageUrlNil(b bool)`

 SetNextPageUrlNil sets the value for NextPageUrl to be an explicit nil

### UnsetNextPageUrl
`func (o *ViewSmsInboundAutomationsData) UnsetNextPageUrl()`

UnsetNextPageUrl ensures that no value is present for NextPageUrl, not even an explicit nil
### GetPrevPageUrl

`func (o *ViewSmsInboundAutomationsData) GetPrevPageUrl() string`

GetPrevPageUrl returns the PrevPageUrl field if non-nil, zero value otherwise.

### GetPrevPageUrlOk

`func (o *ViewSmsInboundAutomationsData) GetPrevPageUrlOk() (*string, bool)`

GetPrevPageUrlOk returns a tuple with the PrevPageUrl field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetPrevPageUrl

`func (o *ViewSmsInboundAutomationsData) SetPrevPageUrl(v string)`

SetPrevPageUrl sets PrevPageUrl field to given value.

### HasPrevPageUrl

`func (o *ViewSmsInboundAutomationsData) HasPrevPageUrl() bool`

HasPrevPageUrl returns a boolean if a field has been set.

### SetPrevPageUrlNil

`func (o *ViewSmsInboundAutomationsData) SetPrevPageUrlNil(b bool)`

 SetPrevPageUrlNil sets the value for PrevPageUrl to be an explicit nil

### UnsetPrevPageUrl
`func (o *ViewSmsInboundAutomationsData) UnsetPrevPageUrl()`

UnsetPrevPageUrl ensures that no value is present for PrevPageUrl, not even an explicit nil
### GetFrom

`func (o *ViewSmsInboundAutomationsData) GetFrom() int32`

GetFrom returns the From field if non-nil, zero value otherwise.

### GetFromOk

`func (o *ViewSmsInboundAutomationsData) GetFromOk() (*int32, bool)`

GetFromOk returns a tuple with the From field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetFrom

`func (o *ViewSmsInboundAutomationsData) SetFrom(v int32)`

SetFrom sets From field to given value.

### HasFrom

`func (o *ViewSmsInboundAutomationsData) HasFrom() bool`

HasFrom returns a boolean if a field has been set.

### GetTo

`func (o *ViewSmsInboundAutomationsData) GetTo() int32`

GetTo returns the To field if non-nil, zero value otherwise.

### GetToOk

`func (o *ViewSmsInboundAutomationsData) GetToOk() (*int32, bool)`

GetToOk returns a tuple with the To field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTo

`func (o *ViewSmsInboundAutomationsData) SetTo(v int32)`

SetTo sets To field to given value.

### HasTo

`func (o *ViewSmsInboundAutomationsData) HasTo() bool`

HasTo returns a boolean if a field has been set.

### GetFirstPageUrl

`func (o *ViewSmsInboundAutomationsData) GetFirstPageUrl() string`

GetFirstPageUrl returns the FirstPageUrl field if non-nil, zero value otherwise.

### GetFirstPageUrlOk

`func (o *ViewSmsInboundAutomationsData) GetFirstPageUrlOk() (*string, bool)`

GetFirstPageUrlOk returns a tuple with the FirstPageUrl field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetFirstPageUrl

`func (o *ViewSmsInboundAutomationsData) SetFirstPageUrl(v string)`

SetFirstPageUrl sets FirstPageUrl field to given value.

### HasFirstPageUrl

`func (o *ViewSmsInboundAutomationsData) HasFirstPageUrl() bool`

HasFirstPageUrl returns a boolean if a field has been set.

### SetFirstPageUrlNil

`func (o *ViewSmsInboundAutomationsData) SetFirstPageUrlNil(b bool)`

 SetFirstPageUrlNil sets the value for FirstPageUrl to be an explicit nil

### UnsetFirstPageUrl
`func (o *ViewSmsInboundAutomationsData) UnsetFirstPageUrl()`

UnsetFirstPageUrl ensures that no value is present for FirstPageUrl, not even an explicit nil
### GetLastPageUrl

`func (o *ViewSmsInboundAutomationsData) GetLastPageUrl() string`

GetLastPageUrl returns the LastPageUrl field if non-nil, zero value otherwise.

### GetLastPageUrlOk

`func (o *ViewSmsInboundAutomationsData) GetLastPageUrlOk() (*string, bool)`

GetLastPageUrlOk returns a tuple with the LastPageUrl field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetLastPageUrl

`func (o *ViewSmsInboundAutomationsData) SetLastPageUrl(v string)`

SetLastPageUrl sets LastPageUrl field to given value.

### HasLastPageUrl

`func (o *ViewSmsInboundAutomationsData) HasLastPageUrl() bool`

HasLastPageUrl returns a boolean if a field has been set.

### SetLastPageUrlNil

`func (o *ViewSmsInboundAutomationsData) SetLastPageUrlNil(b bool)`

 SetLastPageUrlNil sets the value for LastPageUrl to be an explicit nil

### UnsetLastPageUrl
`func (o *ViewSmsInboundAutomationsData) UnsetLastPageUrl()`

UnsetLastPageUrl ensures that no value is present for LastPageUrl, not even an explicit nil
### GetPath

`func (o *ViewSmsInboundAutomationsData) GetPath() string`

GetPath returns the Path field if non-nil, zero value otherwise.

### GetPathOk

`func (o *ViewSmsInboundAutomationsData) GetPathOk() (*string, bool)`

GetPathOk returns a tuple with the Path field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetPath

`func (o *ViewSmsInboundAutomationsData) SetPath(v string)`

SetPath sets Path field to given value.

### HasPath

`func (o *ViewSmsInboundAutomationsData) HasPath() bool`

HasPath returns a boolean if a field has been set.

### GetLinks

`func (o *ViewSmsInboundAutomationsData) GetLinks() []ViewSmsInboundAutomationsDataAllOfLinksInner`

GetLinks returns the Links field if non-nil, zero value otherwise.

### GetLinksOk

`func (o *ViewSmsInboundAutomationsData) GetLinksOk() (*[]ViewSmsInboundAutomationsDataAllOfLinksInner, bool)`

GetLinksOk returns a tuple with the Links field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetLinks

`func (o *ViewSmsInboundAutomationsData) SetLinks(v []ViewSmsInboundAutomationsDataAllOfLinksInner)`

SetLinks sets Links field to given value.

### HasLinks

`func (o *ViewSmsInboundAutomationsData) HasLinks() bool`

HasLinks returns a boolean if a field has been set.

### GetData

`func (o *ViewSmsInboundAutomationsData) GetData() []SmsInboundRule`

GetData returns the Data field if non-nil, zero value otherwise.

### GetDataOk

`func (o *ViewSmsInboundAutomationsData) GetDataOk() (*[]SmsInboundRule, bool)`

GetDataOk returns a tuple with the Data field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetData

`func (o *ViewSmsInboundAutomationsData) SetData(v []SmsInboundRule)`

SetData sets Data field to given value.

### HasData

`func (o *ViewSmsInboundAutomationsData) HasData() bool`

HasData returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


