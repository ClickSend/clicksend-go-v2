# SendVoiceMessageData

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**TotalPrice** | Pointer to **float32** | The total price of the message. | [optional] 
**TotalCount** | Pointer to **float32** | The total count of the message. | [optional] 
**QueuedCount** | Pointer to **float32** | The count of the queued message. | [optional] 
**Messages** | Pointer to [**[]VoiceMessage**](VoiceMessage.md) |  | [optional] 
**Currency** | Pointer to [**Currency**](Currency.md) |  | [optional] 

## Methods

### NewSendVoiceMessageData

`func NewSendVoiceMessageData() *SendVoiceMessageData`

NewSendVoiceMessageData instantiates a new SendVoiceMessageData object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewSendVoiceMessageDataWithDefaults

`func NewSendVoiceMessageDataWithDefaults() *SendVoiceMessageData`

NewSendVoiceMessageDataWithDefaults instantiates a new SendVoiceMessageData object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetTotalPrice

`func (o *SendVoiceMessageData) GetTotalPrice() float32`

GetTotalPrice returns the TotalPrice field if non-nil, zero value otherwise.

### GetTotalPriceOk

`func (o *SendVoiceMessageData) GetTotalPriceOk() (*float32, bool)`

GetTotalPriceOk returns a tuple with the TotalPrice field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTotalPrice

`func (o *SendVoiceMessageData) SetTotalPrice(v float32)`

SetTotalPrice sets TotalPrice field to given value.

### HasTotalPrice

`func (o *SendVoiceMessageData) HasTotalPrice() bool`

HasTotalPrice returns a boolean if a field has been set.

### GetTotalCount

`func (o *SendVoiceMessageData) GetTotalCount() float32`

GetTotalCount returns the TotalCount field if non-nil, zero value otherwise.

### GetTotalCountOk

`func (o *SendVoiceMessageData) GetTotalCountOk() (*float32, bool)`

GetTotalCountOk returns a tuple with the TotalCount field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTotalCount

`func (o *SendVoiceMessageData) SetTotalCount(v float32)`

SetTotalCount sets TotalCount field to given value.

### HasTotalCount

`func (o *SendVoiceMessageData) HasTotalCount() bool`

HasTotalCount returns a boolean if a field has been set.

### GetQueuedCount

`func (o *SendVoiceMessageData) GetQueuedCount() float32`

GetQueuedCount returns the QueuedCount field if non-nil, zero value otherwise.

### GetQueuedCountOk

`func (o *SendVoiceMessageData) GetQueuedCountOk() (*float32, bool)`

GetQueuedCountOk returns a tuple with the QueuedCount field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetQueuedCount

`func (o *SendVoiceMessageData) SetQueuedCount(v float32)`

SetQueuedCount sets QueuedCount field to given value.

### HasQueuedCount

`func (o *SendVoiceMessageData) HasQueuedCount() bool`

HasQueuedCount returns a boolean if a field has been set.

### GetMessages

`func (o *SendVoiceMessageData) GetMessages() []VoiceMessage`

GetMessages returns the Messages field if non-nil, zero value otherwise.

### GetMessagesOk

`func (o *SendVoiceMessageData) GetMessagesOk() (*[]VoiceMessage, bool)`

GetMessagesOk returns a tuple with the Messages field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetMessages

`func (o *SendVoiceMessageData) SetMessages(v []VoiceMessage)`

SetMessages sets Messages field to given value.

### HasMessages

`func (o *SendVoiceMessageData) HasMessages() bool`

HasMessages returns a boolean if a field has been set.

### GetCurrency

`func (o *SendVoiceMessageData) GetCurrency() Currency`

GetCurrency returns the Currency field if non-nil, zero value otherwise.

### GetCurrencyOk

`func (o *SendVoiceMessageData) GetCurrencyOk() (*Currency, bool)`

GetCurrencyOk returns a tuple with the Currency field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCurrency

`func (o *SendVoiceMessageData) SetCurrency(v Currency)`

SetCurrency sets Currency field to given value.

### HasCurrency

`func (o *SendVoiceMessageData) HasCurrency() bool`

HasCurrency returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


