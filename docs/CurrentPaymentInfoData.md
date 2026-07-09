# CurrentPaymentInfoData

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**DisplayNumber** | Pointer to **string** | The credit card number. | [optional] 
**ExpiryMonth** | Pointer to **int32** | The credit card expiry month. | [optional] 
**ExpiryYear** | Pointer to **int32** | The credit card expiry year. | [optional] 
**Name** | Pointer to **string** | The credit card name. | [optional] 

## Methods

### NewCurrentPaymentInfoData

`func NewCurrentPaymentInfoData() *CurrentPaymentInfoData`

NewCurrentPaymentInfoData instantiates a new CurrentPaymentInfoData object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewCurrentPaymentInfoDataWithDefaults

`func NewCurrentPaymentInfoDataWithDefaults() *CurrentPaymentInfoData`

NewCurrentPaymentInfoDataWithDefaults instantiates a new CurrentPaymentInfoData object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetDisplayNumber

`func (o *CurrentPaymentInfoData) GetDisplayNumber() string`

GetDisplayNumber returns the DisplayNumber field if non-nil, zero value otherwise.

### GetDisplayNumberOk

`func (o *CurrentPaymentInfoData) GetDisplayNumberOk() (*string, bool)`

GetDisplayNumberOk returns a tuple with the DisplayNumber field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDisplayNumber

`func (o *CurrentPaymentInfoData) SetDisplayNumber(v string)`

SetDisplayNumber sets DisplayNumber field to given value.

### HasDisplayNumber

`func (o *CurrentPaymentInfoData) HasDisplayNumber() bool`

HasDisplayNumber returns a boolean if a field has been set.

### GetExpiryMonth

`func (o *CurrentPaymentInfoData) GetExpiryMonth() int32`

GetExpiryMonth returns the ExpiryMonth field if non-nil, zero value otherwise.

### GetExpiryMonthOk

`func (o *CurrentPaymentInfoData) GetExpiryMonthOk() (*int32, bool)`

GetExpiryMonthOk returns a tuple with the ExpiryMonth field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetExpiryMonth

`func (o *CurrentPaymentInfoData) SetExpiryMonth(v int32)`

SetExpiryMonth sets ExpiryMonth field to given value.

### HasExpiryMonth

`func (o *CurrentPaymentInfoData) HasExpiryMonth() bool`

HasExpiryMonth returns a boolean if a field has been set.

### GetExpiryYear

`func (o *CurrentPaymentInfoData) GetExpiryYear() int32`

GetExpiryYear returns the ExpiryYear field if non-nil, zero value otherwise.

### GetExpiryYearOk

`func (o *CurrentPaymentInfoData) GetExpiryYearOk() (*int32, bool)`

GetExpiryYearOk returns a tuple with the ExpiryYear field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetExpiryYear

`func (o *CurrentPaymentInfoData) SetExpiryYear(v int32)`

SetExpiryYear sets ExpiryYear field to given value.

### HasExpiryYear

`func (o *CurrentPaymentInfoData) HasExpiryYear() bool`

HasExpiryYear returns a boolean if a field has been set.

### GetName

`func (o *CurrentPaymentInfoData) GetName() string`

GetName returns the Name field if non-nil, zero value otherwise.

### GetNameOk

`func (o *CurrentPaymentInfoData) GetNameOk() (*string, bool)`

GetNameOk returns a tuple with the Name field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetName

`func (o *CurrentPaymentInfoData) SetName(v string)`

SetName sets Name field to given value.

### HasName

`func (o *CurrentPaymentInfoData) HasName() bool`

HasName returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


