# SendEmailVerificationTokenRequest

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**To** | Pointer to [**[]SendEmailVerificationTokenRequestToInner**](SendEmailVerificationTokenRequestToInner.md) |  | [optional] 
**From** | Pointer to [**SendEmailVerificationTokenRequestFrom**](SendEmailVerificationTokenRequestFrom.md) |  | [optional] 
**Subject** | Pointer to **string** |  | [optional] 
**Body** | Pointer to **string** |  | [optional] 

## Methods

### NewSendEmailVerificationTokenRequest

`func NewSendEmailVerificationTokenRequest() *SendEmailVerificationTokenRequest`

NewSendEmailVerificationTokenRequest instantiates a new SendEmailVerificationTokenRequest object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewSendEmailVerificationTokenRequestWithDefaults

`func NewSendEmailVerificationTokenRequestWithDefaults() *SendEmailVerificationTokenRequest`

NewSendEmailVerificationTokenRequestWithDefaults instantiates a new SendEmailVerificationTokenRequest object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetTo

`func (o *SendEmailVerificationTokenRequest) GetTo() []SendEmailVerificationTokenRequestToInner`

GetTo returns the To field if non-nil, zero value otherwise.

### GetToOk

`func (o *SendEmailVerificationTokenRequest) GetToOk() (*[]SendEmailVerificationTokenRequestToInner, bool)`

GetToOk returns a tuple with the To field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTo

`func (o *SendEmailVerificationTokenRequest) SetTo(v []SendEmailVerificationTokenRequestToInner)`

SetTo sets To field to given value.

### HasTo

`func (o *SendEmailVerificationTokenRequest) HasTo() bool`

HasTo returns a boolean if a field has been set.

### GetFrom

`func (o *SendEmailVerificationTokenRequest) GetFrom() SendEmailVerificationTokenRequestFrom`

GetFrom returns the From field if non-nil, zero value otherwise.

### GetFromOk

`func (o *SendEmailVerificationTokenRequest) GetFromOk() (*SendEmailVerificationTokenRequestFrom, bool)`

GetFromOk returns a tuple with the From field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetFrom

`func (o *SendEmailVerificationTokenRequest) SetFrom(v SendEmailVerificationTokenRequestFrom)`

SetFrom sets From field to given value.

### HasFrom

`func (o *SendEmailVerificationTokenRequest) HasFrom() bool`

HasFrom returns a boolean if a field has been set.

### GetSubject

`func (o *SendEmailVerificationTokenRequest) GetSubject() string`

GetSubject returns the Subject field if non-nil, zero value otherwise.

### GetSubjectOk

`func (o *SendEmailVerificationTokenRequest) GetSubjectOk() (*string, bool)`

GetSubjectOk returns a tuple with the Subject field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSubject

`func (o *SendEmailVerificationTokenRequest) SetSubject(v string)`

SetSubject sets Subject field to given value.

### HasSubject

`func (o *SendEmailVerificationTokenRequest) HasSubject() bool`

HasSubject returns a boolean if a field has been set.

### GetBody

`func (o *SendEmailVerificationTokenRequest) GetBody() string`

GetBody returns the Body field if non-nil, zero value otherwise.

### GetBodyOk

`func (o *SendEmailVerificationTokenRequest) GetBodyOk() (*string, bool)`

GetBodyOk returns a tuple with the Body field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetBody

`func (o *SendEmailVerificationTokenRequest) SetBody(v string)`

SetBody sets Body field to given value.

### HasBody

`func (o *SendEmailVerificationTokenRequest) HasBody() bool`

HasBody returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


