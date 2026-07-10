# ViewAvailableNumbersDataAllOfDataInner

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

### NewViewAvailableNumbersDataAllOfDataInner

`func NewViewAvailableNumbersDataAllOfDataInner() *ViewAvailableNumbersDataAllOfDataInner`

NewViewAvailableNumbersDataAllOfDataInner instantiates a new ViewAvailableNumbersDataAllOfDataInner object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewViewAvailableNumbersDataAllOfDataInnerWithDefaults

`func NewViewAvailableNumbersDataAllOfDataInnerWithDefaults() *ViewAvailableNumbersDataAllOfDataInner`

NewViewAvailableNumbersDataAllOfDataInnerWithDefaults instantiates a new ViewAvailableNumbersDataAllOfDataInner object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetCountry

`func (o *ViewAvailableNumbersDataAllOfDataInner) GetCountry() string`

GetCountry returns the Country field if non-nil, zero value otherwise.

### GetCountryOk

`func (o *ViewAvailableNumbersDataAllOfDataInner) GetCountryOk() (*string, bool)`

GetCountryOk returns a tuple with the Country field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCountry

`func (o *ViewAvailableNumbersDataAllOfDataInner) SetCountry(v string)`

SetCountry sets Country field to given value.

### HasCountry

`func (o *ViewAvailableNumbersDataAllOfDataInner) HasCountry() bool`

HasCountry returns a boolean if a field has been set.

### GetCountryName

`func (o *ViewAvailableNumbersDataAllOfDataInner) GetCountryName() string`

GetCountryName returns the CountryName field if non-nil, zero value otherwise.

### GetCountryNameOk

`func (o *ViewAvailableNumbersDataAllOfDataInner) GetCountryNameOk() (*string, bool)`

GetCountryNameOk returns a tuple with the CountryName field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCountryName

`func (o *ViewAvailableNumbersDataAllOfDataInner) SetCountryName(v string)`

SetCountryName sets CountryName field to given value.

### HasCountryName

`func (o *ViewAvailableNumbersDataAllOfDataInner) HasCountryName() bool`

HasCountryName returns a boolean if a field has been set.

### GetDedicatedNumber

`func (o *ViewAvailableNumbersDataAllOfDataInner) GetDedicatedNumber() string`

GetDedicatedNumber returns the DedicatedNumber field if non-nil, zero value otherwise.

### GetDedicatedNumberOk

`func (o *ViewAvailableNumbersDataAllOfDataInner) GetDedicatedNumberOk() (*string, bool)`

GetDedicatedNumberOk returns a tuple with the DedicatedNumber field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDedicatedNumber

`func (o *ViewAvailableNumbersDataAllOfDataInner) SetDedicatedNumber(v string)`

SetDedicatedNumber sets DedicatedNumber field to given value.

### HasDedicatedNumber

`func (o *ViewAvailableNumbersDataAllOfDataInner) HasDedicatedNumber() bool`

HasDedicatedNumber returns a boolean if a field has been set.

### GetPriceSetup

`func (o *ViewAvailableNumbersDataAllOfDataInner) GetPriceSetup() string`

GetPriceSetup returns the PriceSetup field if non-nil, zero value otherwise.

### GetPriceSetupOk

`func (o *ViewAvailableNumbersDataAllOfDataInner) GetPriceSetupOk() (*string, bool)`

GetPriceSetupOk returns a tuple with the PriceSetup field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetPriceSetup

`func (o *ViewAvailableNumbersDataAllOfDataInner) SetPriceSetup(v string)`

SetPriceSetup sets PriceSetup field to given value.

### HasPriceSetup

`func (o *ViewAvailableNumbersDataAllOfDataInner) HasPriceSetup() bool`

HasPriceSetup returns a boolean if a field has been set.

### GetPriceMonthly

`func (o *ViewAvailableNumbersDataAllOfDataInner) GetPriceMonthly() string`

GetPriceMonthly returns the PriceMonthly field if non-nil, zero value otherwise.

### GetPriceMonthlyOk

`func (o *ViewAvailableNumbersDataAllOfDataInner) GetPriceMonthlyOk() (*string, bool)`

GetPriceMonthlyOk returns a tuple with the PriceMonthly field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetPriceMonthly

`func (o *ViewAvailableNumbersDataAllOfDataInner) SetPriceMonthly(v string)`

SetPriceMonthly sets PriceMonthly field to given value.

### HasPriceMonthly

`func (o *ViewAvailableNumbersDataAllOfDataInner) HasPriceMonthly() bool`

HasPriceMonthly returns a boolean if a field has been set.

### GetPriceTotal

`func (o *ViewAvailableNumbersDataAllOfDataInner) GetPriceTotal() string`

GetPriceTotal returns the PriceTotal field if non-nil, zero value otherwise.

### GetPriceTotalOk

`func (o *ViewAvailableNumbersDataAllOfDataInner) GetPriceTotalOk() (*string, bool)`

GetPriceTotalOk returns a tuple with the PriceTotal field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetPriceTotal

`func (o *ViewAvailableNumbersDataAllOfDataInner) SetPriceTotal(v string)`

SetPriceTotal sets PriceTotal field to given value.

### HasPriceTotal

`func (o *ViewAvailableNumbersDataAllOfDataInner) HasPriceTotal() bool`

HasPriceTotal returns a boolean if a field has been set.

### GetAddressRequirement

`func (o *ViewAvailableNumbersDataAllOfDataInner) GetAddressRequirement() string`

GetAddressRequirement returns the AddressRequirement field if non-nil, zero value otherwise.

### GetAddressRequirementOk

`func (o *ViewAvailableNumbersDataAllOfDataInner) GetAddressRequirementOk() (*string, bool)`

GetAddressRequirementOk returns a tuple with the AddressRequirement field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAddressRequirement

`func (o *ViewAvailableNumbersDataAllOfDataInner) SetAddressRequirement(v string)`

SetAddressRequirement sets AddressRequirement field to given value.

### HasAddressRequirement

`func (o *ViewAvailableNumbersDataAllOfDataInner) HasAddressRequirement() bool`

HasAddressRequirement returns a boolean if a field has been set.

### SetAddressRequirementNil

`func (o *ViewAvailableNumbersDataAllOfDataInner) SetAddressRequirementNil(b bool)`

 SetAddressRequirementNil sets the value for AddressRequirement to be an explicit nil

### UnsetAddressRequirement
`func (o *ViewAvailableNumbersDataAllOfDataInner) UnsetAddressRequirement()`

UnsetAddressRequirement ensures that no value is present for AddressRequirement, not even an explicit nil

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


