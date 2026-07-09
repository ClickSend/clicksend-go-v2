# SendFaxRequest

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**FileUrl** | Pointer to **string** |  | [optional] 
**Messages** | Pointer to [**[]SendFaxRequestMessagesInner**](SendFaxRequestMessagesInner.md) |  | [optional] 

## Methods

### NewSendFaxRequest

`func NewSendFaxRequest() *SendFaxRequest`

NewSendFaxRequest instantiates a new SendFaxRequest object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewSendFaxRequestWithDefaults

`func NewSendFaxRequestWithDefaults() *SendFaxRequest`

NewSendFaxRequestWithDefaults instantiates a new SendFaxRequest object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetFileUrl

`func (o *SendFaxRequest) GetFileUrl() string`

GetFileUrl returns the FileUrl field if non-nil, zero value otherwise.

### GetFileUrlOk

`func (o *SendFaxRequest) GetFileUrlOk() (*string, bool)`

GetFileUrlOk returns a tuple with the FileUrl field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetFileUrl

`func (o *SendFaxRequest) SetFileUrl(v string)`

SetFileUrl sets FileUrl field to given value.

### HasFileUrl

`func (o *SendFaxRequest) HasFileUrl() bool`

HasFileUrl returns a boolean if a field has been set.

### GetMessages

`func (o *SendFaxRequest) GetMessages() []SendFaxRequestMessagesInner`

GetMessages returns the Messages field if non-nil, zero value otherwise.

### GetMessagesOk

`func (o *SendFaxRequest) GetMessagesOk() (*[]SendFaxRequestMessagesInner, bool)`

GetMessagesOk returns a tuple with the Messages field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetMessages

`func (o *SendFaxRequest) SetMessages(v []SendFaxRequestMessagesInner)`

SetMessages sets Messages field to given value.

### HasMessages

`func (o *SendFaxRequest) HasMessages() bool`

HasMessages returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


