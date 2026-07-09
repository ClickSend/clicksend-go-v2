# PostcardRecipientReturnAddress

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**ReturnAddressId** | Pointer to **int32** | The ID of the return address. | [optional] 
**UserId** | Pointer to **int32** | The ID of the user associated with the return address. | [optional] 
**AddressName** | Pointer to **string** | The name associated with the return address. | [optional] 
**AddressLine1** | Pointer to **string** | The first line of the return address. | [optional] 
**AddressLine2** | Pointer to **string** | The second line of the return address. | [optional] 
**AddressCity** | Pointer to **string** | The city of the return address. | [optional] 
**AddressState** | Pointer to **string** | The state of the return address. | [optional] 
**AddressPostalCode** | Pointer to **string** | The postal code of the return address. | [optional] 
**AddressCountry** | Pointer to **string** | The country code of the return address. | [optional] 

## Methods

### NewPostcardRecipientReturnAddress

`func NewPostcardRecipientReturnAddress() *PostcardRecipientReturnAddress`

NewPostcardRecipientReturnAddress instantiates a new PostcardRecipientReturnAddress object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewPostcardRecipientReturnAddressWithDefaults

`func NewPostcardRecipientReturnAddressWithDefaults() *PostcardRecipientReturnAddress`

NewPostcardRecipientReturnAddressWithDefaults instantiates a new PostcardRecipientReturnAddress object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetReturnAddressId

`func (o *PostcardRecipientReturnAddress) GetReturnAddressId() int32`

GetReturnAddressId returns the ReturnAddressId field if non-nil, zero value otherwise.

### GetReturnAddressIdOk

`func (o *PostcardRecipientReturnAddress) GetReturnAddressIdOk() (*int32, bool)`

GetReturnAddressIdOk returns a tuple with the ReturnAddressId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetReturnAddressId

`func (o *PostcardRecipientReturnAddress) SetReturnAddressId(v int32)`

SetReturnAddressId sets ReturnAddressId field to given value.

### HasReturnAddressId

`func (o *PostcardRecipientReturnAddress) HasReturnAddressId() bool`

HasReturnAddressId returns a boolean if a field has been set.

### GetUserId

`func (o *PostcardRecipientReturnAddress) GetUserId() int32`

GetUserId returns the UserId field if non-nil, zero value otherwise.

### GetUserIdOk

`func (o *PostcardRecipientReturnAddress) GetUserIdOk() (*int32, bool)`

GetUserIdOk returns a tuple with the UserId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetUserId

`func (o *PostcardRecipientReturnAddress) SetUserId(v int32)`

SetUserId sets UserId field to given value.

### HasUserId

`func (o *PostcardRecipientReturnAddress) HasUserId() bool`

HasUserId returns a boolean if a field has been set.

### GetAddressName

`func (o *PostcardRecipientReturnAddress) GetAddressName() string`

GetAddressName returns the AddressName field if non-nil, zero value otherwise.

### GetAddressNameOk

`func (o *PostcardRecipientReturnAddress) GetAddressNameOk() (*string, bool)`

GetAddressNameOk returns a tuple with the AddressName field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAddressName

`func (o *PostcardRecipientReturnAddress) SetAddressName(v string)`

SetAddressName sets AddressName field to given value.

### HasAddressName

`func (o *PostcardRecipientReturnAddress) HasAddressName() bool`

HasAddressName returns a boolean if a field has been set.

### GetAddressLine1

`func (o *PostcardRecipientReturnAddress) GetAddressLine1() string`

GetAddressLine1 returns the AddressLine1 field if non-nil, zero value otherwise.

### GetAddressLine1Ok

`func (o *PostcardRecipientReturnAddress) GetAddressLine1Ok() (*string, bool)`

GetAddressLine1Ok returns a tuple with the AddressLine1 field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAddressLine1

`func (o *PostcardRecipientReturnAddress) SetAddressLine1(v string)`

SetAddressLine1 sets AddressLine1 field to given value.

### HasAddressLine1

`func (o *PostcardRecipientReturnAddress) HasAddressLine1() bool`

HasAddressLine1 returns a boolean if a field has been set.

### GetAddressLine2

`func (o *PostcardRecipientReturnAddress) GetAddressLine2() string`

GetAddressLine2 returns the AddressLine2 field if non-nil, zero value otherwise.

### GetAddressLine2Ok

`func (o *PostcardRecipientReturnAddress) GetAddressLine2Ok() (*string, bool)`

GetAddressLine2Ok returns a tuple with the AddressLine2 field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAddressLine2

`func (o *PostcardRecipientReturnAddress) SetAddressLine2(v string)`

SetAddressLine2 sets AddressLine2 field to given value.

### HasAddressLine2

`func (o *PostcardRecipientReturnAddress) HasAddressLine2() bool`

HasAddressLine2 returns a boolean if a field has been set.

### GetAddressCity

`func (o *PostcardRecipientReturnAddress) GetAddressCity() string`

GetAddressCity returns the AddressCity field if non-nil, zero value otherwise.

### GetAddressCityOk

`func (o *PostcardRecipientReturnAddress) GetAddressCityOk() (*string, bool)`

GetAddressCityOk returns a tuple with the AddressCity field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAddressCity

`func (o *PostcardRecipientReturnAddress) SetAddressCity(v string)`

SetAddressCity sets AddressCity field to given value.

### HasAddressCity

`func (o *PostcardRecipientReturnAddress) HasAddressCity() bool`

HasAddressCity returns a boolean if a field has been set.

### GetAddressState

`func (o *PostcardRecipientReturnAddress) GetAddressState() string`

GetAddressState returns the AddressState field if non-nil, zero value otherwise.

### GetAddressStateOk

`func (o *PostcardRecipientReturnAddress) GetAddressStateOk() (*string, bool)`

GetAddressStateOk returns a tuple with the AddressState field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAddressState

`func (o *PostcardRecipientReturnAddress) SetAddressState(v string)`

SetAddressState sets AddressState field to given value.

### HasAddressState

`func (o *PostcardRecipientReturnAddress) HasAddressState() bool`

HasAddressState returns a boolean if a field has been set.

### GetAddressPostalCode

`func (o *PostcardRecipientReturnAddress) GetAddressPostalCode() string`

GetAddressPostalCode returns the AddressPostalCode field if non-nil, zero value otherwise.

### GetAddressPostalCodeOk

`func (o *PostcardRecipientReturnAddress) GetAddressPostalCodeOk() (*string, bool)`

GetAddressPostalCodeOk returns a tuple with the AddressPostalCode field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAddressPostalCode

`func (o *PostcardRecipientReturnAddress) SetAddressPostalCode(v string)`

SetAddressPostalCode sets AddressPostalCode field to given value.

### HasAddressPostalCode

`func (o *PostcardRecipientReturnAddress) HasAddressPostalCode() bool`

HasAddressPostalCode returns a boolean if a field has been set.

### GetAddressCountry

`func (o *PostcardRecipientReturnAddress) GetAddressCountry() string`

GetAddressCountry returns the AddressCountry field if non-nil, zero value otherwise.

### GetAddressCountryOk

`func (o *PostcardRecipientReturnAddress) GetAddressCountryOk() (*string, bool)`

GetAddressCountryOk returns a tuple with the AddressCountry field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAddressCountry

`func (o *PostcardRecipientReturnAddress) SetAddressCountry(v string)`

SetAddressCountry sets AddressCountry field to given value.

### HasAddressCountry

`func (o *PostcardRecipientReturnAddress) HasAddressCountry() bool`

HasAddressCountry returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


