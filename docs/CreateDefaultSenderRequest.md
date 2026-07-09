# CreateDefaultSenderRequest

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**CountryCode** | **string** | The country code of the recipient. Must be a valid ISO 3166-1 alpha-2 country code. | 
**ProductType** | **string** | The type of product for the assignment. Support for additional types coming soon. | 
**DefaultSenderStrategies** | [**[]CreateDefaultSenderRequestDefaultSenderStrategiesInner**](CreateDefaultSenderRequestDefaultSenderStrategiesInner.md) | Array detailing sender strategies. Must contain exactly 1 element. Multiple strategies support coming soon. | 

## Methods

### NewCreateDefaultSenderRequest

`func NewCreateDefaultSenderRequest(countryCode string, productType string, defaultSenderStrategies []CreateDefaultSenderRequestDefaultSenderStrategiesInner, ) *CreateDefaultSenderRequest`

NewCreateDefaultSenderRequest instantiates a new CreateDefaultSenderRequest object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewCreateDefaultSenderRequestWithDefaults

`func NewCreateDefaultSenderRequestWithDefaults() *CreateDefaultSenderRequest`

NewCreateDefaultSenderRequestWithDefaults instantiates a new CreateDefaultSenderRequest object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetCountryCode

`func (o *CreateDefaultSenderRequest) GetCountryCode() string`

GetCountryCode returns the CountryCode field if non-nil, zero value otherwise.

### GetCountryCodeOk

`func (o *CreateDefaultSenderRequest) GetCountryCodeOk() (*string, bool)`

GetCountryCodeOk returns a tuple with the CountryCode field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCountryCode

`func (o *CreateDefaultSenderRequest) SetCountryCode(v string)`

SetCountryCode sets CountryCode field to given value.


### GetProductType

`func (o *CreateDefaultSenderRequest) GetProductType() string`

GetProductType returns the ProductType field if non-nil, zero value otherwise.

### GetProductTypeOk

`func (o *CreateDefaultSenderRequest) GetProductTypeOk() (*string, bool)`

GetProductTypeOk returns a tuple with the ProductType field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetProductType

`func (o *CreateDefaultSenderRequest) SetProductType(v string)`

SetProductType sets ProductType field to given value.


### GetDefaultSenderStrategies

`func (o *CreateDefaultSenderRequest) GetDefaultSenderStrategies() []CreateDefaultSenderRequestDefaultSenderStrategiesInner`

GetDefaultSenderStrategies returns the DefaultSenderStrategies field if non-nil, zero value otherwise.

### GetDefaultSenderStrategiesOk

`func (o *CreateDefaultSenderRequest) GetDefaultSenderStrategiesOk() (*[]CreateDefaultSenderRequestDefaultSenderStrategiesInner, bool)`

GetDefaultSenderStrategiesOk returns a tuple with the DefaultSenderStrategies field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDefaultSenderStrategies

`func (o *CreateDefaultSenderRequest) SetDefaultSenderStrategies(v []CreateDefaultSenderRequestDefaultSenderStrategiesInner)`

SetDefaultSenderStrategies sets DefaultSenderStrategies field to given value.



[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


