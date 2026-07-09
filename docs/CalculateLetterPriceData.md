# CalculateLetterPriceData

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**TotalPrice** | Pointer to **float32** | The total price of the letter. | [optional] 
**TotalCost** | Pointer to **float32** | The total cost of the letter. | [optional] 
**Recipients** | Pointer to [**[]Recipient**](Recipient.md) |  | [optional] 

## Methods

### NewCalculateLetterPriceData

`func NewCalculateLetterPriceData() *CalculateLetterPriceData`

NewCalculateLetterPriceData instantiates a new CalculateLetterPriceData object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewCalculateLetterPriceDataWithDefaults

`func NewCalculateLetterPriceDataWithDefaults() *CalculateLetterPriceData`

NewCalculateLetterPriceDataWithDefaults instantiates a new CalculateLetterPriceData object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetTotalPrice

`func (o *CalculateLetterPriceData) GetTotalPrice() float32`

GetTotalPrice returns the TotalPrice field if non-nil, zero value otherwise.

### GetTotalPriceOk

`func (o *CalculateLetterPriceData) GetTotalPriceOk() (*float32, bool)`

GetTotalPriceOk returns a tuple with the TotalPrice field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTotalPrice

`func (o *CalculateLetterPriceData) SetTotalPrice(v float32)`

SetTotalPrice sets TotalPrice field to given value.

### HasTotalPrice

`func (o *CalculateLetterPriceData) HasTotalPrice() bool`

HasTotalPrice returns a boolean if a field has been set.

### GetTotalCost

`func (o *CalculateLetterPriceData) GetTotalCost() float32`

GetTotalCost returns the TotalCost field if non-nil, zero value otherwise.

### GetTotalCostOk

`func (o *CalculateLetterPriceData) GetTotalCostOk() (*float32, bool)`

GetTotalCostOk returns a tuple with the TotalCost field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTotalCost

`func (o *CalculateLetterPriceData) SetTotalCost(v float32)`

SetTotalCost sets TotalCost field to given value.

### HasTotalCost

`func (o *CalculateLetterPriceData) HasTotalCost() bool`

HasTotalCost returns a boolean if a field has been set.

### GetRecipients

`func (o *CalculateLetterPriceData) GetRecipients() []Recipient`

GetRecipients returns the Recipients field if non-nil, zero value otherwise.

### GetRecipientsOk

`func (o *CalculateLetterPriceData) GetRecipientsOk() (*[]Recipient, bool)`

GetRecipientsOk returns a tuple with the Recipients field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetRecipients

`func (o *CalculateLetterPriceData) SetRecipients(v []Recipient)`

SetRecipients sets Recipients field to given value.

### HasRecipients

`func (o *CalculateLetterPriceData) HasRecipients() bool`

HasRecipients returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


