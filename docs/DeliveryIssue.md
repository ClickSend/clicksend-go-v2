# DeliveryIssue

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**IssueId** | Pointer to **string** | The unique identifier of the delivery issue. | [optional] 
**UserId** | Pointer to **int32** | The unique identifier of the user. | [optional] 
**MessageId** | Pointer to **string** | The message id of the message. | [optional] 
**Type** | Pointer to **string** | The type of message, must be one of the following values SMS, MMS, VOICE, EMAIL_MARKETING, EMAIL_TRANSACTIONAL, FAX, POST. | [optional] 
**Description** | Pointer to **string** | The description of the message. | [optional] 
**ClientComments** | Pointer to **NullableString** | The user&#39;s comments. | [optional] 
**SupportComments** | Pointer to **NullableString** | The support&#39;s comments. | [optional] 
**Status** | Pointer to **NullableString** | The status of the delivery issue. | [optional] 
**DateAdded** | Pointer to **float32** | The date and time the delivery issue was created. | [optional] 
**Resolved** | Pointer to **float32** | Flag indicating if the delivery issue is resolved. | [optional] 
**EmailAddress** | Pointer to **string** | The user&#39;s email address. | [optional] 

## Methods

### NewDeliveryIssue

`func NewDeliveryIssue() *DeliveryIssue`

NewDeliveryIssue instantiates a new DeliveryIssue object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewDeliveryIssueWithDefaults

`func NewDeliveryIssueWithDefaults() *DeliveryIssue`

NewDeliveryIssueWithDefaults instantiates a new DeliveryIssue object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetIssueId

`func (o *DeliveryIssue) GetIssueId() string`

GetIssueId returns the IssueId field if non-nil, zero value otherwise.

### GetIssueIdOk

`func (o *DeliveryIssue) GetIssueIdOk() (*string, bool)`

GetIssueIdOk returns a tuple with the IssueId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetIssueId

`func (o *DeliveryIssue) SetIssueId(v string)`

SetIssueId sets IssueId field to given value.

### HasIssueId

`func (o *DeliveryIssue) HasIssueId() bool`

HasIssueId returns a boolean if a field has been set.

### GetUserId

`func (o *DeliveryIssue) GetUserId() int32`

GetUserId returns the UserId field if non-nil, zero value otherwise.

### GetUserIdOk

`func (o *DeliveryIssue) GetUserIdOk() (*int32, bool)`

GetUserIdOk returns a tuple with the UserId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetUserId

`func (o *DeliveryIssue) SetUserId(v int32)`

SetUserId sets UserId field to given value.

### HasUserId

`func (o *DeliveryIssue) HasUserId() bool`

HasUserId returns a boolean if a field has been set.

### GetMessageId

`func (o *DeliveryIssue) GetMessageId() string`

GetMessageId returns the MessageId field if non-nil, zero value otherwise.

### GetMessageIdOk

`func (o *DeliveryIssue) GetMessageIdOk() (*string, bool)`

GetMessageIdOk returns a tuple with the MessageId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetMessageId

`func (o *DeliveryIssue) SetMessageId(v string)`

SetMessageId sets MessageId field to given value.

### HasMessageId

`func (o *DeliveryIssue) HasMessageId() bool`

HasMessageId returns a boolean if a field has been set.

### GetType

`func (o *DeliveryIssue) GetType() string`

GetType returns the Type field if non-nil, zero value otherwise.

### GetTypeOk

`func (o *DeliveryIssue) GetTypeOk() (*string, bool)`

GetTypeOk returns a tuple with the Type field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetType

`func (o *DeliveryIssue) SetType(v string)`

SetType sets Type field to given value.

### HasType

`func (o *DeliveryIssue) HasType() bool`

HasType returns a boolean if a field has been set.

### GetDescription

`func (o *DeliveryIssue) GetDescription() string`

GetDescription returns the Description field if non-nil, zero value otherwise.

### GetDescriptionOk

`func (o *DeliveryIssue) GetDescriptionOk() (*string, bool)`

GetDescriptionOk returns a tuple with the Description field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDescription

`func (o *DeliveryIssue) SetDescription(v string)`

SetDescription sets Description field to given value.

### HasDescription

`func (o *DeliveryIssue) HasDescription() bool`

HasDescription returns a boolean if a field has been set.

### GetClientComments

`func (o *DeliveryIssue) GetClientComments() string`

GetClientComments returns the ClientComments field if non-nil, zero value otherwise.

### GetClientCommentsOk

`func (o *DeliveryIssue) GetClientCommentsOk() (*string, bool)`

GetClientCommentsOk returns a tuple with the ClientComments field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetClientComments

`func (o *DeliveryIssue) SetClientComments(v string)`

SetClientComments sets ClientComments field to given value.

### HasClientComments

`func (o *DeliveryIssue) HasClientComments() bool`

HasClientComments returns a boolean if a field has been set.

### SetClientCommentsNil

`func (o *DeliveryIssue) SetClientCommentsNil(b bool)`

 SetClientCommentsNil sets the value for ClientComments to be an explicit nil

### UnsetClientComments
`func (o *DeliveryIssue) UnsetClientComments()`

UnsetClientComments ensures that no value is present for ClientComments, not even an explicit nil
### GetSupportComments

`func (o *DeliveryIssue) GetSupportComments() string`

GetSupportComments returns the SupportComments field if non-nil, zero value otherwise.

### GetSupportCommentsOk

`func (o *DeliveryIssue) GetSupportCommentsOk() (*string, bool)`

GetSupportCommentsOk returns a tuple with the SupportComments field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSupportComments

`func (o *DeliveryIssue) SetSupportComments(v string)`

SetSupportComments sets SupportComments field to given value.

### HasSupportComments

`func (o *DeliveryIssue) HasSupportComments() bool`

HasSupportComments returns a boolean if a field has been set.

### SetSupportCommentsNil

`func (o *DeliveryIssue) SetSupportCommentsNil(b bool)`

 SetSupportCommentsNil sets the value for SupportComments to be an explicit nil

### UnsetSupportComments
`func (o *DeliveryIssue) UnsetSupportComments()`

UnsetSupportComments ensures that no value is present for SupportComments, not even an explicit nil
### GetStatus

`func (o *DeliveryIssue) GetStatus() string`

GetStatus returns the Status field if non-nil, zero value otherwise.

### GetStatusOk

`func (o *DeliveryIssue) GetStatusOk() (*string, bool)`

GetStatusOk returns a tuple with the Status field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetStatus

`func (o *DeliveryIssue) SetStatus(v string)`

SetStatus sets Status field to given value.

### HasStatus

`func (o *DeliveryIssue) HasStatus() bool`

HasStatus returns a boolean if a field has been set.

### SetStatusNil

`func (o *DeliveryIssue) SetStatusNil(b bool)`

 SetStatusNil sets the value for Status to be an explicit nil

### UnsetStatus
`func (o *DeliveryIssue) UnsetStatus()`

UnsetStatus ensures that no value is present for Status, not even an explicit nil
### GetDateAdded

`func (o *DeliveryIssue) GetDateAdded() float32`

GetDateAdded returns the DateAdded field if non-nil, zero value otherwise.

### GetDateAddedOk

`func (o *DeliveryIssue) GetDateAddedOk() (*float32, bool)`

GetDateAddedOk returns a tuple with the DateAdded field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDateAdded

`func (o *DeliveryIssue) SetDateAdded(v float32)`

SetDateAdded sets DateAdded field to given value.

### HasDateAdded

`func (o *DeliveryIssue) HasDateAdded() bool`

HasDateAdded returns a boolean if a field has been set.

### GetResolved

`func (o *DeliveryIssue) GetResolved() float32`

GetResolved returns the Resolved field if non-nil, zero value otherwise.

### GetResolvedOk

`func (o *DeliveryIssue) GetResolvedOk() (*float32, bool)`

GetResolvedOk returns a tuple with the Resolved field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetResolved

`func (o *DeliveryIssue) SetResolved(v float32)`

SetResolved sets Resolved field to given value.

### HasResolved

`func (o *DeliveryIssue) HasResolved() bool`

HasResolved returns a boolean if a field has been set.

### GetEmailAddress

`func (o *DeliveryIssue) GetEmailAddress() string`

GetEmailAddress returns the EmailAddress field if non-nil, zero value otherwise.

### GetEmailAddressOk

`func (o *DeliveryIssue) GetEmailAddressOk() (*string, bool)`

GetEmailAddressOk returns a tuple with the EmailAddress field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetEmailAddress

`func (o *DeliveryIssue) SetEmailAddress(v string)`

SetEmailAddress sets EmailAddress field to given value.

### HasEmailAddress

`func (o *DeliveryIssue) HasEmailAddress() bool`

HasEmailAddress returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


