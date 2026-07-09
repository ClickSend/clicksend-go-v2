# SendMmsRequest

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**MediaFile** | Pointer to **string** |  | [optional] 
**Messages** | Pointer to [**[]SendMmsRequestMessagesInner**](SendMmsRequestMessagesInner.md) |  | [optional] 

## Methods

### NewSendMmsRequest

`func NewSendMmsRequest() *SendMmsRequest`

NewSendMmsRequest instantiates a new SendMmsRequest object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewSendMmsRequestWithDefaults

`func NewSendMmsRequestWithDefaults() *SendMmsRequest`

NewSendMmsRequestWithDefaults instantiates a new SendMmsRequest object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetMediaFile

`func (o *SendMmsRequest) GetMediaFile() string`

GetMediaFile returns the MediaFile field if non-nil, zero value otherwise.

### GetMediaFileOk

`func (o *SendMmsRequest) GetMediaFileOk() (*string, bool)`

GetMediaFileOk returns a tuple with the MediaFile field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetMediaFile

`func (o *SendMmsRequest) SetMediaFile(v string)`

SetMediaFile sets MediaFile field to given value.

### HasMediaFile

`func (o *SendMmsRequest) HasMediaFile() bool`

HasMediaFile returns a boolean if a field has been set.

### GetMessages

`func (o *SendMmsRequest) GetMessages() []SendMmsRequestMessagesInner`

GetMessages returns the Messages field if non-nil, zero value otherwise.

### GetMessagesOk

`func (o *SendMmsRequest) GetMessagesOk() (*[]SendMmsRequestMessagesInner, bool)`

GetMessagesOk returns a tuple with the Messages field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetMessages

`func (o *SendMmsRequest) SetMessages(v []SendMmsRequestMessagesInner)`

SetMessages sets Messages field to given value.

### HasMessages

`func (o *SendMmsRequest) HasMessages() bool`

HasMessages returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


