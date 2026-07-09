# SendEmailRequest

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**To** | Pointer to [**[]SendEmailRequestToInner**](SendEmailRequestToInner.md) |  | [optional] 
**From** | Pointer to [**SendEmailRequestFrom**](SendEmailRequestFrom.md) |  | [optional] 
**Subject** | Pointer to **string** |  | [optional] 
**Body** | Pointer to **string** |  | [optional] 
**Attachments** | Pointer to [**[]SendEmailRequestAttachmentsInner**](SendEmailRequestAttachmentsInner.md) |  | [optional] 

## Methods

### NewSendEmailRequest

`func NewSendEmailRequest() *SendEmailRequest`

NewSendEmailRequest instantiates a new SendEmailRequest object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewSendEmailRequestWithDefaults

`func NewSendEmailRequestWithDefaults() *SendEmailRequest`

NewSendEmailRequestWithDefaults instantiates a new SendEmailRequest object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetTo

`func (o *SendEmailRequest) GetTo() []SendEmailRequestToInner`

GetTo returns the To field if non-nil, zero value otherwise.

### GetToOk

`func (o *SendEmailRequest) GetToOk() (*[]SendEmailRequestToInner, bool)`

GetToOk returns a tuple with the To field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTo

`func (o *SendEmailRequest) SetTo(v []SendEmailRequestToInner)`

SetTo sets To field to given value.

### HasTo

`func (o *SendEmailRequest) HasTo() bool`

HasTo returns a boolean if a field has been set.

### GetFrom

`func (o *SendEmailRequest) GetFrom() SendEmailRequestFrom`

GetFrom returns the From field if non-nil, zero value otherwise.

### GetFromOk

`func (o *SendEmailRequest) GetFromOk() (*SendEmailRequestFrom, bool)`

GetFromOk returns a tuple with the From field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetFrom

`func (o *SendEmailRequest) SetFrom(v SendEmailRequestFrom)`

SetFrom sets From field to given value.

### HasFrom

`func (o *SendEmailRequest) HasFrom() bool`

HasFrom returns a boolean if a field has been set.

### GetSubject

`func (o *SendEmailRequest) GetSubject() string`

GetSubject returns the Subject field if non-nil, zero value otherwise.

### GetSubjectOk

`func (o *SendEmailRequest) GetSubjectOk() (*string, bool)`

GetSubjectOk returns a tuple with the Subject field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSubject

`func (o *SendEmailRequest) SetSubject(v string)`

SetSubject sets Subject field to given value.

### HasSubject

`func (o *SendEmailRequest) HasSubject() bool`

HasSubject returns a boolean if a field has been set.

### GetBody

`func (o *SendEmailRequest) GetBody() string`

GetBody returns the Body field if non-nil, zero value otherwise.

### GetBodyOk

`func (o *SendEmailRequest) GetBodyOk() (*string, bool)`

GetBodyOk returns a tuple with the Body field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetBody

`func (o *SendEmailRequest) SetBody(v string)`

SetBody sets Body field to given value.

### HasBody

`func (o *SendEmailRequest) HasBody() bool`

HasBody returns a boolean if a field has been set.

### GetAttachments

`func (o *SendEmailRequest) GetAttachments() []SendEmailRequestAttachmentsInner`

GetAttachments returns the Attachments field if non-nil, zero value otherwise.

### GetAttachmentsOk

`func (o *SendEmailRequest) GetAttachmentsOk() (*[]SendEmailRequestAttachmentsInner, bool)`

GetAttachmentsOk returns a tuple with the Attachments field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAttachments

`func (o *SendEmailRequest) SetAttachments(v []SendEmailRequestAttachmentsInner)`

SetAttachments sets Attachments field to given value.

### HasAttachments

`func (o *SendEmailRequest) HasAttachments() bool`

HasAttachments returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


