# CreateDeliveryIssueData

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**IssueId** | Pointer to **int32** | The ID of the created delivery issue. | [optional] 
**UserId** | Pointer to **int32** | The ID of the user who created the delivery issue. | [optional] 
**MessageId** | Pointer to **string** | The ID of the message associated with the delivery issue. | [optional] 
**Type** | Pointer to **string** | The type of delivery issue. | [optional] 
**Description** | Pointer to **string** | The description of the delivery issue. | [optional] 
**DateAdded** | Pointer to **int32** | The timestamp of when the delivery issue was created. | [optional] 
**EmailAddress** | Pointer to **string** | The email address associated with the delivery issue. | [optional] 

## Methods

### NewCreateDeliveryIssueData

`func NewCreateDeliveryIssueData() *CreateDeliveryIssueData`

NewCreateDeliveryIssueData instantiates a new CreateDeliveryIssueData object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewCreateDeliveryIssueDataWithDefaults

`func NewCreateDeliveryIssueDataWithDefaults() *CreateDeliveryIssueData`

NewCreateDeliveryIssueDataWithDefaults instantiates a new CreateDeliveryIssueData object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetIssueId

`func (o *CreateDeliveryIssueData) GetIssueId() int32`

GetIssueId returns the IssueId field if non-nil, zero value otherwise.

### GetIssueIdOk

`func (o *CreateDeliveryIssueData) GetIssueIdOk() (*int32, bool)`

GetIssueIdOk returns a tuple with the IssueId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetIssueId

`func (o *CreateDeliveryIssueData) SetIssueId(v int32)`

SetIssueId sets IssueId field to given value.

### HasIssueId

`func (o *CreateDeliveryIssueData) HasIssueId() bool`

HasIssueId returns a boolean if a field has been set.

### GetUserId

`func (o *CreateDeliveryIssueData) GetUserId() int32`

GetUserId returns the UserId field if non-nil, zero value otherwise.

### GetUserIdOk

`func (o *CreateDeliveryIssueData) GetUserIdOk() (*int32, bool)`

GetUserIdOk returns a tuple with the UserId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetUserId

`func (o *CreateDeliveryIssueData) SetUserId(v int32)`

SetUserId sets UserId field to given value.

### HasUserId

`func (o *CreateDeliveryIssueData) HasUserId() bool`

HasUserId returns a boolean if a field has been set.

### GetMessageId

`func (o *CreateDeliveryIssueData) GetMessageId() string`

GetMessageId returns the MessageId field if non-nil, zero value otherwise.

### GetMessageIdOk

`func (o *CreateDeliveryIssueData) GetMessageIdOk() (*string, bool)`

GetMessageIdOk returns a tuple with the MessageId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetMessageId

`func (o *CreateDeliveryIssueData) SetMessageId(v string)`

SetMessageId sets MessageId field to given value.

### HasMessageId

`func (o *CreateDeliveryIssueData) HasMessageId() bool`

HasMessageId returns a boolean if a field has been set.

### GetType

`func (o *CreateDeliveryIssueData) GetType() string`

GetType returns the Type field if non-nil, zero value otherwise.

### GetTypeOk

`func (o *CreateDeliveryIssueData) GetTypeOk() (*string, bool)`

GetTypeOk returns a tuple with the Type field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetType

`func (o *CreateDeliveryIssueData) SetType(v string)`

SetType sets Type field to given value.

### HasType

`func (o *CreateDeliveryIssueData) HasType() bool`

HasType returns a boolean if a field has been set.

### GetDescription

`func (o *CreateDeliveryIssueData) GetDescription() string`

GetDescription returns the Description field if non-nil, zero value otherwise.

### GetDescriptionOk

`func (o *CreateDeliveryIssueData) GetDescriptionOk() (*string, bool)`

GetDescriptionOk returns a tuple with the Description field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDescription

`func (o *CreateDeliveryIssueData) SetDescription(v string)`

SetDescription sets Description field to given value.

### HasDescription

`func (o *CreateDeliveryIssueData) HasDescription() bool`

HasDescription returns a boolean if a field has been set.

### GetDateAdded

`func (o *CreateDeliveryIssueData) GetDateAdded() int32`

GetDateAdded returns the DateAdded field if non-nil, zero value otherwise.

### GetDateAddedOk

`func (o *CreateDeliveryIssueData) GetDateAddedOk() (*int32, bool)`

GetDateAddedOk returns a tuple with the DateAdded field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDateAdded

`func (o *CreateDeliveryIssueData) SetDateAdded(v int32)`

SetDateAdded sets DateAdded field to given value.

### HasDateAdded

`func (o *CreateDeliveryIssueData) HasDateAdded() bool`

HasDateAdded returns a boolean if a field has been set.

### GetEmailAddress

`func (o *CreateDeliveryIssueData) GetEmailAddress() string`

GetEmailAddress returns the EmailAddress field if non-nil, zero value otherwise.

### GetEmailAddressOk

`func (o *CreateDeliveryIssueData) GetEmailAddressOk() (*string, bool)`

GetEmailAddressOk returns a tuple with the EmailAddress field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetEmailAddress

`func (o *CreateDeliveryIssueData) SetEmailAddress(v string)`

SetEmailAddress sets EmailAddress field to given value.

### HasEmailAddress

`func (o *CreateDeliveryIssueData) HasEmailAddress() bool`

HasEmailAddress returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


