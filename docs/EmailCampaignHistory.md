# EmailCampaignHistory

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**EmailCampaignId** | Pointer to **int32** | The ID of the email campaign. | [optional] 
**FromName** | Pointer to **string** | The name of the sender. | [optional] 
**FromAddress** | Pointer to **string** | The email address of the sender. | [optional] 
**ToName** | Pointer to **string** | The name of the recipient. | [optional] 
**ToAddress** | Pointer to **string** | The email address of the recipient. | [optional] 
**ContactId** | Pointer to **int32** | The ID of the contact associated with the email. | [optional] 
**Subject** | Pointer to **string** | The subject of the email. | [optional] 
**MessageId** | Pointer to **string** | The unique ID of the email message. | [optional] 
**ProcessedAt** | Pointer to **NullableString** | The date and time when the email was processed. | [optional] 
**Status** | Pointer to **string** | The status of the email (e.g., SpamReport, Sent). | [optional] 
**OpenCount** | Pointer to **int32** | The count of times the email was opened. | [optional] 
**ClickCount** | Pointer to **int32** | The count of times links in the email were clicked. | [optional] 
**HardBounceCount** | Pointer to **int32** | The count of hard bounces for the email. | [optional] 
**SoftBounceCount** | Pointer to **int32** | The count of soft bounces for the email. | [optional] 

## Methods

### NewEmailCampaignHistory

`func NewEmailCampaignHistory() *EmailCampaignHistory`

NewEmailCampaignHistory instantiates a new EmailCampaignHistory object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewEmailCampaignHistoryWithDefaults

`func NewEmailCampaignHistoryWithDefaults() *EmailCampaignHistory`

NewEmailCampaignHistoryWithDefaults instantiates a new EmailCampaignHistory object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetEmailCampaignId

`func (o *EmailCampaignHistory) GetEmailCampaignId() int32`

GetEmailCampaignId returns the EmailCampaignId field if non-nil, zero value otherwise.

### GetEmailCampaignIdOk

`func (o *EmailCampaignHistory) GetEmailCampaignIdOk() (*int32, bool)`

GetEmailCampaignIdOk returns a tuple with the EmailCampaignId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetEmailCampaignId

`func (o *EmailCampaignHistory) SetEmailCampaignId(v int32)`

SetEmailCampaignId sets EmailCampaignId field to given value.

### HasEmailCampaignId

`func (o *EmailCampaignHistory) HasEmailCampaignId() bool`

HasEmailCampaignId returns a boolean if a field has been set.

### GetFromName

`func (o *EmailCampaignHistory) GetFromName() string`

GetFromName returns the FromName field if non-nil, zero value otherwise.

### GetFromNameOk

`func (o *EmailCampaignHistory) GetFromNameOk() (*string, bool)`

GetFromNameOk returns a tuple with the FromName field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetFromName

`func (o *EmailCampaignHistory) SetFromName(v string)`

SetFromName sets FromName field to given value.

### HasFromName

`func (o *EmailCampaignHistory) HasFromName() bool`

HasFromName returns a boolean if a field has been set.

### GetFromAddress

`func (o *EmailCampaignHistory) GetFromAddress() string`

GetFromAddress returns the FromAddress field if non-nil, zero value otherwise.

### GetFromAddressOk

`func (o *EmailCampaignHistory) GetFromAddressOk() (*string, bool)`

GetFromAddressOk returns a tuple with the FromAddress field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetFromAddress

`func (o *EmailCampaignHistory) SetFromAddress(v string)`

SetFromAddress sets FromAddress field to given value.

### HasFromAddress

`func (o *EmailCampaignHistory) HasFromAddress() bool`

HasFromAddress returns a boolean if a field has been set.

### GetToName

`func (o *EmailCampaignHistory) GetToName() string`

GetToName returns the ToName field if non-nil, zero value otherwise.

### GetToNameOk

`func (o *EmailCampaignHistory) GetToNameOk() (*string, bool)`

GetToNameOk returns a tuple with the ToName field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetToName

`func (o *EmailCampaignHistory) SetToName(v string)`

SetToName sets ToName field to given value.

### HasToName

`func (o *EmailCampaignHistory) HasToName() bool`

HasToName returns a boolean if a field has been set.

### GetToAddress

`func (o *EmailCampaignHistory) GetToAddress() string`

GetToAddress returns the ToAddress field if non-nil, zero value otherwise.

### GetToAddressOk

`func (o *EmailCampaignHistory) GetToAddressOk() (*string, bool)`

GetToAddressOk returns a tuple with the ToAddress field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetToAddress

`func (o *EmailCampaignHistory) SetToAddress(v string)`

SetToAddress sets ToAddress field to given value.

### HasToAddress

`func (o *EmailCampaignHistory) HasToAddress() bool`

HasToAddress returns a boolean if a field has been set.

### GetContactId

`func (o *EmailCampaignHistory) GetContactId() int32`

GetContactId returns the ContactId field if non-nil, zero value otherwise.

### GetContactIdOk

`func (o *EmailCampaignHistory) GetContactIdOk() (*int32, bool)`

GetContactIdOk returns a tuple with the ContactId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetContactId

`func (o *EmailCampaignHistory) SetContactId(v int32)`

SetContactId sets ContactId field to given value.

### HasContactId

`func (o *EmailCampaignHistory) HasContactId() bool`

HasContactId returns a boolean if a field has been set.

### GetSubject

`func (o *EmailCampaignHistory) GetSubject() string`

GetSubject returns the Subject field if non-nil, zero value otherwise.

### GetSubjectOk

`func (o *EmailCampaignHistory) GetSubjectOk() (*string, bool)`

GetSubjectOk returns a tuple with the Subject field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSubject

`func (o *EmailCampaignHistory) SetSubject(v string)`

SetSubject sets Subject field to given value.

### HasSubject

`func (o *EmailCampaignHistory) HasSubject() bool`

HasSubject returns a boolean if a field has been set.

### GetMessageId

`func (o *EmailCampaignHistory) GetMessageId() string`

GetMessageId returns the MessageId field if non-nil, zero value otherwise.

### GetMessageIdOk

`func (o *EmailCampaignHistory) GetMessageIdOk() (*string, bool)`

GetMessageIdOk returns a tuple with the MessageId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetMessageId

`func (o *EmailCampaignHistory) SetMessageId(v string)`

SetMessageId sets MessageId field to given value.

### HasMessageId

`func (o *EmailCampaignHistory) HasMessageId() bool`

HasMessageId returns a boolean if a field has been set.

### GetProcessedAt

`func (o *EmailCampaignHistory) GetProcessedAt() string`

GetProcessedAt returns the ProcessedAt field if non-nil, zero value otherwise.

### GetProcessedAtOk

`func (o *EmailCampaignHistory) GetProcessedAtOk() (*string, bool)`

GetProcessedAtOk returns a tuple with the ProcessedAt field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetProcessedAt

`func (o *EmailCampaignHistory) SetProcessedAt(v string)`

SetProcessedAt sets ProcessedAt field to given value.

### HasProcessedAt

`func (o *EmailCampaignHistory) HasProcessedAt() bool`

HasProcessedAt returns a boolean if a field has been set.

### SetProcessedAtNil

`func (o *EmailCampaignHistory) SetProcessedAtNil(b bool)`

 SetProcessedAtNil sets the value for ProcessedAt to be an explicit nil

### UnsetProcessedAt
`func (o *EmailCampaignHistory) UnsetProcessedAt()`

UnsetProcessedAt ensures that no value is present for ProcessedAt, not even an explicit nil
### GetStatus

`func (o *EmailCampaignHistory) GetStatus() string`

GetStatus returns the Status field if non-nil, zero value otherwise.

### GetStatusOk

`func (o *EmailCampaignHistory) GetStatusOk() (*string, bool)`

GetStatusOk returns a tuple with the Status field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetStatus

`func (o *EmailCampaignHistory) SetStatus(v string)`

SetStatus sets Status field to given value.

### HasStatus

`func (o *EmailCampaignHistory) HasStatus() bool`

HasStatus returns a boolean if a field has been set.

### GetOpenCount

`func (o *EmailCampaignHistory) GetOpenCount() int32`

GetOpenCount returns the OpenCount field if non-nil, zero value otherwise.

### GetOpenCountOk

`func (o *EmailCampaignHistory) GetOpenCountOk() (*int32, bool)`

GetOpenCountOk returns a tuple with the OpenCount field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetOpenCount

`func (o *EmailCampaignHistory) SetOpenCount(v int32)`

SetOpenCount sets OpenCount field to given value.

### HasOpenCount

`func (o *EmailCampaignHistory) HasOpenCount() bool`

HasOpenCount returns a boolean if a field has been set.

### GetClickCount

`func (o *EmailCampaignHistory) GetClickCount() int32`

GetClickCount returns the ClickCount field if non-nil, zero value otherwise.

### GetClickCountOk

`func (o *EmailCampaignHistory) GetClickCountOk() (*int32, bool)`

GetClickCountOk returns a tuple with the ClickCount field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetClickCount

`func (o *EmailCampaignHistory) SetClickCount(v int32)`

SetClickCount sets ClickCount field to given value.

### HasClickCount

`func (o *EmailCampaignHistory) HasClickCount() bool`

HasClickCount returns a boolean if a field has been set.

### GetHardBounceCount

`func (o *EmailCampaignHistory) GetHardBounceCount() int32`

GetHardBounceCount returns the HardBounceCount field if non-nil, zero value otherwise.

### GetHardBounceCountOk

`func (o *EmailCampaignHistory) GetHardBounceCountOk() (*int32, bool)`

GetHardBounceCountOk returns a tuple with the HardBounceCount field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetHardBounceCount

`func (o *EmailCampaignHistory) SetHardBounceCount(v int32)`

SetHardBounceCount sets HardBounceCount field to given value.

### HasHardBounceCount

`func (o *EmailCampaignHistory) HasHardBounceCount() bool`

HasHardBounceCount returns a boolean if a field has been set.

### GetSoftBounceCount

`func (o *EmailCampaignHistory) GetSoftBounceCount() int32`

GetSoftBounceCount returns the SoftBounceCount field if non-nil, zero value otherwise.

### GetSoftBounceCountOk

`func (o *EmailCampaignHistory) GetSoftBounceCountOk() (*int32, bool)`

GetSoftBounceCountOk returns a tuple with the SoftBounceCount field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSoftBounceCount

`func (o *EmailCampaignHistory) SetSoftBounceCount(v int32)`

SetSoftBounceCount sets SoftBounceCount field to given value.

### HasSoftBounceCount

`func (o *EmailCampaignHistory) HasSoftBounceCount() bool`

HasSoftBounceCount returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


