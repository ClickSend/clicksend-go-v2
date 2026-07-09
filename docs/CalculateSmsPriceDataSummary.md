# CalculateSmsPriceDataSummary

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**TestMessage** | Pointer to **string** | This parameter is used for internal developers. This is used when your account is in trial period. | [optional] 
**Countries** | Pointer to [**[]CalculateSmsPriceDataSummaryCountriesInner**](CalculateSmsPriceDataSummaryCountriesInner.md) | The list of countries of the receipients in two-letter format (e.g. US, UK, AU, NZ, etc). | [optional] 

## Methods

### NewCalculateSmsPriceDataSummary

`func NewCalculateSmsPriceDataSummary() *CalculateSmsPriceDataSummary`

NewCalculateSmsPriceDataSummary instantiates a new CalculateSmsPriceDataSummary object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewCalculateSmsPriceDataSummaryWithDefaults

`func NewCalculateSmsPriceDataSummaryWithDefaults() *CalculateSmsPriceDataSummary`

NewCalculateSmsPriceDataSummaryWithDefaults instantiates a new CalculateSmsPriceDataSummary object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetTestMessage

`func (o *CalculateSmsPriceDataSummary) GetTestMessage() string`

GetTestMessage returns the TestMessage field if non-nil, zero value otherwise.

### GetTestMessageOk

`func (o *CalculateSmsPriceDataSummary) GetTestMessageOk() (*string, bool)`

GetTestMessageOk returns a tuple with the TestMessage field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTestMessage

`func (o *CalculateSmsPriceDataSummary) SetTestMessage(v string)`

SetTestMessage sets TestMessage field to given value.

### HasTestMessage

`func (o *CalculateSmsPriceDataSummary) HasTestMessage() bool`

HasTestMessage returns a boolean if a field has been set.

### GetCountries

`func (o *CalculateSmsPriceDataSummary) GetCountries() []CalculateSmsPriceDataSummaryCountriesInner`

GetCountries returns the Countries field if non-nil, zero value otherwise.

### GetCountriesOk

`func (o *CalculateSmsPriceDataSummary) GetCountriesOk() (*[]CalculateSmsPriceDataSummaryCountriesInner, bool)`

GetCountriesOk returns a tuple with the Countries field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCountries

`func (o *CalculateSmsPriceDataSummary) SetCountries(v []CalculateSmsPriceDataSummaryCountriesInner)`

SetCountries sets Countries field to given value.

### HasCountries

`func (o *CalculateSmsPriceDataSummary) HasCountries() bool`

HasCountries returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


