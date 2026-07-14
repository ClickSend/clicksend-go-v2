# Currency

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**CurrencyNameShort** | Pointer to **string** | The currency used for the sender in three-letter format (e.g. USD, EUR, AUD, NZD, etc). | [optional] 
**CurrencyPrefixD** | Pointer to **string** | The symbol used to indicate the currency of the sender (e.g. $ , €, etc). | [optional] 
**CurrencyPrefixC** | Pointer to **string** | The currency basic unit (e.g. cents). | [optional] 
**CurrencyNameLong** | Pointer to **string** | The full name of the currency. | [optional] 
**MinRechargeAmount** | Pointer to **string** | The minimum amount that can be used to recharge the account, in this currency. | [optional] 
**MaxRechargeAmount** | Pointer to **string** | The maximum amount that can be used to recharge the account, in this currency. | [optional] 

## Methods

### NewCurrency

`func NewCurrency() *Currency`

NewCurrency instantiates a new Currency object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewCurrencyWithDefaults

`func NewCurrencyWithDefaults() *Currency`

NewCurrencyWithDefaults instantiates a new Currency object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetCurrencyNameShort

`func (o *Currency) GetCurrencyNameShort() string`

GetCurrencyNameShort returns the CurrencyNameShort field if non-nil, zero value otherwise.

### GetCurrencyNameShortOk

`func (o *Currency) GetCurrencyNameShortOk() (*string, bool)`

GetCurrencyNameShortOk returns a tuple with the CurrencyNameShort field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCurrencyNameShort

`func (o *Currency) SetCurrencyNameShort(v string)`

SetCurrencyNameShort sets CurrencyNameShort field to given value.

### HasCurrencyNameShort

`func (o *Currency) HasCurrencyNameShort() bool`

HasCurrencyNameShort returns a boolean if a field has been set.

### GetCurrencyPrefixD

`func (o *Currency) GetCurrencyPrefixD() string`

GetCurrencyPrefixD returns the CurrencyPrefixD field if non-nil, zero value otherwise.

### GetCurrencyPrefixDOk

`func (o *Currency) GetCurrencyPrefixDOk() (*string, bool)`

GetCurrencyPrefixDOk returns a tuple with the CurrencyPrefixD field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCurrencyPrefixD

`func (o *Currency) SetCurrencyPrefixD(v string)`

SetCurrencyPrefixD sets CurrencyPrefixD field to given value.

### HasCurrencyPrefixD

`func (o *Currency) HasCurrencyPrefixD() bool`

HasCurrencyPrefixD returns a boolean if a field has been set.

### GetCurrencyPrefixC

`func (o *Currency) GetCurrencyPrefixC() string`

GetCurrencyPrefixC returns the CurrencyPrefixC field if non-nil, zero value otherwise.

### GetCurrencyPrefixCOk

`func (o *Currency) GetCurrencyPrefixCOk() (*string, bool)`

GetCurrencyPrefixCOk returns a tuple with the CurrencyPrefixC field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCurrencyPrefixC

`func (o *Currency) SetCurrencyPrefixC(v string)`

SetCurrencyPrefixC sets CurrencyPrefixC field to given value.

### HasCurrencyPrefixC

`func (o *Currency) HasCurrencyPrefixC() bool`

HasCurrencyPrefixC returns a boolean if a field has been set.

### GetCurrencyNameLong

`func (o *Currency) GetCurrencyNameLong() string`

GetCurrencyNameLong returns the CurrencyNameLong field if non-nil, zero value otherwise.

### GetCurrencyNameLongOk

`func (o *Currency) GetCurrencyNameLongOk() (*string, bool)`

GetCurrencyNameLongOk returns a tuple with the CurrencyNameLong field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCurrencyNameLong

`func (o *Currency) SetCurrencyNameLong(v string)`

SetCurrencyNameLong sets CurrencyNameLong field to given value.

### HasCurrencyNameLong

`func (o *Currency) HasCurrencyNameLong() bool`

HasCurrencyNameLong returns a boolean if a field has been set.

### GetMinRechargeAmount

`func (o *Currency) GetMinRechargeAmount() string`

GetMinRechargeAmount returns the MinRechargeAmount field if non-nil, zero value otherwise.

### GetMinRechargeAmountOk

`func (o *Currency) GetMinRechargeAmountOk() (*string, bool)`

GetMinRechargeAmountOk returns a tuple with the MinRechargeAmount field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetMinRechargeAmount

`func (o *Currency) SetMinRechargeAmount(v string)`

SetMinRechargeAmount sets MinRechargeAmount field to given value.

### HasMinRechargeAmount

`func (o *Currency) HasMinRechargeAmount() bool`

HasMinRechargeAmount returns a boolean if a field has been set.

### GetMaxRechargeAmount

`func (o *Currency) GetMaxRechargeAmount() string`

GetMaxRechargeAmount returns the MaxRechargeAmount field if non-nil, zero value otherwise.

### GetMaxRechargeAmountOk

`func (o *Currency) GetMaxRechargeAmountOk() (*string, bool)`

GetMaxRechargeAmountOk returns a tuple with the MaxRechargeAmount field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetMaxRechargeAmount

`func (o *Currency) SetMaxRechargeAmount(v string)`

SetMaxRechargeAmount sets MaxRechargeAmount field to given value.

### HasMaxRechargeAmount

`func (o *Currency) HasMaxRechargeAmount() bool`

HasMaxRechargeAmount returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


