# GetTracking

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Total** | Pointer to **float32** | Total number of short URLs associated with the long URL ID | [optional] 
**PerPage** | Pointer to **float32** | The limit of tracking data per page | [optional] 
**CurrentPageSize** | Pointer to **float32** | The number of data in the current page | [optional] 
**PrevPageUrl** | Pointer to **string** | Link to the previous page. This attribute will not be present if there is no previous page. | [optional] 
**NextPageUrl** | Pointer to **string** | Link to the next page. This attribute will not be present if there is no next page. | [optional] 
**Data** | Pointer to [**[]GetTrackingDataInner**](GetTrackingDataInner.md) | Tracking data of the short URLs associated with the specified long URL ID. Note that only the data from the most recent click of the recipient (country, region, device, browser, and os) is recorded. | [optional] 

## Methods

### NewGetTracking

`func NewGetTracking() *GetTracking`

NewGetTracking instantiates a new GetTracking object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewGetTrackingWithDefaults

`func NewGetTrackingWithDefaults() *GetTracking`

NewGetTrackingWithDefaults instantiates a new GetTracking object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetTotal

`func (o *GetTracking) GetTotal() float32`

GetTotal returns the Total field if non-nil, zero value otherwise.

### GetTotalOk

`func (o *GetTracking) GetTotalOk() (*float32, bool)`

GetTotalOk returns a tuple with the Total field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTotal

`func (o *GetTracking) SetTotal(v float32)`

SetTotal sets Total field to given value.

### HasTotal

`func (o *GetTracking) HasTotal() bool`

HasTotal returns a boolean if a field has been set.

### GetPerPage

`func (o *GetTracking) GetPerPage() float32`

GetPerPage returns the PerPage field if non-nil, zero value otherwise.

### GetPerPageOk

`func (o *GetTracking) GetPerPageOk() (*float32, bool)`

GetPerPageOk returns a tuple with the PerPage field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetPerPage

`func (o *GetTracking) SetPerPage(v float32)`

SetPerPage sets PerPage field to given value.

### HasPerPage

`func (o *GetTracking) HasPerPage() bool`

HasPerPage returns a boolean if a field has been set.

### GetCurrentPageSize

`func (o *GetTracking) GetCurrentPageSize() float32`

GetCurrentPageSize returns the CurrentPageSize field if non-nil, zero value otherwise.

### GetCurrentPageSizeOk

`func (o *GetTracking) GetCurrentPageSizeOk() (*float32, bool)`

GetCurrentPageSizeOk returns a tuple with the CurrentPageSize field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCurrentPageSize

`func (o *GetTracking) SetCurrentPageSize(v float32)`

SetCurrentPageSize sets CurrentPageSize field to given value.

### HasCurrentPageSize

`func (o *GetTracking) HasCurrentPageSize() bool`

HasCurrentPageSize returns a boolean if a field has been set.

### GetPrevPageUrl

`func (o *GetTracking) GetPrevPageUrl() string`

GetPrevPageUrl returns the PrevPageUrl field if non-nil, zero value otherwise.

### GetPrevPageUrlOk

`func (o *GetTracking) GetPrevPageUrlOk() (*string, bool)`

GetPrevPageUrlOk returns a tuple with the PrevPageUrl field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetPrevPageUrl

`func (o *GetTracking) SetPrevPageUrl(v string)`

SetPrevPageUrl sets PrevPageUrl field to given value.

### HasPrevPageUrl

`func (o *GetTracking) HasPrevPageUrl() bool`

HasPrevPageUrl returns a boolean if a field has been set.

### GetNextPageUrl

`func (o *GetTracking) GetNextPageUrl() string`

GetNextPageUrl returns the NextPageUrl field if non-nil, zero value otherwise.

### GetNextPageUrlOk

`func (o *GetTracking) GetNextPageUrlOk() (*string, bool)`

GetNextPageUrlOk returns a tuple with the NextPageUrl field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetNextPageUrl

`func (o *GetTracking) SetNextPageUrl(v string)`

SetNextPageUrl sets NextPageUrl field to given value.

### HasNextPageUrl

`func (o *GetTracking) HasNextPageUrl() bool`

HasNextPageUrl returns a boolean if a field has been set.

### GetData

`func (o *GetTracking) GetData() []GetTrackingDataInner`

GetData returns the Data field if non-nil, zero value otherwise.

### GetDataOk

`func (o *GetTracking) GetDataOk() (*[]GetTrackingDataInner, bool)`

GetDataOk returns a tuple with the Data field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetData

`func (o *GetTracking) SetData(v []GetTrackingDataInner)`

SetData sets Data field to given value.

### HasData

`func (o *GetTracking) HasData() bool`

HasData returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


