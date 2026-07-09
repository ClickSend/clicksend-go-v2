# CalculateFaxPriceRequest

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**FileUrl** | Pointer to **string** |  | [optional] 
**Messages** | Pointer to [**[]CalculateFaxPriceRequestMessagesInner**](CalculateFaxPriceRequestMessagesInner.md) |  | [optional] 

## Methods

### NewCalculateFaxPriceRequest

`func NewCalculateFaxPriceRequest() *CalculateFaxPriceRequest`

NewCalculateFaxPriceRequest instantiates a new CalculateFaxPriceRequest object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewCalculateFaxPriceRequestWithDefaults

`func NewCalculateFaxPriceRequestWithDefaults() *CalculateFaxPriceRequest`

NewCalculateFaxPriceRequestWithDefaults instantiates a new CalculateFaxPriceRequest object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetFileUrl

`func (o *CalculateFaxPriceRequest) GetFileUrl() string`

GetFileUrl returns the FileUrl field if non-nil, zero value otherwise.

### GetFileUrlOk

`func (o *CalculateFaxPriceRequest) GetFileUrlOk() (*string, bool)`

GetFileUrlOk returns a tuple with the FileUrl field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetFileUrl

`func (o *CalculateFaxPriceRequest) SetFileUrl(v string)`

SetFileUrl sets FileUrl field to given value.

### HasFileUrl

`func (o *CalculateFaxPriceRequest) HasFileUrl() bool`

HasFileUrl returns a boolean if a field has been set.

### GetMessages

`func (o *CalculateFaxPriceRequest) GetMessages() []CalculateFaxPriceRequestMessagesInner`

GetMessages returns the Messages field if non-nil, zero value otherwise.

### GetMessagesOk

`func (o *CalculateFaxPriceRequest) GetMessagesOk() (*[]CalculateFaxPriceRequestMessagesInner, bool)`

GetMessagesOk returns a tuple with the Messages field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetMessages

`func (o *CalculateFaxPriceRequest) SetMessages(v []CalculateFaxPriceRequestMessagesInner)`

SetMessages sets Messages field to given value.

### HasMessages

`func (o *CalculateFaxPriceRequest) HasMessages() bool`

HasMessages returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


