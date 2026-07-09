# BuyNumberRequest

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**DedicatedNumber** | **string** | Phone number to purchase | 
**Type** | **string** | Service type for the number | 
**RegistrationData** | Pointer to [**BuyNumberRequestRegistrationData**](BuyNumberRequestRegistrationData.md) |  | [optional] 

## Methods

### NewBuyNumberRequest

`func NewBuyNumberRequest(dedicatedNumber string, type_ string, ) *BuyNumberRequest`

NewBuyNumberRequest instantiates a new BuyNumberRequest object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewBuyNumberRequestWithDefaults

`func NewBuyNumberRequestWithDefaults() *BuyNumberRequest`

NewBuyNumberRequestWithDefaults instantiates a new BuyNumberRequest object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetDedicatedNumber

`func (o *BuyNumberRequest) GetDedicatedNumber() string`

GetDedicatedNumber returns the DedicatedNumber field if non-nil, zero value otherwise.

### GetDedicatedNumberOk

`func (o *BuyNumberRequest) GetDedicatedNumberOk() (*string, bool)`

GetDedicatedNumberOk returns a tuple with the DedicatedNumber field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDedicatedNumber

`func (o *BuyNumberRequest) SetDedicatedNumber(v string)`

SetDedicatedNumber sets DedicatedNumber field to given value.


### GetType

`func (o *BuyNumberRequest) GetType() string`

GetType returns the Type field if non-nil, zero value otherwise.

### GetTypeOk

`func (o *BuyNumberRequest) GetTypeOk() (*string, bool)`

GetTypeOk returns a tuple with the Type field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetType

`func (o *BuyNumberRequest) SetType(v string)`

SetType sets Type field to given value.


### GetRegistrationData

`func (o *BuyNumberRequest) GetRegistrationData() BuyNumberRequestRegistrationData`

GetRegistrationData returns the RegistrationData field if non-nil, zero value otherwise.

### GetRegistrationDataOk

`func (o *BuyNumberRequest) GetRegistrationDataOk() (*BuyNumberRequestRegistrationData, bool)`

GetRegistrationDataOk returns a tuple with the RegistrationData field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetRegistrationData

`func (o *BuyNumberRequest) SetRegistrationData(v BuyNumberRequestRegistrationData)`

SetRegistrationData sets RegistrationData field to given value.

### HasRegistrationData

`func (o *BuyNumberRequest) HasRegistrationData() bool`

HasRegistrationData returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


