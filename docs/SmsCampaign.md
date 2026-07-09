# SmsCampaign

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**SmsCampaignId** | Pointer to **int32** | The ID of the SMS campaign. | [optional] 
**Name** | Pointer to **string** | The name of the SMS campaign. | [optional] 
**UserId** | Pointer to **int32** | The unique user ID of the sender. | [optional] 
**SubaccountId** | Pointer to **int32** | The sub-account of the user. A user can have multiple sub-accounts. | [optional] 
**ListId** | Pointer to **int32** | The _list_id_ of the contact list to which the SMS campaign was sent or will be sent to. | [optional] 
**From** | Pointer to **string** | The sender of the message. This is also referred to as the **Sender ID**. If your **Sender ID** has a different country code to the recipient’s, it&#39;ll be replaced by a local number, except in &lt;a href&#x3D;\&quot;https://help.clicksend.com/category/mfdctha7f0-country-specific-features-and-restrictions\&quot; target&#x3D;\&quot;_blank\&quot;&gt;certain countries&lt;/a&gt;. If the sender number is blocked, a different number will replace it. | [optional] 
**Body** | Pointer to **string** | The message body of the SMS campaign sent. | [optional] 
**Schedule** | Pointer to **string** | The scheduled date of the message. It is in &lt;a href&#x3D;\&quot;http://help.clicksend.com/what-is-a-unix-timestamp\&quot; target&#x3D;\&quot;_blank\&quot;&gt;Unix format&lt;/a&gt;. | [optional] 
**Status** | Pointer to **string** | The status of the SMS. Available statuses are:    - _Approved_: The SMS campaign has been approved and is ready to be sent.   - _Cancelled_: The SMS campaign was scheduled but has been cancelled before sending.   - _Draft_: The SMS campaign is saved as a draft and has not been sent.   - _Failed_: The SMS campaign failed to send due to an issue.   - _Queued_: The SMS campaign is waiting to be sent.   - _Scheduled_: The SMS campaign is set to be sent at a later time.   - _Sending_: The SMS campaign is currently being sent.   - _Sent_: The SMS campaign has been sent, but this does not guarantee that all messages were successfully delivered.   - _WaitApproval_: The SMS campaign is awaiting approval from ClickSend, which may take a few minutes. | [optional] 
**DateAdded** | Pointer to **string** | The date you created the SMS campaign. It is in &lt;a href&#x3D;\&quot;http://help.clicksend.com/what-is-a-unix-timestamp\&quot; target&#x3D;\&quot;_blank\&quot;&gt;Unix format&lt;/a&gt;. | [optional] 
**CustomString** | Pointer to **NullableString** | The custom note that was added when creating or updating the SMS campaign. | [optional] 
**UrlToShorten** | Pointer to **string** | The original URL that had been shorten. It will return an **empty** value if the SMS campaign didn’t include any shortened URL. | [optional] 
**UnsubscribeLink** | Pointer to **int32** | Indicates whether an unsubscribe link has been included in the message. To provide the option to unsubscribe, you can add the literal &#x60;StopMsg.me/xxxxx&#x60; in the message body. This parameter specifies whether the link was added:    - **0**: The unsubscribe option was not provided.   - **1**: The unsubscribe option was provided. | [optional] 
**Source** | Pointer to **NullableString** | The source of the request. For example, the name of your application. It&#39;s used to identify messages sent from various applications. It will return a **null** value if the source was not specified in the SMS campaign. | [optional] 
**Senders** | Pointer to [**[]SmsCampaignSendersInner**](SmsCampaignSendersInner.md) | The specific sender IDs for each recipient country. It will return a **null** value if you did not specify the sender in the SMS campaign. | [optional] 
**TotalCount** | Pointer to **int32** | The total number of messages sent in the SMS campaign. | [optional] 
**ListName** | Pointer to **string** | The name of the contact list of the SMS campaign. This is related of the _list_id_ parameter. | [optional] 

## Methods

### NewSmsCampaign

`func NewSmsCampaign() *SmsCampaign`

NewSmsCampaign instantiates a new SmsCampaign object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewSmsCampaignWithDefaults

`func NewSmsCampaignWithDefaults() *SmsCampaign`

NewSmsCampaignWithDefaults instantiates a new SmsCampaign object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetSmsCampaignId

`func (o *SmsCampaign) GetSmsCampaignId() int32`

GetSmsCampaignId returns the SmsCampaignId field if non-nil, zero value otherwise.

### GetSmsCampaignIdOk

`func (o *SmsCampaign) GetSmsCampaignIdOk() (*int32, bool)`

GetSmsCampaignIdOk returns a tuple with the SmsCampaignId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSmsCampaignId

`func (o *SmsCampaign) SetSmsCampaignId(v int32)`

SetSmsCampaignId sets SmsCampaignId field to given value.

### HasSmsCampaignId

`func (o *SmsCampaign) HasSmsCampaignId() bool`

HasSmsCampaignId returns a boolean if a field has been set.

### GetName

`func (o *SmsCampaign) GetName() string`

GetName returns the Name field if non-nil, zero value otherwise.

### GetNameOk

`func (o *SmsCampaign) GetNameOk() (*string, bool)`

GetNameOk returns a tuple with the Name field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetName

`func (o *SmsCampaign) SetName(v string)`

SetName sets Name field to given value.

### HasName

`func (o *SmsCampaign) HasName() bool`

HasName returns a boolean if a field has been set.

### GetUserId

`func (o *SmsCampaign) GetUserId() int32`

GetUserId returns the UserId field if non-nil, zero value otherwise.

### GetUserIdOk

`func (o *SmsCampaign) GetUserIdOk() (*int32, bool)`

GetUserIdOk returns a tuple with the UserId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetUserId

`func (o *SmsCampaign) SetUserId(v int32)`

SetUserId sets UserId field to given value.

### HasUserId

`func (o *SmsCampaign) HasUserId() bool`

HasUserId returns a boolean if a field has been set.

### GetSubaccountId

`func (o *SmsCampaign) GetSubaccountId() int32`

GetSubaccountId returns the SubaccountId field if non-nil, zero value otherwise.

### GetSubaccountIdOk

`func (o *SmsCampaign) GetSubaccountIdOk() (*int32, bool)`

GetSubaccountIdOk returns a tuple with the SubaccountId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSubaccountId

`func (o *SmsCampaign) SetSubaccountId(v int32)`

SetSubaccountId sets SubaccountId field to given value.

### HasSubaccountId

`func (o *SmsCampaign) HasSubaccountId() bool`

HasSubaccountId returns a boolean if a field has been set.

### GetListId

`func (o *SmsCampaign) GetListId() int32`

GetListId returns the ListId field if non-nil, zero value otherwise.

### GetListIdOk

`func (o *SmsCampaign) GetListIdOk() (*int32, bool)`

GetListIdOk returns a tuple with the ListId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetListId

`func (o *SmsCampaign) SetListId(v int32)`

SetListId sets ListId field to given value.

### HasListId

`func (o *SmsCampaign) HasListId() bool`

HasListId returns a boolean if a field has been set.

### GetFrom

`func (o *SmsCampaign) GetFrom() string`

GetFrom returns the From field if non-nil, zero value otherwise.

### GetFromOk

`func (o *SmsCampaign) GetFromOk() (*string, bool)`

GetFromOk returns a tuple with the From field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetFrom

`func (o *SmsCampaign) SetFrom(v string)`

SetFrom sets From field to given value.

### HasFrom

`func (o *SmsCampaign) HasFrom() bool`

HasFrom returns a boolean if a field has been set.

### GetBody

`func (o *SmsCampaign) GetBody() string`

GetBody returns the Body field if non-nil, zero value otherwise.

### GetBodyOk

`func (o *SmsCampaign) GetBodyOk() (*string, bool)`

GetBodyOk returns a tuple with the Body field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetBody

`func (o *SmsCampaign) SetBody(v string)`

SetBody sets Body field to given value.

### HasBody

`func (o *SmsCampaign) HasBody() bool`

HasBody returns a boolean if a field has been set.

### GetSchedule

`func (o *SmsCampaign) GetSchedule() string`

GetSchedule returns the Schedule field if non-nil, zero value otherwise.

### GetScheduleOk

`func (o *SmsCampaign) GetScheduleOk() (*string, bool)`

GetScheduleOk returns a tuple with the Schedule field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSchedule

`func (o *SmsCampaign) SetSchedule(v string)`

SetSchedule sets Schedule field to given value.

### HasSchedule

`func (o *SmsCampaign) HasSchedule() bool`

HasSchedule returns a boolean if a field has been set.

### GetStatus

`func (o *SmsCampaign) GetStatus() string`

GetStatus returns the Status field if non-nil, zero value otherwise.

### GetStatusOk

`func (o *SmsCampaign) GetStatusOk() (*string, bool)`

GetStatusOk returns a tuple with the Status field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetStatus

`func (o *SmsCampaign) SetStatus(v string)`

SetStatus sets Status field to given value.

### HasStatus

`func (o *SmsCampaign) HasStatus() bool`

HasStatus returns a boolean if a field has been set.

### GetDateAdded

`func (o *SmsCampaign) GetDateAdded() string`

GetDateAdded returns the DateAdded field if non-nil, zero value otherwise.

### GetDateAddedOk

`func (o *SmsCampaign) GetDateAddedOk() (*string, bool)`

GetDateAddedOk returns a tuple with the DateAdded field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDateAdded

`func (o *SmsCampaign) SetDateAdded(v string)`

SetDateAdded sets DateAdded field to given value.

### HasDateAdded

`func (o *SmsCampaign) HasDateAdded() bool`

HasDateAdded returns a boolean if a field has been set.

### GetCustomString

`func (o *SmsCampaign) GetCustomString() string`

GetCustomString returns the CustomString field if non-nil, zero value otherwise.

### GetCustomStringOk

`func (o *SmsCampaign) GetCustomStringOk() (*string, bool)`

GetCustomStringOk returns a tuple with the CustomString field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCustomString

`func (o *SmsCampaign) SetCustomString(v string)`

SetCustomString sets CustomString field to given value.

### HasCustomString

`func (o *SmsCampaign) HasCustomString() bool`

HasCustomString returns a boolean if a field has been set.

### SetCustomStringNil

`func (o *SmsCampaign) SetCustomStringNil(b bool)`

 SetCustomStringNil sets the value for CustomString to be an explicit nil

### UnsetCustomString
`func (o *SmsCampaign) UnsetCustomString()`

UnsetCustomString ensures that no value is present for CustomString, not even an explicit nil
### GetUrlToShorten

`func (o *SmsCampaign) GetUrlToShorten() string`

GetUrlToShorten returns the UrlToShorten field if non-nil, zero value otherwise.

### GetUrlToShortenOk

`func (o *SmsCampaign) GetUrlToShortenOk() (*string, bool)`

GetUrlToShortenOk returns a tuple with the UrlToShorten field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetUrlToShorten

`func (o *SmsCampaign) SetUrlToShorten(v string)`

SetUrlToShorten sets UrlToShorten field to given value.

### HasUrlToShorten

`func (o *SmsCampaign) HasUrlToShorten() bool`

HasUrlToShorten returns a boolean if a field has been set.

### GetUnsubscribeLink

`func (o *SmsCampaign) GetUnsubscribeLink() int32`

GetUnsubscribeLink returns the UnsubscribeLink field if non-nil, zero value otherwise.

### GetUnsubscribeLinkOk

`func (o *SmsCampaign) GetUnsubscribeLinkOk() (*int32, bool)`

GetUnsubscribeLinkOk returns a tuple with the UnsubscribeLink field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetUnsubscribeLink

`func (o *SmsCampaign) SetUnsubscribeLink(v int32)`

SetUnsubscribeLink sets UnsubscribeLink field to given value.

### HasUnsubscribeLink

`func (o *SmsCampaign) HasUnsubscribeLink() bool`

HasUnsubscribeLink returns a boolean if a field has been set.

### GetSource

`func (o *SmsCampaign) GetSource() string`

GetSource returns the Source field if non-nil, zero value otherwise.

### GetSourceOk

`func (o *SmsCampaign) GetSourceOk() (*string, bool)`

GetSourceOk returns a tuple with the Source field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSource

`func (o *SmsCampaign) SetSource(v string)`

SetSource sets Source field to given value.

### HasSource

`func (o *SmsCampaign) HasSource() bool`

HasSource returns a boolean if a field has been set.

### SetSourceNil

`func (o *SmsCampaign) SetSourceNil(b bool)`

 SetSourceNil sets the value for Source to be an explicit nil

### UnsetSource
`func (o *SmsCampaign) UnsetSource()`

UnsetSource ensures that no value is present for Source, not even an explicit nil
### GetSenders

`func (o *SmsCampaign) GetSenders() []SmsCampaignSendersInner`

GetSenders returns the Senders field if non-nil, zero value otherwise.

### GetSendersOk

`func (o *SmsCampaign) GetSendersOk() (*[]SmsCampaignSendersInner, bool)`

GetSendersOk returns a tuple with the Senders field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSenders

`func (o *SmsCampaign) SetSenders(v []SmsCampaignSendersInner)`

SetSenders sets Senders field to given value.

### HasSenders

`func (o *SmsCampaign) HasSenders() bool`

HasSenders returns a boolean if a field has been set.

### GetTotalCount

`func (o *SmsCampaign) GetTotalCount() int32`

GetTotalCount returns the TotalCount field if non-nil, zero value otherwise.

### GetTotalCountOk

`func (o *SmsCampaign) GetTotalCountOk() (*int32, bool)`

GetTotalCountOk returns a tuple with the TotalCount field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTotalCount

`func (o *SmsCampaign) SetTotalCount(v int32)`

SetTotalCount sets TotalCount field to given value.

### HasTotalCount

`func (o *SmsCampaign) HasTotalCount() bool`

HasTotalCount returns a boolean if a field has been set.

### GetListName

`func (o *SmsCampaign) GetListName() string`

GetListName returns the ListName field if non-nil, zero value otherwise.

### GetListNameOk

`func (o *SmsCampaign) GetListNameOk() (*string, bool)`

GetListNameOk returns a tuple with the ListName field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetListName

`func (o *SmsCampaign) SetListName(v string)`

SetListName sets ListName field to given value.

### HasListName

`func (o *SmsCampaign) HasListName() bool`

HasListName returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


