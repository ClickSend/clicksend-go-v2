# SendFaxData

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**TotalPrice** | Pointer to **float32** | The total price of the fax. | [optional] 
**TotalCount** | Pointer to **string** | The total count of the fax. | [optional] 
**QueuedCount** | Pointer to **string** | The count of the queued fax. | [optional] 
**Messages** | Pointer to [**[]Fax**](Fax.md) | The list of messages that were sent. | [optional] 
**Currency** | Pointer to [**Currency**](Currency.md) |  | [optional] 

## Methods

### NewSendFaxData

`func NewSendFaxData() *SendFaxData`

NewSendFaxData instantiates a new SendFaxData object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewSendFaxDataWithDefaults

`func NewSendFaxDataWithDefaults() *SendFaxData`

NewSendFaxDataWithDefaults instantiates a new SendFaxData object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetTotalPrice

`func (o *SendFaxData) GetTotalPrice() float32`

GetTotalPrice returns the TotalPrice field if non-nil, zero value otherwise.

### GetTotalPriceOk

`func (o *SendFaxData) GetTotalPriceOk() (*float32, bool)`

GetTotalPriceOk returns a tuple with the TotalPrice field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTotalPrice

`func (o *SendFaxData) SetTotalPrice(v float32)`

SetTotalPrice sets TotalPrice field to given value.

### HasTotalPrice

`func (o *SendFaxData) HasTotalPrice() bool`

HasTotalPrice returns a boolean if a field has been set.

### GetTotalCount

`func (o *SendFaxData) GetTotalCount() string`

GetTotalCount returns the TotalCount field if non-nil, zero value otherwise.

### GetTotalCountOk

`func (o *SendFaxData) GetTotalCountOk() (*string, bool)`

GetTotalCountOk returns a tuple with the TotalCount field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTotalCount

`func (o *SendFaxData) SetTotalCount(v string)`

SetTotalCount sets TotalCount field to given value.

### HasTotalCount

`func (o *SendFaxData) HasTotalCount() bool`

HasTotalCount returns a boolean if a field has been set.

### GetQueuedCount

`func (o *SendFaxData) GetQueuedCount() string`

GetQueuedCount returns the QueuedCount field if non-nil, zero value otherwise.

### GetQueuedCountOk

`func (o *SendFaxData) GetQueuedCountOk() (*string, bool)`

GetQueuedCountOk returns a tuple with the QueuedCount field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetQueuedCount

`func (o *SendFaxData) SetQueuedCount(v string)`

SetQueuedCount sets QueuedCount field to given value.

### HasQueuedCount

`func (o *SendFaxData) HasQueuedCount() bool`

HasQueuedCount returns a boolean if a field has been set.

### GetMessages

`func (o *SendFaxData) GetMessages() []Fax`

GetMessages returns the Messages field if non-nil, zero value otherwise.

### GetMessagesOk

`func (o *SendFaxData) GetMessagesOk() (*[]Fax, bool)`

GetMessagesOk returns a tuple with the Messages field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetMessages

`func (o *SendFaxData) SetMessages(v []Fax)`

SetMessages sets Messages field to given value.

### HasMessages

`func (o *SendFaxData) HasMessages() bool`

HasMessages returns a boolean if a field has been set.

### GetCurrency

`func (o *SendFaxData) GetCurrency() Currency`

GetCurrency returns the Currency field if non-nil, zero value otherwise.

### GetCurrencyOk

`func (o *SendFaxData) GetCurrencyOk() (*Currency, bool)`

GetCurrencyOk returns a tuple with the Currency field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCurrency

`func (o *SendFaxData) SetCurrency(v Currency)`

SetCurrency sets Currency field to given value.

### HasCurrency

`func (o *SendFaxData) HasCurrency() bool`

HasCurrency returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


