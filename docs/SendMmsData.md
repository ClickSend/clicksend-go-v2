# SendMmsData

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**TotalPrice** | Pointer to **float32** | The total price of the MMS messages. | [optional] 
**TotalCount** | Pointer to **int32** | The total count of the MMS messages. | [optional] 
**QueuedCount** | Pointer to **int32** | The count of the queued MMS messages. | [optional] 
**Messages** | Pointer to [**[]Mms**](Mms.md) |  | [optional] 

## Methods

### NewSendMmsData

`func NewSendMmsData() *SendMmsData`

NewSendMmsData instantiates a new SendMmsData object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewSendMmsDataWithDefaults

`func NewSendMmsDataWithDefaults() *SendMmsData`

NewSendMmsDataWithDefaults instantiates a new SendMmsData object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetTotalPrice

`func (o *SendMmsData) GetTotalPrice() float32`

GetTotalPrice returns the TotalPrice field if non-nil, zero value otherwise.

### GetTotalPriceOk

`func (o *SendMmsData) GetTotalPriceOk() (*float32, bool)`

GetTotalPriceOk returns a tuple with the TotalPrice field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTotalPrice

`func (o *SendMmsData) SetTotalPrice(v float32)`

SetTotalPrice sets TotalPrice field to given value.

### HasTotalPrice

`func (o *SendMmsData) HasTotalPrice() bool`

HasTotalPrice returns a boolean if a field has been set.

### GetTotalCount

`func (o *SendMmsData) GetTotalCount() int32`

GetTotalCount returns the TotalCount field if non-nil, zero value otherwise.

### GetTotalCountOk

`func (o *SendMmsData) GetTotalCountOk() (*int32, bool)`

GetTotalCountOk returns a tuple with the TotalCount field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTotalCount

`func (o *SendMmsData) SetTotalCount(v int32)`

SetTotalCount sets TotalCount field to given value.

### HasTotalCount

`func (o *SendMmsData) HasTotalCount() bool`

HasTotalCount returns a boolean if a field has been set.

### GetQueuedCount

`func (o *SendMmsData) GetQueuedCount() int32`

GetQueuedCount returns the QueuedCount field if non-nil, zero value otherwise.

### GetQueuedCountOk

`func (o *SendMmsData) GetQueuedCountOk() (*int32, bool)`

GetQueuedCountOk returns a tuple with the QueuedCount field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetQueuedCount

`func (o *SendMmsData) SetQueuedCount(v int32)`

SetQueuedCount sets QueuedCount field to given value.

### HasQueuedCount

`func (o *SendMmsData) HasQueuedCount() bool`

HasQueuedCount returns a boolean if a field has been set.

### GetMessages

`func (o *SendMmsData) GetMessages() []Mms`

GetMessages returns the Messages field if non-nil, zero value otherwise.

### GetMessagesOk

`func (o *SendMmsData) GetMessagesOk() (*[]Mms, bool)`

GetMessagesOk returns a tuple with the Messages field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetMessages

`func (o *SendMmsData) SetMessages(v []Mms)`

SetMessages sets Messages field to given value.

### HasMessages

`func (o *SendMmsData) HasMessages() bool`

HasMessages returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


