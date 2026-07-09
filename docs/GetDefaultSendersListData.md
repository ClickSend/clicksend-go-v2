# GetDefaultSendersListData

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Data** | Pointer to [**[]DefaultSender**](DefaultSender.md) | List of default senders. | [optional] 
**PerPage** | Pointer to **int32** | Number of items per page. | [optional] 
**SelfPageUrl** | Pointer to **string** | URL for the current page. | [optional] 
**NextPageUrl** | Pointer to **string** | URL for the next page. | [optional] 

## Methods

### NewGetDefaultSendersListData

`func NewGetDefaultSendersListData() *GetDefaultSendersListData`

NewGetDefaultSendersListData instantiates a new GetDefaultSendersListData object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewGetDefaultSendersListDataWithDefaults

`func NewGetDefaultSendersListDataWithDefaults() *GetDefaultSendersListData`

NewGetDefaultSendersListDataWithDefaults instantiates a new GetDefaultSendersListData object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetData

`func (o *GetDefaultSendersListData) GetData() []DefaultSender`

GetData returns the Data field if non-nil, zero value otherwise.

### GetDataOk

`func (o *GetDefaultSendersListData) GetDataOk() (*[]DefaultSender, bool)`

GetDataOk returns a tuple with the Data field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetData

`func (o *GetDefaultSendersListData) SetData(v []DefaultSender)`

SetData sets Data field to given value.

### HasData

`func (o *GetDefaultSendersListData) HasData() bool`

HasData returns a boolean if a field has been set.

### GetPerPage

`func (o *GetDefaultSendersListData) GetPerPage() int32`

GetPerPage returns the PerPage field if non-nil, zero value otherwise.

### GetPerPageOk

`func (o *GetDefaultSendersListData) GetPerPageOk() (*int32, bool)`

GetPerPageOk returns a tuple with the PerPage field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetPerPage

`func (o *GetDefaultSendersListData) SetPerPage(v int32)`

SetPerPage sets PerPage field to given value.

### HasPerPage

`func (o *GetDefaultSendersListData) HasPerPage() bool`

HasPerPage returns a boolean if a field has been set.

### GetSelfPageUrl

`func (o *GetDefaultSendersListData) GetSelfPageUrl() string`

GetSelfPageUrl returns the SelfPageUrl field if non-nil, zero value otherwise.

### GetSelfPageUrlOk

`func (o *GetDefaultSendersListData) GetSelfPageUrlOk() (*string, bool)`

GetSelfPageUrlOk returns a tuple with the SelfPageUrl field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSelfPageUrl

`func (o *GetDefaultSendersListData) SetSelfPageUrl(v string)`

SetSelfPageUrl sets SelfPageUrl field to given value.

### HasSelfPageUrl

`func (o *GetDefaultSendersListData) HasSelfPageUrl() bool`

HasSelfPageUrl returns a boolean if a field has been set.

### GetNextPageUrl

`func (o *GetDefaultSendersListData) GetNextPageUrl() string`

GetNextPageUrl returns the NextPageUrl field if non-nil, zero value otherwise.

### GetNextPageUrlOk

`func (o *GetDefaultSendersListData) GetNextPageUrlOk() (*string, bool)`

GetNextPageUrlOk returns a tuple with the NextPageUrl field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetNextPageUrl

`func (o *GetDefaultSendersListData) SetNextPageUrl(v string)`

SetNextPageUrl sets NextPageUrl field to given value.

### HasNextPageUrl

`func (o *GetDefaultSendersListData) HasNextPageUrl() bool`

HasNextPageUrl returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


