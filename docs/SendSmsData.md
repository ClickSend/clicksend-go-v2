# SendSmsData

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**TotalPrice** | Pointer to **float32** | The total price of sending the messages. Visit [this page](/#status-codes) for more information. | [optional] 
**TotalCount** | Pointer to **int32** | The total number of messages sent from the request. | [optional] 
**QueuedCount** | Pointer to **int32** | The messages will be put in a queue if it goes through the validation process. The validation process checks whether the **Sender ID** is registered or not. Some countries don&#39;t require messages to go through the validation process.  Messages scheduled to be sent right away will be sent immediately. If not, it will be queued. | [optional] 
**Messages** | Pointer to [**[]SmsSendSms**](SmsSendSms.md) | The parameters related to messages. | [optional] 
**Currency** | Pointer to [**Currency**](Currency.md) |  | [optional] 
**BlockedCount** | Pointer to **int32** | The number of messages unable to be sent. This is often caused by:  - Receipient’s country not enabled for &lt;a href&#x3D;\&quot;https://help.clicksend.com/article/qdavyt16qs-global-sending\&quot;&gt;global sending&lt;/a&gt;.      - **Sender ID** resitriction.      - Number registration restrcition. | [optional] 

## Methods

### NewSendSmsData

`func NewSendSmsData() *SendSmsData`

NewSendSmsData instantiates a new SendSmsData object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewSendSmsDataWithDefaults

`func NewSendSmsDataWithDefaults() *SendSmsData`

NewSendSmsDataWithDefaults instantiates a new SendSmsData object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetTotalPrice

`func (o *SendSmsData) GetTotalPrice() float32`

GetTotalPrice returns the TotalPrice field if non-nil, zero value otherwise.

### GetTotalPriceOk

`func (o *SendSmsData) GetTotalPriceOk() (*float32, bool)`

GetTotalPriceOk returns a tuple with the TotalPrice field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTotalPrice

`func (o *SendSmsData) SetTotalPrice(v float32)`

SetTotalPrice sets TotalPrice field to given value.

### HasTotalPrice

`func (o *SendSmsData) HasTotalPrice() bool`

HasTotalPrice returns a boolean if a field has been set.

### GetTotalCount

`func (o *SendSmsData) GetTotalCount() int32`

GetTotalCount returns the TotalCount field if non-nil, zero value otherwise.

### GetTotalCountOk

`func (o *SendSmsData) GetTotalCountOk() (*int32, bool)`

GetTotalCountOk returns a tuple with the TotalCount field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTotalCount

`func (o *SendSmsData) SetTotalCount(v int32)`

SetTotalCount sets TotalCount field to given value.

### HasTotalCount

`func (o *SendSmsData) HasTotalCount() bool`

HasTotalCount returns a boolean if a field has been set.

### GetQueuedCount

`func (o *SendSmsData) GetQueuedCount() int32`

GetQueuedCount returns the QueuedCount field if non-nil, zero value otherwise.

### GetQueuedCountOk

`func (o *SendSmsData) GetQueuedCountOk() (*int32, bool)`

GetQueuedCountOk returns a tuple with the QueuedCount field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetQueuedCount

`func (o *SendSmsData) SetQueuedCount(v int32)`

SetQueuedCount sets QueuedCount field to given value.

### HasQueuedCount

`func (o *SendSmsData) HasQueuedCount() bool`

HasQueuedCount returns a boolean if a field has been set.

### GetMessages

`func (o *SendSmsData) GetMessages() []SmsSendSms`

GetMessages returns the Messages field if non-nil, zero value otherwise.

### GetMessagesOk

`func (o *SendSmsData) GetMessagesOk() (*[]SmsSendSms, bool)`

GetMessagesOk returns a tuple with the Messages field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetMessages

`func (o *SendSmsData) SetMessages(v []SmsSendSms)`

SetMessages sets Messages field to given value.

### HasMessages

`func (o *SendSmsData) HasMessages() bool`

HasMessages returns a boolean if a field has been set.

### GetCurrency

`func (o *SendSmsData) GetCurrency() Currency`

GetCurrency returns the Currency field if non-nil, zero value otherwise.

### GetCurrencyOk

`func (o *SendSmsData) GetCurrencyOk() (*Currency, bool)`

GetCurrencyOk returns a tuple with the Currency field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCurrency

`func (o *SendSmsData) SetCurrency(v Currency)`

SetCurrency sets Currency field to given value.

### HasCurrency

`func (o *SendSmsData) HasCurrency() bool`

HasCurrency returns a boolean if a field has been set.

### GetBlockedCount

`func (o *SendSmsData) GetBlockedCount() int32`

GetBlockedCount returns the BlockedCount field if non-nil, zero value otherwise.

### GetBlockedCountOk

`func (o *SendSmsData) GetBlockedCountOk() (*int32, bool)`

GetBlockedCountOk returns a tuple with the BlockedCount field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetBlockedCount

`func (o *SendSmsData) SetBlockedCount(v int32)`

SetBlockedCount sets BlockedCount field to given value.

### HasBlockedCount

`func (o *SendSmsData) HasBlockedCount() bool`

HasBlockedCount returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


