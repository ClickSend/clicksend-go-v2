# ViewRechargePackagesData

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Packages** | Pointer to [**[]ViewRechargePackagesDataPackagesInner**](ViewRechargePackagesDataPackagesInner.md) |  | [optional] 
**Currency** | Pointer to [**Currency**](Currency.md) |  | [optional] 

## Methods

### NewViewRechargePackagesData

`func NewViewRechargePackagesData() *ViewRechargePackagesData`

NewViewRechargePackagesData instantiates a new ViewRechargePackagesData object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewViewRechargePackagesDataWithDefaults

`func NewViewRechargePackagesDataWithDefaults() *ViewRechargePackagesData`

NewViewRechargePackagesDataWithDefaults instantiates a new ViewRechargePackagesData object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetPackages

`func (o *ViewRechargePackagesData) GetPackages() []ViewRechargePackagesDataPackagesInner`

GetPackages returns the Packages field if non-nil, zero value otherwise.

### GetPackagesOk

`func (o *ViewRechargePackagesData) GetPackagesOk() (*[]ViewRechargePackagesDataPackagesInner, bool)`

GetPackagesOk returns a tuple with the Packages field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetPackages

`func (o *ViewRechargePackagesData) SetPackages(v []ViewRechargePackagesDataPackagesInner)`

SetPackages sets Packages field to given value.

### HasPackages

`func (o *ViewRechargePackagesData) HasPackages() bool`

HasPackages returns a boolean if a field has been set.

### GetCurrency

`func (o *ViewRechargePackagesData) GetCurrency() Currency`

GetCurrency returns the Currency field if non-nil, zero value otherwise.

### GetCurrencyOk

`func (o *ViewRechargePackagesData) GetCurrencyOk() (*Currency, bool)`

GetCurrencyOk returns a tuple with the Currency field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCurrency

`func (o *ViewRechargePackagesData) SetCurrency(v Currency)`

SetCurrency sets Currency field to given value.

### HasCurrency

`func (o *ViewRechargePackagesData) HasCurrency() bool`

HasCurrency returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


