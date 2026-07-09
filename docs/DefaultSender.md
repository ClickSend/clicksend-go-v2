# DefaultSender

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Id** | **string** | ID of the default sender. | 
**UserId** | **int32** | User ID from the version 3 system. | 
**SubaccountId** | **int32** | Subaccount ID from version 3. | 
**CountryCode** | **string** | ISO 3166-1 alpha-2 formatted country code. | 
**ProductType** | **string** | Type of product for which the setting is applied. | 
**DefaultSenderStrategies** | [**[]DefaultSenderDefaultSenderStrategiesInner**](DefaultSenderDefaultSenderStrategiesInner.md) | Default sender strategies. Must contain 1 or more objects. | 
**Status** | **string** | Overall status of the default sender. | 
**CreatedTimestamp** | **string** | Timestamp of when the default sender was created. Must be in ISO 8601 format. | 
**UpdatedTimestamp** | **string** | Timestamp of the last update to the default sender. Must be in ISO 8601 format. | 

## Methods

### NewDefaultSender

`func NewDefaultSender(id string, userId int32, subaccountId int32, countryCode string, productType string, defaultSenderStrategies []DefaultSenderDefaultSenderStrategiesInner, status string, createdTimestamp string, updatedTimestamp string, ) *DefaultSender`

NewDefaultSender instantiates a new DefaultSender object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewDefaultSenderWithDefaults

`func NewDefaultSenderWithDefaults() *DefaultSender`

NewDefaultSenderWithDefaults instantiates a new DefaultSender object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetId

`func (o *DefaultSender) GetId() string`

GetId returns the Id field if non-nil, zero value otherwise.

### GetIdOk

`func (o *DefaultSender) GetIdOk() (*string, bool)`

GetIdOk returns a tuple with the Id field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetId

`func (o *DefaultSender) SetId(v string)`

SetId sets Id field to given value.


### GetUserId

`func (o *DefaultSender) GetUserId() int32`

GetUserId returns the UserId field if non-nil, zero value otherwise.

### GetUserIdOk

`func (o *DefaultSender) GetUserIdOk() (*int32, bool)`

GetUserIdOk returns a tuple with the UserId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetUserId

`func (o *DefaultSender) SetUserId(v int32)`

SetUserId sets UserId field to given value.


### GetSubaccountId

`func (o *DefaultSender) GetSubaccountId() int32`

GetSubaccountId returns the SubaccountId field if non-nil, zero value otherwise.

### GetSubaccountIdOk

`func (o *DefaultSender) GetSubaccountIdOk() (*int32, bool)`

GetSubaccountIdOk returns a tuple with the SubaccountId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSubaccountId

`func (o *DefaultSender) SetSubaccountId(v int32)`

SetSubaccountId sets SubaccountId field to given value.


### GetCountryCode

`func (o *DefaultSender) GetCountryCode() string`

GetCountryCode returns the CountryCode field if non-nil, zero value otherwise.

### GetCountryCodeOk

`func (o *DefaultSender) GetCountryCodeOk() (*string, bool)`

GetCountryCodeOk returns a tuple with the CountryCode field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCountryCode

`func (o *DefaultSender) SetCountryCode(v string)`

SetCountryCode sets CountryCode field to given value.


### GetProductType

`func (o *DefaultSender) GetProductType() string`

GetProductType returns the ProductType field if non-nil, zero value otherwise.

### GetProductTypeOk

`func (o *DefaultSender) GetProductTypeOk() (*string, bool)`

GetProductTypeOk returns a tuple with the ProductType field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetProductType

`func (o *DefaultSender) SetProductType(v string)`

SetProductType sets ProductType field to given value.


### GetDefaultSenderStrategies

`func (o *DefaultSender) GetDefaultSenderStrategies() []DefaultSenderDefaultSenderStrategiesInner`

GetDefaultSenderStrategies returns the DefaultSenderStrategies field if non-nil, zero value otherwise.

### GetDefaultSenderStrategiesOk

`func (o *DefaultSender) GetDefaultSenderStrategiesOk() (*[]DefaultSenderDefaultSenderStrategiesInner, bool)`

GetDefaultSenderStrategiesOk returns a tuple with the DefaultSenderStrategies field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDefaultSenderStrategies

`func (o *DefaultSender) SetDefaultSenderStrategies(v []DefaultSenderDefaultSenderStrategiesInner)`

SetDefaultSenderStrategies sets DefaultSenderStrategies field to given value.


### GetStatus

`func (o *DefaultSender) GetStatus() string`

GetStatus returns the Status field if non-nil, zero value otherwise.

### GetStatusOk

`func (o *DefaultSender) GetStatusOk() (*string, bool)`

GetStatusOk returns a tuple with the Status field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetStatus

`func (o *DefaultSender) SetStatus(v string)`

SetStatus sets Status field to given value.


### GetCreatedTimestamp

`func (o *DefaultSender) GetCreatedTimestamp() string`

GetCreatedTimestamp returns the CreatedTimestamp field if non-nil, zero value otherwise.

### GetCreatedTimestampOk

`func (o *DefaultSender) GetCreatedTimestampOk() (*string, bool)`

GetCreatedTimestampOk returns a tuple with the CreatedTimestamp field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCreatedTimestamp

`func (o *DefaultSender) SetCreatedTimestamp(v string)`

SetCreatedTimestamp sets CreatedTimestamp field to given value.


### GetUpdatedTimestamp

`func (o *DefaultSender) GetUpdatedTimestamp() string`

GetUpdatedTimestamp returns the UpdatedTimestamp field if non-nil, zero value otherwise.

### GetUpdatedTimestampOk

`func (o *DefaultSender) GetUpdatedTimestampOk() (*string, bool)`

GetUpdatedTimestampOk returns a tuple with the UpdatedTimestamp field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetUpdatedTimestamp

`func (o *DefaultSender) SetUpdatedTimestamp(v string)`

SetUpdatedTimestamp sets UpdatedTimestamp field to given value.



[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


