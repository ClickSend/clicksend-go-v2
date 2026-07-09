# EmailAddress

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**EmailAddressId** | Pointer to **int32** | The unique identifier for the email address. | [optional] 
**EmailAddress** | Pointer to **string** | The email address. | [optional] 
**Verified** | Pointer to **int32** | Flag indicating if the email address is verified. | [optional] 
**DateAdded** | Pointer to **string** | The date the email address was added. | [optional] 

## Methods

### NewEmailAddress

`func NewEmailAddress() *EmailAddress`

NewEmailAddress instantiates a new EmailAddress object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewEmailAddressWithDefaults

`func NewEmailAddressWithDefaults() *EmailAddress`

NewEmailAddressWithDefaults instantiates a new EmailAddress object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetEmailAddressId

`func (o *EmailAddress) GetEmailAddressId() int32`

GetEmailAddressId returns the EmailAddressId field if non-nil, zero value otherwise.

### GetEmailAddressIdOk

`func (o *EmailAddress) GetEmailAddressIdOk() (*int32, bool)`

GetEmailAddressIdOk returns a tuple with the EmailAddressId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetEmailAddressId

`func (o *EmailAddress) SetEmailAddressId(v int32)`

SetEmailAddressId sets EmailAddressId field to given value.

### HasEmailAddressId

`func (o *EmailAddress) HasEmailAddressId() bool`

HasEmailAddressId returns a boolean if a field has been set.

### GetEmailAddress

`func (o *EmailAddress) GetEmailAddress() string`

GetEmailAddress returns the EmailAddress field if non-nil, zero value otherwise.

### GetEmailAddressOk

`func (o *EmailAddress) GetEmailAddressOk() (*string, bool)`

GetEmailAddressOk returns a tuple with the EmailAddress field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetEmailAddress

`func (o *EmailAddress) SetEmailAddress(v string)`

SetEmailAddress sets EmailAddress field to given value.

### HasEmailAddress

`func (o *EmailAddress) HasEmailAddress() bool`

HasEmailAddress returns a boolean if a field has been set.

### GetVerified

`func (o *EmailAddress) GetVerified() int32`

GetVerified returns the Verified field if non-nil, zero value otherwise.

### GetVerifiedOk

`func (o *EmailAddress) GetVerifiedOk() (*int32, bool)`

GetVerifiedOk returns a tuple with the Verified field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetVerified

`func (o *EmailAddress) SetVerified(v int32)`

SetVerified sets Verified field to given value.

### HasVerified

`func (o *EmailAddress) HasVerified() bool`

HasVerified returns a boolean if a field has been set.

### GetDateAdded

`func (o *EmailAddress) GetDateAdded() string`

GetDateAdded returns the DateAdded field if non-nil, zero value otherwise.

### GetDateAddedOk

`func (o *EmailAddress) GetDateAddedOk() (*string, bool)`

GetDateAddedOk returns a tuple with the DateAdded field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDateAdded

`func (o *EmailAddress) SetDateAdded(v string)`

SetDateAdded sets DateAdded field to given value.

### HasDateAdded

`func (o *EmailAddress) HasDateAdded() bool`

HasDateAdded returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


