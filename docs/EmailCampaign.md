# EmailCampaign

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**EmailCampaignId** | Pointer to **int32** | The ID of the email campaign. | [optional] 
**Name** | Pointer to **string** | The name of the email campaign. | [optional] 
**UserId** | Pointer to **int32** | The ID of the user who created the email campaign. | [optional] 
**SubaccountId** | Pointer to **int32** | The ID of the subaccount associated with the email campaign. | [optional] 
**Subject** | Pointer to **string** | The subject of the email campaign. | [optional] 
**ListId** | Pointer to **int32** | The ID of the email list associated with the campaign. | [optional] 
**FromEmailAddressId** | Pointer to **int32** | The ID of the sender&#39;s email address. | [optional] 
**FromName** | Pointer to **string** | The name of the sender. | [optional] 
**TemplateId** | Pointer to **int32** | The ID of the email template used in the campaign. | [optional] 
**Schedule** | Pointer to **string** | The schedule for sending the email campaign. | [optional] 
**Status** | Pointer to **string** | The status of the email campaign (e.g., Sent, Scheduled, Draft). | [optional] 
**DateAdded** | Pointer to **string** | The date when the email campaign was added. | [optional] 
**CustomString** | Pointer to **string** | A custom string associated with the email campaign. | [optional] 
**SendCount** | Pointer to **int32** | The count of emails sent in the campaign. | [optional] 
**OpenCount** | Pointer to **int32** | The count of emails opened in the campaign. | [optional] 
**ClickCount** | Pointer to **int32** | The count of links clicked in the campaign. | [optional] 
**HardBounceCount** | Pointer to **int32** | The count of hard bounces in the campaign. | [optional] 
**SoftBounceCount** | Pointer to **int32** | The count of soft bounces in the campaign. | [optional] 
**AbuseCount** | Pointer to **int32** | The count of abuse complaints in the campaign. | [optional] 
**UnsubscribeCount** | Pointer to **int32** | The count of unsubscribes in the campaign. | [optional] 
**Body** | Pointer to **string** | The body of the email campaign. | [optional] 
**BodyPlainText** | Pointer to **string** | The plain text body of the email campaign. | [optional] 

## Methods

### NewEmailCampaign

`func NewEmailCampaign() *EmailCampaign`

NewEmailCampaign instantiates a new EmailCampaign object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewEmailCampaignWithDefaults

`func NewEmailCampaignWithDefaults() *EmailCampaign`

NewEmailCampaignWithDefaults instantiates a new EmailCampaign object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetEmailCampaignId

`func (o *EmailCampaign) GetEmailCampaignId() int32`

GetEmailCampaignId returns the EmailCampaignId field if non-nil, zero value otherwise.

### GetEmailCampaignIdOk

`func (o *EmailCampaign) GetEmailCampaignIdOk() (*int32, bool)`

GetEmailCampaignIdOk returns a tuple with the EmailCampaignId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetEmailCampaignId

`func (o *EmailCampaign) SetEmailCampaignId(v int32)`

SetEmailCampaignId sets EmailCampaignId field to given value.

### HasEmailCampaignId

`func (o *EmailCampaign) HasEmailCampaignId() bool`

HasEmailCampaignId returns a boolean if a field has been set.

### GetName

`func (o *EmailCampaign) GetName() string`

GetName returns the Name field if non-nil, zero value otherwise.

### GetNameOk

`func (o *EmailCampaign) GetNameOk() (*string, bool)`

GetNameOk returns a tuple with the Name field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetName

`func (o *EmailCampaign) SetName(v string)`

SetName sets Name field to given value.

### HasName

`func (o *EmailCampaign) HasName() bool`

HasName returns a boolean if a field has been set.

### GetUserId

`func (o *EmailCampaign) GetUserId() int32`

GetUserId returns the UserId field if non-nil, zero value otherwise.

### GetUserIdOk

`func (o *EmailCampaign) GetUserIdOk() (*int32, bool)`

GetUserIdOk returns a tuple with the UserId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetUserId

`func (o *EmailCampaign) SetUserId(v int32)`

SetUserId sets UserId field to given value.

### HasUserId

`func (o *EmailCampaign) HasUserId() bool`

HasUserId returns a boolean if a field has been set.

### GetSubaccountId

`func (o *EmailCampaign) GetSubaccountId() int32`

GetSubaccountId returns the SubaccountId field if non-nil, zero value otherwise.

### GetSubaccountIdOk

`func (o *EmailCampaign) GetSubaccountIdOk() (*int32, bool)`

GetSubaccountIdOk returns a tuple with the SubaccountId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSubaccountId

`func (o *EmailCampaign) SetSubaccountId(v int32)`

SetSubaccountId sets SubaccountId field to given value.

### HasSubaccountId

`func (o *EmailCampaign) HasSubaccountId() bool`

HasSubaccountId returns a boolean if a field has been set.

### GetSubject

`func (o *EmailCampaign) GetSubject() string`

GetSubject returns the Subject field if non-nil, zero value otherwise.

### GetSubjectOk

`func (o *EmailCampaign) GetSubjectOk() (*string, bool)`

GetSubjectOk returns a tuple with the Subject field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSubject

`func (o *EmailCampaign) SetSubject(v string)`

SetSubject sets Subject field to given value.

### HasSubject

`func (o *EmailCampaign) HasSubject() bool`

HasSubject returns a boolean if a field has been set.

### GetListId

`func (o *EmailCampaign) GetListId() int32`

GetListId returns the ListId field if non-nil, zero value otherwise.

### GetListIdOk

`func (o *EmailCampaign) GetListIdOk() (*int32, bool)`

GetListIdOk returns a tuple with the ListId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetListId

`func (o *EmailCampaign) SetListId(v int32)`

SetListId sets ListId field to given value.

### HasListId

`func (o *EmailCampaign) HasListId() bool`

HasListId returns a boolean if a field has been set.

### GetFromEmailAddressId

`func (o *EmailCampaign) GetFromEmailAddressId() int32`

GetFromEmailAddressId returns the FromEmailAddressId field if non-nil, zero value otherwise.

### GetFromEmailAddressIdOk

`func (o *EmailCampaign) GetFromEmailAddressIdOk() (*int32, bool)`

GetFromEmailAddressIdOk returns a tuple with the FromEmailAddressId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetFromEmailAddressId

`func (o *EmailCampaign) SetFromEmailAddressId(v int32)`

SetFromEmailAddressId sets FromEmailAddressId field to given value.

### HasFromEmailAddressId

`func (o *EmailCampaign) HasFromEmailAddressId() bool`

HasFromEmailAddressId returns a boolean if a field has been set.

### GetFromName

`func (o *EmailCampaign) GetFromName() string`

GetFromName returns the FromName field if non-nil, zero value otherwise.

### GetFromNameOk

`func (o *EmailCampaign) GetFromNameOk() (*string, bool)`

GetFromNameOk returns a tuple with the FromName field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetFromName

`func (o *EmailCampaign) SetFromName(v string)`

SetFromName sets FromName field to given value.

### HasFromName

`func (o *EmailCampaign) HasFromName() bool`

HasFromName returns a boolean if a field has been set.

### GetTemplateId

`func (o *EmailCampaign) GetTemplateId() int32`

GetTemplateId returns the TemplateId field if non-nil, zero value otherwise.

### GetTemplateIdOk

`func (o *EmailCampaign) GetTemplateIdOk() (*int32, bool)`

GetTemplateIdOk returns a tuple with the TemplateId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTemplateId

`func (o *EmailCampaign) SetTemplateId(v int32)`

SetTemplateId sets TemplateId field to given value.

### HasTemplateId

`func (o *EmailCampaign) HasTemplateId() bool`

HasTemplateId returns a boolean if a field has been set.

### GetSchedule

`func (o *EmailCampaign) GetSchedule() string`

GetSchedule returns the Schedule field if non-nil, zero value otherwise.

### GetScheduleOk

`func (o *EmailCampaign) GetScheduleOk() (*string, bool)`

GetScheduleOk returns a tuple with the Schedule field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSchedule

`func (o *EmailCampaign) SetSchedule(v string)`

SetSchedule sets Schedule field to given value.

### HasSchedule

`func (o *EmailCampaign) HasSchedule() bool`

HasSchedule returns a boolean if a field has been set.

### GetStatus

`func (o *EmailCampaign) GetStatus() string`

GetStatus returns the Status field if non-nil, zero value otherwise.

### GetStatusOk

`func (o *EmailCampaign) GetStatusOk() (*string, bool)`

GetStatusOk returns a tuple with the Status field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetStatus

`func (o *EmailCampaign) SetStatus(v string)`

SetStatus sets Status field to given value.

### HasStatus

`func (o *EmailCampaign) HasStatus() bool`

HasStatus returns a boolean if a field has been set.

### GetDateAdded

`func (o *EmailCampaign) GetDateAdded() string`

GetDateAdded returns the DateAdded field if non-nil, zero value otherwise.

### GetDateAddedOk

`func (o *EmailCampaign) GetDateAddedOk() (*string, bool)`

GetDateAddedOk returns a tuple with the DateAdded field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDateAdded

`func (o *EmailCampaign) SetDateAdded(v string)`

SetDateAdded sets DateAdded field to given value.

### HasDateAdded

`func (o *EmailCampaign) HasDateAdded() bool`

HasDateAdded returns a boolean if a field has been set.

### GetCustomString

`func (o *EmailCampaign) GetCustomString() string`

GetCustomString returns the CustomString field if non-nil, zero value otherwise.

### GetCustomStringOk

`func (o *EmailCampaign) GetCustomStringOk() (*string, bool)`

GetCustomStringOk returns a tuple with the CustomString field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCustomString

`func (o *EmailCampaign) SetCustomString(v string)`

SetCustomString sets CustomString field to given value.

### HasCustomString

`func (o *EmailCampaign) HasCustomString() bool`

HasCustomString returns a boolean if a field has been set.

### GetSendCount

`func (o *EmailCampaign) GetSendCount() int32`

GetSendCount returns the SendCount field if non-nil, zero value otherwise.

### GetSendCountOk

`func (o *EmailCampaign) GetSendCountOk() (*int32, bool)`

GetSendCountOk returns a tuple with the SendCount field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSendCount

`func (o *EmailCampaign) SetSendCount(v int32)`

SetSendCount sets SendCount field to given value.

### HasSendCount

`func (o *EmailCampaign) HasSendCount() bool`

HasSendCount returns a boolean if a field has been set.

### GetOpenCount

`func (o *EmailCampaign) GetOpenCount() int32`

GetOpenCount returns the OpenCount field if non-nil, zero value otherwise.

### GetOpenCountOk

`func (o *EmailCampaign) GetOpenCountOk() (*int32, bool)`

GetOpenCountOk returns a tuple with the OpenCount field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetOpenCount

`func (o *EmailCampaign) SetOpenCount(v int32)`

SetOpenCount sets OpenCount field to given value.

### HasOpenCount

`func (o *EmailCampaign) HasOpenCount() bool`

HasOpenCount returns a boolean if a field has been set.

### GetClickCount

`func (o *EmailCampaign) GetClickCount() int32`

GetClickCount returns the ClickCount field if non-nil, zero value otherwise.

### GetClickCountOk

`func (o *EmailCampaign) GetClickCountOk() (*int32, bool)`

GetClickCountOk returns a tuple with the ClickCount field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetClickCount

`func (o *EmailCampaign) SetClickCount(v int32)`

SetClickCount sets ClickCount field to given value.

### HasClickCount

`func (o *EmailCampaign) HasClickCount() bool`

HasClickCount returns a boolean if a field has been set.

### GetHardBounceCount

`func (o *EmailCampaign) GetHardBounceCount() int32`

GetHardBounceCount returns the HardBounceCount field if non-nil, zero value otherwise.

### GetHardBounceCountOk

`func (o *EmailCampaign) GetHardBounceCountOk() (*int32, bool)`

GetHardBounceCountOk returns a tuple with the HardBounceCount field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetHardBounceCount

`func (o *EmailCampaign) SetHardBounceCount(v int32)`

SetHardBounceCount sets HardBounceCount field to given value.

### HasHardBounceCount

`func (o *EmailCampaign) HasHardBounceCount() bool`

HasHardBounceCount returns a boolean if a field has been set.

### GetSoftBounceCount

`func (o *EmailCampaign) GetSoftBounceCount() int32`

GetSoftBounceCount returns the SoftBounceCount field if non-nil, zero value otherwise.

### GetSoftBounceCountOk

`func (o *EmailCampaign) GetSoftBounceCountOk() (*int32, bool)`

GetSoftBounceCountOk returns a tuple with the SoftBounceCount field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSoftBounceCount

`func (o *EmailCampaign) SetSoftBounceCount(v int32)`

SetSoftBounceCount sets SoftBounceCount field to given value.

### HasSoftBounceCount

`func (o *EmailCampaign) HasSoftBounceCount() bool`

HasSoftBounceCount returns a boolean if a field has been set.

### GetAbuseCount

`func (o *EmailCampaign) GetAbuseCount() int32`

GetAbuseCount returns the AbuseCount field if non-nil, zero value otherwise.

### GetAbuseCountOk

`func (o *EmailCampaign) GetAbuseCountOk() (*int32, bool)`

GetAbuseCountOk returns a tuple with the AbuseCount field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAbuseCount

`func (o *EmailCampaign) SetAbuseCount(v int32)`

SetAbuseCount sets AbuseCount field to given value.

### HasAbuseCount

`func (o *EmailCampaign) HasAbuseCount() bool`

HasAbuseCount returns a boolean if a field has been set.

### GetUnsubscribeCount

`func (o *EmailCampaign) GetUnsubscribeCount() int32`

GetUnsubscribeCount returns the UnsubscribeCount field if non-nil, zero value otherwise.

### GetUnsubscribeCountOk

`func (o *EmailCampaign) GetUnsubscribeCountOk() (*int32, bool)`

GetUnsubscribeCountOk returns a tuple with the UnsubscribeCount field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetUnsubscribeCount

`func (o *EmailCampaign) SetUnsubscribeCount(v int32)`

SetUnsubscribeCount sets UnsubscribeCount field to given value.

### HasUnsubscribeCount

`func (o *EmailCampaign) HasUnsubscribeCount() bool`

HasUnsubscribeCount returns a boolean if a field has been set.

### GetBody

`func (o *EmailCampaign) GetBody() string`

GetBody returns the Body field if non-nil, zero value otherwise.

### GetBodyOk

`func (o *EmailCampaign) GetBodyOk() (*string, bool)`

GetBodyOk returns a tuple with the Body field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetBody

`func (o *EmailCampaign) SetBody(v string)`

SetBody sets Body field to given value.

### HasBody

`func (o *EmailCampaign) HasBody() bool`

HasBody returns a boolean if a field has been set.

### GetBodyPlainText

`func (o *EmailCampaign) GetBodyPlainText() string`

GetBodyPlainText returns the BodyPlainText field if non-nil, zero value otherwise.

### GetBodyPlainTextOk

`func (o *EmailCampaign) GetBodyPlainTextOk() (*string, bool)`

GetBodyPlainTextOk returns a tuple with the BodyPlainText field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetBodyPlainText

`func (o *EmailCampaign) SetBodyPlainText(v string)`

SetBodyPlainText sets BodyPlainText field to given value.

### HasBodyPlainText

`func (o *EmailCampaign) HasBodyPlainText() bool`

HasBodyPlainText returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


