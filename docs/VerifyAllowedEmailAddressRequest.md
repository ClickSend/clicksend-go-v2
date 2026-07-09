# VerifyAllowedEmailAddressRequest

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**To** | Pointer to [**[]SendEmailRequestToInner**](SendEmailRequestToInner.md) |  | [optional] 
**From** | Pointer to [**SendEmailVerificationTokenRequestFrom**](SendEmailVerificationTokenRequestFrom.md) |  | [optional] 
**Subject** | Pointer to **string** |  | [optional] 
**Body** | Pointer to **string** |  | [optional] 

## Methods

### NewVerifyAllowedEmailAddressRequest

`func NewVerifyAllowedEmailAddressRequest() *VerifyAllowedEmailAddressRequest`

NewVerifyAllowedEmailAddressRequest instantiates a new VerifyAllowedEmailAddressRequest object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewVerifyAllowedEmailAddressRequestWithDefaults

`func NewVerifyAllowedEmailAddressRequestWithDefaults() *VerifyAllowedEmailAddressRequest`

NewVerifyAllowedEmailAddressRequestWithDefaults instantiates a new VerifyAllowedEmailAddressRequest object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetTo

`func (o *VerifyAllowedEmailAddressRequest) GetTo() []SendEmailRequestToInner`

GetTo returns the To field if non-nil, zero value otherwise.

### GetToOk

`func (o *VerifyAllowedEmailAddressRequest) GetToOk() (*[]SendEmailRequestToInner, bool)`

GetToOk returns a tuple with the To field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTo

`func (o *VerifyAllowedEmailAddressRequest) SetTo(v []SendEmailRequestToInner)`

SetTo sets To field to given value.

### HasTo

`func (o *VerifyAllowedEmailAddressRequest) HasTo() bool`

HasTo returns a boolean if a field has been set.

### GetFrom

`func (o *VerifyAllowedEmailAddressRequest) GetFrom() SendEmailVerificationTokenRequestFrom`

GetFrom returns the From field if non-nil, zero value otherwise.

### GetFromOk

`func (o *VerifyAllowedEmailAddressRequest) GetFromOk() (*SendEmailVerificationTokenRequestFrom, bool)`

GetFromOk returns a tuple with the From field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetFrom

`func (o *VerifyAllowedEmailAddressRequest) SetFrom(v SendEmailVerificationTokenRequestFrom)`

SetFrom sets From field to given value.

### HasFrom

`func (o *VerifyAllowedEmailAddressRequest) HasFrom() bool`

HasFrom returns a boolean if a field has been set.

### GetSubject

`func (o *VerifyAllowedEmailAddressRequest) GetSubject() string`

GetSubject returns the Subject field if non-nil, zero value otherwise.

### GetSubjectOk

`func (o *VerifyAllowedEmailAddressRequest) GetSubjectOk() (*string, bool)`

GetSubjectOk returns a tuple with the Subject field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSubject

`func (o *VerifyAllowedEmailAddressRequest) SetSubject(v string)`

SetSubject sets Subject field to given value.

### HasSubject

`func (o *VerifyAllowedEmailAddressRequest) HasSubject() bool`

HasSubject returns a boolean if a field has been set.

### GetBody

`func (o *VerifyAllowedEmailAddressRequest) GetBody() string`

GetBody returns the Body field if non-nil, zero value otherwise.

### GetBodyOk

`func (o *VerifyAllowedEmailAddressRequest) GetBodyOk() (*string, bool)`

GetBodyOk returns a tuple with the Body field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetBody

`func (o *VerifyAllowedEmailAddressRequest) SetBody(v string)`

SetBody sets Body field to given value.

### HasBody

`func (o *VerifyAllowedEmailAddressRequest) HasBody() bool`

HasBody returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


