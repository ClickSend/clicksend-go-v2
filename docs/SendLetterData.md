# SendLetterData

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Recipients** | Pointer to [**[]Recipient**](Recipient.md) |  | [optional] 
**Currency** | Pointer to [**Currency**](Currency.md) |  | [optional] 

## Methods

### NewSendLetterData

`func NewSendLetterData() *SendLetterData`

NewSendLetterData instantiates a new SendLetterData object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewSendLetterDataWithDefaults

`func NewSendLetterDataWithDefaults() *SendLetterData`

NewSendLetterDataWithDefaults instantiates a new SendLetterData object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetRecipients

`func (o *SendLetterData) GetRecipients() []Recipient`

GetRecipients returns the Recipients field if non-nil, zero value otherwise.

### GetRecipientsOk

`func (o *SendLetterData) GetRecipientsOk() (*[]Recipient, bool)`

GetRecipientsOk returns a tuple with the Recipients field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetRecipients

`func (o *SendLetterData) SetRecipients(v []Recipient)`

SetRecipients sets Recipients field to given value.

### HasRecipients

`func (o *SendLetterData) HasRecipients() bool`

HasRecipients returns a boolean if a field has been set.

### GetCurrency

`func (o *SendLetterData) GetCurrency() Currency`

GetCurrency returns the Currency field if non-nil, zero value otherwise.

### GetCurrencyOk

`func (o *SendLetterData) GetCurrencyOk() (*Currency, bool)`

GetCurrencyOk returns a tuple with the Currency field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCurrency

`func (o *SendLetterData) SetCurrency(v Currency)`

SetCurrency sets Currency field to given value.

### HasCurrency

`func (o *SendLetterData) HasCurrency() bool`

HasCurrency returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


