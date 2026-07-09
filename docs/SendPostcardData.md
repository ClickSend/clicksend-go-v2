# SendPostcardData

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**TotalPrice** | Pointer to **float32** | The total price of the postcard. | [optional] 
**TotalCount** | Pointer to **int32** | The total count of the postcard. | [optional] 
**QueuedCount** | Pointer to **int32** | The count of the queued postcard. | [optional] 
**Recipients** | Pointer to [**[]PostcardRecipient**](PostcardRecipient.md) |  | [optional] 
**Currency** | Pointer to [**Currency**](Currency.md) |  | [optional] 

## Methods

### NewSendPostcardData

`func NewSendPostcardData() *SendPostcardData`

NewSendPostcardData instantiates a new SendPostcardData object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewSendPostcardDataWithDefaults

`func NewSendPostcardDataWithDefaults() *SendPostcardData`

NewSendPostcardDataWithDefaults instantiates a new SendPostcardData object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetTotalPrice

`func (o *SendPostcardData) GetTotalPrice() float32`

GetTotalPrice returns the TotalPrice field if non-nil, zero value otherwise.

### GetTotalPriceOk

`func (o *SendPostcardData) GetTotalPriceOk() (*float32, bool)`

GetTotalPriceOk returns a tuple with the TotalPrice field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTotalPrice

`func (o *SendPostcardData) SetTotalPrice(v float32)`

SetTotalPrice sets TotalPrice field to given value.

### HasTotalPrice

`func (o *SendPostcardData) HasTotalPrice() bool`

HasTotalPrice returns a boolean if a field has been set.

### GetTotalCount

`func (o *SendPostcardData) GetTotalCount() int32`

GetTotalCount returns the TotalCount field if non-nil, zero value otherwise.

### GetTotalCountOk

`func (o *SendPostcardData) GetTotalCountOk() (*int32, bool)`

GetTotalCountOk returns a tuple with the TotalCount field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTotalCount

`func (o *SendPostcardData) SetTotalCount(v int32)`

SetTotalCount sets TotalCount field to given value.

### HasTotalCount

`func (o *SendPostcardData) HasTotalCount() bool`

HasTotalCount returns a boolean if a field has been set.

### GetQueuedCount

`func (o *SendPostcardData) GetQueuedCount() int32`

GetQueuedCount returns the QueuedCount field if non-nil, zero value otherwise.

### GetQueuedCountOk

`func (o *SendPostcardData) GetQueuedCountOk() (*int32, bool)`

GetQueuedCountOk returns a tuple with the QueuedCount field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetQueuedCount

`func (o *SendPostcardData) SetQueuedCount(v int32)`

SetQueuedCount sets QueuedCount field to given value.

### HasQueuedCount

`func (o *SendPostcardData) HasQueuedCount() bool`

HasQueuedCount returns a boolean if a field has been set.

### GetRecipients

`func (o *SendPostcardData) GetRecipients() []PostcardRecipient`

GetRecipients returns the Recipients field if non-nil, zero value otherwise.

### GetRecipientsOk

`func (o *SendPostcardData) GetRecipientsOk() (*[]PostcardRecipient, bool)`

GetRecipientsOk returns a tuple with the Recipients field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetRecipients

`func (o *SendPostcardData) SetRecipients(v []PostcardRecipient)`

SetRecipients sets Recipients field to given value.

### HasRecipients

`func (o *SendPostcardData) HasRecipients() bool`

HasRecipients returns a boolean if a field has been set.

### GetCurrency

`func (o *SendPostcardData) GetCurrency() Currency`

GetCurrency returns the Currency field if non-nil, zero value otherwise.

### GetCurrencyOk

`func (o *SendPostcardData) GetCurrencyOk() (*Currency, bool)`

GetCurrencyOk returns a tuple with the Currency field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCurrency

`func (o *SendPostcardData) SetCurrency(v Currency)`

SetCurrency sets Currency field to given value.

### HasCurrency

`func (o *SendPostcardData) HasCurrency() bool`

HasCurrency returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


