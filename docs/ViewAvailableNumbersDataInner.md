# ViewAvailableNumbersDataInner

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Country** | Pointer to **string** | The country code of the number. | [optional] 
**CountryName** | Pointer to **string** | The country name of the number. | [optional] 
**DedicatedNumber** | Pointer to **string** | The dedicated number. | [optional] 
**PriceSetup** | Pointer to **string** | The setup price of the number. | [optional] 
**PriceMonthly** | Pointer to **string** | The monthly price of the number. | [optional] 
**PriceTotal** | Pointer to **string** | The total price of the number. | [optional] 
**AddressRequirement** | Pointer to **NullableString** | The address requirement for the number.  &lt;br&gt; &#x60;local&#x60;: requires an address that corresponds  to the phone number&#39;s prefix. | [optional] 

## Methods

### NewViewAvailableNumbersDataInner

`func NewViewAvailableNumbersDataInner() *ViewAvailableNumbersDataInner`

NewViewAvailableNumbersDataInner instantiates a new ViewAvailableNumbersDataInner object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewViewAvailableNumbersDataInnerWithDefaults

`func NewViewAvailableNumbersDataInnerWithDefaults() *ViewAvailableNumbersDataInner`

NewViewAvailableNumbersDataInnerWithDefaults instantiates a new ViewAvailableNumbersDataInner object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetCountry

`func (o *ViewAvailableNumbersDataInner) GetCountry() string`

GetCountry returns the Country field if non-nil, zero value otherwise.

### GetCountryOk

`func (o *ViewAvailableNumbersDataInner) GetCountryOk() (*string, bool)`

GetCountryOk returns a tuple with the Country field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCountry

`func (o *ViewAvailableNumbersDataInner) SetCountry(v string)`

SetCountry sets Country field to given value.

### HasCountry

`func (o *ViewAvailableNumbersDataInner) HasCountry() bool`

HasCountry returns a boolean if a field has been set.

### GetCountryName

`func (o *ViewAvailableNumbersDataInner) GetCountryName() string`

GetCountryName returns the CountryName field if non-nil, zero value otherwise.

### GetCountryNameOk

`func (o *ViewAvailableNumbersDataInner) GetCountryNameOk() (*string, bool)`

GetCountryNameOk returns a tuple with the CountryName field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCountryName

`func (o *ViewAvailableNumbersDataInner) SetCountryName(v string)`

SetCountryName sets CountryName field to given value.

### HasCountryName

`func (o *ViewAvailableNumbersDataInner) HasCountryName() bool`

HasCountryName returns a boolean if a field has been set.

### GetDedicatedNumber

`func (o *ViewAvailableNumbersDataInner) GetDedicatedNumber() string`

GetDedicatedNumber returns the DedicatedNumber field if non-nil, zero value otherwise.

### GetDedicatedNumberOk

`func (o *ViewAvailableNumbersDataInner) GetDedicatedNumberOk() (*string, bool)`

GetDedicatedNumberOk returns a tuple with the DedicatedNumber field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDedicatedNumber

`func (o *ViewAvailableNumbersDataInner) SetDedicatedNumber(v string)`

SetDedicatedNumber sets DedicatedNumber field to given value.

### HasDedicatedNumber

`func (o *ViewAvailableNumbersDataInner) HasDedicatedNumber() bool`

HasDedicatedNumber returns a boolean if a field has been set.

### GetPriceSetup

`func (o *ViewAvailableNumbersDataInner) GetPriceSetup() string`

GetPriceSetup returns the PriceSetup field if non-nil, zero value otherwise.

### GetPriceSetupOk

`func (o *ViewAvailableNumbersDataInner) GetPriceSetupOk() (*string, bool)`

GetPriceSetupOk returns a tuple with the PriceSetup field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetPriceSetup

`func (o *ViewAvailableNumbersDataInner) SetPriceSetup(v string)`

SetPriceSetup sets PriceSetup field to given value.

### HasPriceSetup

`func (o *ViewAvailableNumbersDataInner) HasPriceSetup() bool`

HasPriceSetup returns a boolean if a field has been set.

### GetPriceMonthly

`func (o *ViewAvailableNumbersDataInner) GetPriceMonthly() string`

GetPriceMonthly returns the PriceMonthly field if non-nil, zero value otherwise.

### GetPriceMonthlyOk

`func (o *ViewAvailableNumbersDataInner) GetPriceMonthlyOk() (*string, bool)`

GetPriceMonthlyOk returns a tuple with the PriceMonthly field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetPriceMonthly

`func (o *ViewAvailableNumbersDataInner) SetPriceMonthly(v string)`

SetPriceMonthly sets PriceMonthly field to given value.

### HasPriceMonthly

`func (o *ViewAvailableNumbersDataInner) HasPriceMonthly() bool`

HasPriceMonthly returns a boolean if a field has been set.

### GetPriceTotal

`func (o *ViewAvailableNumbersDataInner) GetPriceTotal() string`

GetPriceTotal returns the PriceTotal field if non-nil, zero value otherwise.

### GetPriceTotalOk

`func (o *ViewAvailableNumbersDataInner) GetPriceTotalOk() (*string, bool)`

GetPriceTotalOk returns a tuple with the PriceTotal field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetPriceTotal

`func (o *ViewAvailableNumbersDataInner) SetPriceTotal(v string)`

SetPriceTotal sets PriceTotal field to given value.

### HasPriceTotal

`func (o *ViewAvailableNumbersDataInner) HasPriceTotal() bool`

HasPriceTotal returns a boolean if a field has been set.

### GetAddressRequirement

`func (o *ViewAvailableNumbersDataInner) GetAddressRequirement() string`

GetAddressRequirement returns the AddressRequirement field if non-nil, zero value otherwise.

### GetAddressRequirementOk

`func (o *ViewAvailableNumbersDataInner) GetAddressRequirementOk() (*string, bool)`

GetAddressRequirementOk returns a tuple with the AddressRequirement field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAddressRequirement

`func (o *ViewAvailableNumbersDataInner) SetAddressRequirement(v string)`

SetAddressRequirement sets AddressRequirement field to given value.

### HasAddressRequirement

`func (o *ViewAvailableNumbersDataInner) HasAddressRequirement() bool`

HasAddressRequirement returns a boolean if a field has been set.

### SetAddressRequirementNil

`func (o *ViewAvailableNumbersDataInner) SetAddressRequirementNil(b bool)`

 SetAddressRequirementNil sets the value for AddressRequirement to be an explicit nil

### UnsetAddressRequirement
`func (o *ViewAvailableNumbersDataInner) UnsetAddressRequirement()`

UnsetAddressRequirement ensures that no value is present for AddressRequirement, not even an explicit nil

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


