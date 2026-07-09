# CreateDeliveryIssueRequest

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**MessageId** | Pointer to **string** |  | [optional] 
**Type** | Pointer to **string** |  | [optional] 
**Description** | Pointer to **string** |  | [optional] 
**EmailAddress** | Pointer to **string** |  | [optional] 
**ClientComments** | Pointer to **string** |  | [optional] 
**SupportComments** | Pointer to **string** |  | [optional] 
**Resolved** | Pointer to **bool** |  | [optional] 

## Methods

### NewCreateDeliveryIssueRequest

`func NewCreateDeliveryIssueRequest() *CreateDeliveryIssueRequest`

NewCreateDeliveryIssueRequest instantiates a new CreateDeliveryIssueRequest object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewCreateDeliveryIssueRequestWithDefaults

`func NewCreateDeliveryIssueRequestWithDefaults() *CreateDeliveryIssueRequest`

NewCreateDeliveryIssueRequestWithDefaults instantiates a new CreateDeliveryIssueRequest object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetMessageId

`func (o *CreateDeliveryIssueRequest) GetMessageId() string`

GetMessageId returns the MessageId field if non-nil, zero value otherwise.

### GetMessageIdOk

`func (o *CreateDeliveryIssueRequest) GetMessageIdOk() (*string, bool)`

GetMessageIdOk returns a tuple with the MessageId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetMessageId

`func (o *CreateDeliveryIssueRequest) SetMessageId(v string)`

SetMessageId sets MessageId field to given value.

### HasMessageId

`func (o *CreateDeliveryIssueRequest) HasMessageId() bool`

HasMessageId returns a boolean if a field has been set.

### GetType

`func (o *CreateDeliveryIssueRequest) GetType() string`

GetType returns the Type field if non-nil, zero value otherwise.

### GetTypeOk

`func (o *CreateDeliveryIssueRequest) GetTypeOk() (*string, bool)`

GetTypeOk returns a tuple with the Type field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetType

`func (o *CreateDeliveryIssueRequest) SetType(v string)`

SetType sets Type field to given value.

### HasType

`func (o *CreateDeliveryIssueRequest) HasType() bool`

HasType returns a boolean if a field has been set.

### GetDescription

`func (o *CreateDeliveryIssueRequest) GetDescription() string`

GetDescription returns the Description field if non-nil, zero value otherwise.

### GetDescriptionOk

`func (o *CreateDeliveryIssueRequest) GetDescriptionOk() (*string, bool)`

GetDescriptionOk returns a tuple with the Description field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDescription

`func (o *CreateDeliveryIssueRequest) SetDescription(v string)`

SetDescription sets Description field to given value.

### HasDescription

`func (o *CreateDeliveryIssueRequest) HasDescription() bool`

HasDescription returns a boolean if a field has been set.

### GetEmailAddress

`func (o *CreateDeliveryIssueRequest) GetEmailAddress() string`

GetEmailAddress returns the EmailAddress field if non-nil, zero value otherwise.

### GetEmailAddressOk

`func (o *CreateDeliveryIssueRequest) GetEmailAddressOk() (*string, bool)`

GetEmailAddressOk returns a tuple with the EmailAddress field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetEmailAddress

`func (o *CreateDeliveryIssueRequest) SetEmailAddress(v string)`

SetEmailAddress sets EmailAddress field to given value.

### HasEmailAddress

`func (o *CreateDeliveryIssueRequest) HasEmailAddress() bool`

HasEmailAddress returns a boolean if a field has been set.

### GetClientComments

`func (o *CreateDeliveryIssueRequest) GetClientComments() string`

GetClientComments returns the ClientComments field if non-nil, zero value otherwise.

### GetClientCommentsOk

`func (o *CreateDeliveryIssueRequest) GetClientCommentsOk() (*string, bool)`

GetClientCommentsOk returns a tuple with the ClientComments field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetClientComments

`func (o *CreateDeliveryIssueRequest) SetClientComments(v string)`

SetClientComments sets ClientComments field to given value.

### HasClientComments

`func (o *CreateDeliveryIssueRequest) HasClientComments() bool`

HasClientComments returns a boolean if a field has been set.

### GetSupportComments

`func (o *CreateDeliveryIssueRequest) GetSupportComments() string`

GetSupportComments returns the SupportComments field if non-nil, zero value otherwise.

### GetSupportCommentsOk

`func (o *CreateDeliveryIssueRequest) GetSupportCommentsOk() (*string, bool)`

GetSupportCommentsOk returns a tuple with the SupportComments field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSupportComments

`func (o *CreateDeliveryIssueRequest) SetSupportComments(v string)`

SetSupportComments sets SupportComments field to given value.

### HasSupportComments

`func (o *CreateDeliveryIssueRequest) HasSupportComments() bool`

HasSupportComments returns a boolean if a field has been set.

### GetResolved

`func (o *CreateDeliveryIssueRequest) GetResolved() bool`

GetResolved returns the Resolved field if non-nil, zero value otherwise.

### GetResolvedOk

`func (o *CreateDeliveryIssueRequest) GetResolvedOk() (*bool, bool)`

GetResolvedOk returns a tuple with the Resolved field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetResolved

`func (o *CreateDeliveryIssueRequest) SetResolved(v bool)`

SetResolved sets Resolved field to given value.

### HasResolved

`func (o *CreateDeliveryIssueRequest) HasResolved() bool`

HasResolved returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


