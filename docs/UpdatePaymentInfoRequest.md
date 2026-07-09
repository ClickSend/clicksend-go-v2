# UpdatePaymentInfoRequest

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Number** | Pointer to **string** |  | [optional] 
**ExpiryMonth** | Pointer to **int32** |  | [optional] 
**ExpiryYear** | Pointer to **int32** |  | [optional] 
**Cvc** | Pointer to **int32** |  | [optional] 
**Name** | Pointer to **string** |  | [optional] 
**BankName** | Pointer to **string** |  | [optional] 

## Methods

### NewUpdatePaymentInfoRequest

`func NewUpdatePaymentInfoRequest() *UpdatePaymentInfoRequest`

NewUpdatePaymentInfoRequest instantiates a new UpdatePaymentInfoRequest object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewUpdatePaymentInfoRequestWithDefaults

`func NewUpdatePaymentInfoRequestWithDefaults() *UpdatePaymentInfoRequest`

NewUpdatePaymentInfoRequestWithDefaults instantiates a new UpdatePaymentInfoRequest object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetNumber

`func (o *UpdatePaymentInfoRequest) GetNumber() string`

GetNumber returns the Number field if non-nil, zero value otherwise.

### GetNumberOk

`func (o *UpdatePaymentInfoRequest) GetNumberOk() (*string, bool)`

GetNumberOk returns a tuple with the Number field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetNumber

`func (o *UpdatePaymentInfoRequest) SetNumber(v string)`

SetNumber sets Number field to given value.

### HasNumber

`func (o *UpdatePaymentInfoRequest) HasNumber() bool`

HasNumber returns a boolean if a field has been set.

### GetExpiryMonth

`func (o *UpdatePaymentInfoRequest) GetExpiryMonth() int32`

GetExpiryMonth returns the ExpiryMonth field if non-nil, zero value otherwise.

### GetExpiryMonthOk

`func (o *UpdatePaymentInfoRequest) GetExpiryMonthOk() (*int32, bool)`

GetExpiryMonthOk returns a tuple with the ExpiryMonth field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetExpiryMonth

`func (o *UpdatePaymentInfoRequest) SetExpiryMonth(v int32)`

SetExpiryMonth sets ExpiryMonth field to given value.

### HasExpiryMonth

`func (o *UpdatePaymentInfoRequest) HasExpiryMonth() bool`

HasExpiryMonth returns a boolean if a field has been set.

### GetExpiryYear

`func (o *UpdatePaymentInfoRequest) GetExpiryYear() int32`

GetExpiryYear returns the ExpiryYear field if non-nil, zero value otherwise.

### GetExpiryYearOk

`func (o *UpdatePaymentInfoRequest) GetExpiryYearOk() (*int32, bool)`

GetExpiryYearOk returns a tuple with the ExpiryYear field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetExpiryYear

`func (o *UpdatePaymentInfoRequest) SetExpiryYear(v int32)`

SetExpiryYear sets ExpiryYear field to given value.

### HasExpiryYear

`func (o *UpdatePaymentInfoRequest) HasExpiryYear() bool`

HasExpiryYear returns a boolean if a field has been set.

### GetCvc

`func (o *UpdatePaymentInfoRequest) GetCvc() int32`

GetCvc returns the Cvc field if non-nil, zero value otherwise.

### GetCvcOk

`func (o *UpdatePaymentInfoRequest) GetCvcOk() (*int32, bool)`

GetCvcOk returns a tuple with the Cvc field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCvc

`func (o *UpdatePaymentInfoRequest) SetCvc(v int32)`

SetCvc sets Cvc field to given value.

### HasCvc

`func (o *UpdatePaymentInfoRequest) HasCvc() bool`

HasCvc returns a boolean if a field has been set.

### GetName

`func (o *UpdatePaymentInfoRequest) GetName() string`

GetName returns the Name field if non-nil, zero value otherwise.

### GetNameOk

`func (o *UpdatePaymentInfoRequest) GetNameOk() (*string, bool)`

GetNameOk returns a tuple with the Name field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetName

`func (o *UpdatePaymentInfoRequest) SetName(v string)`

SetName sets Name field to given value.

### HasName

`func (o *UpdatePaymentInfoRequest) HasName() bool`

HasName returns a boolean if a field has been set.

### GetBankName

`func (o *UpdatePaymentInfoRequest) GetBankName() string`

GetBankName returns the BankName field if non-nil, zero value otherwise.

### GetBankNameOk

`func (o *UpdatePaymentInfoRequest) GetBankNameOk() (*string, bool)`

GetBankNameOk returns a tuple with the BankName field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetBankName

`func (o *UpdatePaymentInfoRequest) SetBankName(v string)`

SetBankName sets BankName field to given value.

### HasBankName

`func (o *UpdatePaymentInfoRequest) HasBankName() bool`

HasBankName returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


