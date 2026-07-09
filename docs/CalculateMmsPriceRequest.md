# CalculateMmsPriceRequest

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**MediaFile** | Pointer to **string** |  | [optional] 
**Messages** | Pointer to [**[]CalculateMmsPriceRequestMessagesInner**](CalculateMmsPriceRequestMessagesInner.md) |  | [optional] 

## Methods

### NewCalculateMmsPriceRequest

`func NewCalculateMmsPriceRequest() *CalculateMmsPriceRequest`

NewCalculateMmsPriceRequest instantiates a new CalculateMmsPriceRequest object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewCalculateMmsPriceRequestWithDefaults

`func NewCalculateMmsPriceRequestWithDefaults() *CalculateMmsPriceRequest`

NewCalculateMmsPriceRequestWithDefaults instantiates a new CalculateMmsPriceRequest object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetMediaFile

`func (o *CalculateMmsPriceRequest) GetMediaFile() string`

GetMediaFile returns the MediaFile field if non-nil, zero value otherwise.

### GetMediaFileOk

`func (o *CalculateMmsPriceRequest) GetMediaFileOk() (*string, bool)`

GetMediaFileOk returns a tuple with the MediaFile field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetMediaFile

`func (o *CalculateMmsPriceRequest) SetMediaFile(v string)`

SetMediaFile sets MediaFile field to given value.

### HasMediaFile

`func (o *CalculateMmsPriceRequest) HasMediaFile() bool`

HasMediaFile returns a boolean if a field has been set.

### GetMessages

`func (o *CalculateMmsPriceRequest) GetMessages() []CalculateMmsPriceRequestMessagesInner`

GetMessages returns the Messages field if non-nil, zero value otherwise.

### GetMessagesOk

`func (o *CalculateMmsPriceRequest) GetMessagesOk() (*[]CalculateMmsPriceRequestMessagesInner, bool)`

GetMessagesOk returns a tuple with the Messages field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetMessages

`func (o *CalculateMmsPriceRequest) SetMessages(v []CalculateMmsPriceRequestMessagesInner)`

SetMessages sets Messages field to given value.

### HasMessages

`func (o *CalculateMmsPriceRequest) HasMessages() bool`

HasMessages returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


