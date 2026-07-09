# SendVoiceMessageRequest

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Messages** | Pointer to [**[]SendVoiceMessageRequestMessagesInner**](SendVoiceMessageRequestMessagesInner.md) |  | [optional] 

## Methods

### NewSendVoiceMessageRequest

`func NewSendVoiceMessageRequest() *SendVoiceMessageRequest`

NewSendVoiceMessageRequest instantiates a new SendVoiceMessageRequest object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewSendVoiceMessageRequestWithDefaults

`func NewSendVoiceMessageRequestWithDefaults() *SendVoiceMessageRequest`

NewSendVoiceMessageRequestWithDefaults instantiates a new SendVoiceMessageRequest object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetMessages

`func (o *SendVoiceMessageRequest) GetMessages() []SendVoiceMessageRequestMessagesInner`

GetMessages returns the Messages field if non-nil, zero value otherwise.

### GetMessagesOk

`func (o *SendVoiceMessageRequest) GetMessagesOk() (*[]SendVoiceMessageRequestMessagesInner, bool)`

GetMessagesOk returns a tuple with the Messages field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetMessages

`func (o *SendVoiceMessageRequest) SetMessages(v []SendVoiceMessageRequestMessagesInner)`

SetMessages sets Messages field to given value.

### HasMessages

`func (o *SendVoiceMessageRequest) HasMessages() bool`

HasMessages returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


