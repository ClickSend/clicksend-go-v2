# SmsSendSms

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Direction** | Pointer to **string** | It can either be **in** or **out**:  - **in** - You received a message. it has to do with inbound messages.      - **out** \\- You are sending a message. It has to do with outbound messages. | [optional] 
**Date** | Pointer to **int32** | The date you sent the message. It is in &lt;a href&#x3D;\&quot;http://help.clicksend.com/what-is-a-unix-timestamp\&quot; target&#x3D;\&quot;_blank\&quot;&gt;Unix format&lt;/a&gt;. | [optional] 
**To** | Pointer to **string** | The phone number of the recipient. It should be in &lt;a href&#x3D;\&quot;https://en.wikipedia.org/wiki/E.164\&quot; target&#x3D;\&quot;_blank\&quot;&gt;E.164 format&lt;/a&gt;. | [optional] 
**Body** | Pointer to **string** | The message sent. The price of sending a message depends on the number of characters and the type of message. There are two types:  - Standard message - Contains only characters in the &lt;a href&#x3D;\&quot;https://en.wikipedia.org/wiki/GSM_03.38\&quot; target&#x3D;\&quot;_blank\&quot;&gt;GSM&lt;/a&gt; set, with a maximum of 160 characters.      - Unicode message - Contains characters outside the &lt;a href&#x3D;\&quot;https://en.wikipedia.org/wiki/GSM_03.38\&quot; target&#x3D;\&quot;_blank\&quot;&gt;GSM&lt;/a&gt; set, with a maximum of 70 characters.       Longer messages will be sent as multiple messages (parts), but the recipient will receive them as a single long message. Visit &lt;a href&#x3D;\&quot;https://help.clicksend.com/article/h474eseq3a-how-many-characters-can-i-send-in-an-sms\&quot; target&#x3D;\&quot;_blank\&quot;&gt;this page&lt;/a&gt; to learn more about the number of characters per message, and &lt;a href&#x3D;\&quot;http://smscharactercount.com/\&quot; target&#x3D;\&quot;_blank\&quot;&gt;this page&lt;/a&gt; to count the number of characters. | [optional] 
**From** | Pointer to **string** | The sender of the message. This is also referred to as the **Sender ID**. If your **Sender ID** has a different country code to the recipient’s, it&#39;ll be replaced by a local number, except in &lt;a href&#x3D;\&quot;https://help.clicksend.com/category/mfdctha7f0-country-specific-features-and-restrictions\&quot; target&#x3D;\&quot;_blank\&quot;&gt;certain countries&lt;/a&gt;. If the sender number is blocked, a different number will replace it. | [optional] 
**Schedule** | Pointer to **int32** | The scheduled date of the message. It is in &lt;a href&#x3D;\&quot;http://help.clicksend.com/what-is-a-unix-timestamp\&quot; target&#x3D;\&quot;_blank\&quot;&gt;Unix format&lt;/a&gt;. | [optional] 
**MessageId** | Pointer to **string** | The generated ID of the message. This ID is typically used as a reference for &lt;a href&#x3D;\&quot;https://www.clicksend.com/au/help/\&quot; target&#x3D;\&quot;_blank\&quot;&gt;customer support&lt;/a&gt; in case of any issues. | [optional] 
**MessageParts** | Pointer to **int32** | The number of parts the message was broken into. To look at how many parts your message is broken down into, use the **&lt;a href&#x3D;\&quot;http://smscharactercount.com/\&quot;&gt;SMS Character Count&lt;/a&gt;**. | [optional] 
**MessagePrice** | Pointer to **float32** | The price of this message. This depends on the total number of parts of the message. | [optional] 
**FromEmail** | Pointer to **string** | The email address to which replies should be emailed to. If omitted, the reply will be emailed back to the user who sent the outgoing SMS. | [optional] 
**ListId** | Pointer to **string** | The _list_id_ of the contact list the message was sent to. This parameter will have a **null** value if you didn’t send to a list in the request. | [optional] 
**CustomString** | Pointer to **string** | A note that was sent from the request. | [optional] 
**ContactId** | Pointer to **string** | This is the ID of the contact. This parameter will have a **null** value if you didn’t provide a _contact_id_ in the request. | [optional] 
**UserId** | Pointer to **int32** | The unique user ID of the sender. | [optional] 
**SubaccountId** | Pointer to **int32** | This sub-account of the user. A user can have multiple sub-accounts. | [optional] 
**IsSharedSystemNumber** | Pointer to **bool** | Indicates whether you use a shared number to send a message:  - **True** \\- if the sender is randomly selected.      - **False** \\- if the sender is specified and passed the validation process. | [optional] 
**Country** | Pointer to **string** | The country of the recipient in two-letter format (e.g. US, UK, AU, NZ, etc). | [optional] 
**Carrier** | Pointer to **string** | The phone carrier of the recipient. | [optional] 
**Status** | Pointer to **string** | The response code of the operation. Visit [this page](/#application-status-codes) for more information. This reflects the actual status of the individual message. | [optional] 

## Methods

### NewSmsSendSms

`func NewSmsSendSms() *SmsSendSms`

NewSmsSendSms instantiates a new SmsSendSms object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewSmsSendSmsWithDefaults

`func NewSmsSendSmsWithDefaults() *SmsSendSms`

NewSmsSendSmsWithDefaults instantiates a new SmsSendSms object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetDirection

`func (o *SmsSendSms) GetDirection() string`

GetDirection returns the Direction field if non-nil, zero value otherwise.

### GetDirectionOk

`func (o *SmsSendSms) GetDirectionOk() (*string, bool)`

GetDirectionOk returns a tuple with the Direction field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDirection

`func (o *SmsSendSms) SetDirection(v string)`

SetDirection sets Direction field to given value.

### HasDirection

`func (o *SmsSendSms) HasDirection() bool`

HasDirection returns a boolean if a field has been set.

### GetDate

`func (o *SmsSendSms) GetDate() int32`

GetDate returns the Date field if non-nil, zero value otherwise.

### GetDateOk

`func (o *SmsSendSms) GetDateOk() (*int32, bool)`

GetDateOk returns a tuple with the Date field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDate

`func (o *SmsSendSms) SetDate(v int32)`

SetDate sets Date field to given value.

### HasDate

`func (o *SmsSendSms) HasDate() bool`

HasDate returns a boolean if a field has been set.

### GetTo

`func (o *SmsSendSms) GetTo() string`

GetTo returns the To field if non-nil, zero value otherwise.

### GetToOk

`func (o *SmsSendSms) GetToOk() (*string, bool)`

GetToOk returns a tuple with the To field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTo

`func (o *SmsSendSms) SetTo(v string)`

SetTo sets To field to given value.

### HasTo

`func (o *SmsSendSms) HasTo() bool`

HasTo returns a boolean if a field has been set.

### GetBody

`func (o *SmsSendSms) GetBody() string`

GetBody returns the Body field if non-nil, zero value otherwise.

### GetBodyOk

`func (o *SmsSendSms) GetBodyOk() (*string, bool)`

GetBodyOk returns a tuple with the Body field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetBody

`func (o *SmsSendSms) SetBody(v string)`

SetBody sets Body field to given value.

### HasBody

`func (o *SmsSendSms) HasBody() bool`

HasBody returns a boolean if a field has been set.

### GetFrom

`func (o *SmsSendSms) GetFrom() string`

GetFrom returns the From field if non-nil, zero value otherwise.

### GetFromOk

`func (o *SmsSendSms) GetFromOk() (*string, bool)`

GetFromOk returns a tuple with the From field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetFrom

`func (o *SmsSendSms) SetFrom(v string)`

SetFrom sets From field to given value.

### HasFrom

`func (o *SmsSendSms) HasFrom() bool`

HasFrom returns a boolean if a field has been set.

### GetSchedule

`func (o *SmsSendSms) GetSchedule() int32`

GetSchedule returns the Schedule field if non-nil, zero value otherwise.

### GetScheduleOk

`func (o *SmsSendSms) GetScheduleOk() (*int32, bool)`

GetScheduleOk returns a tuple with the Schedule field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSchedule

`func (o *SmsSendSms) SetSchedule(v int32)`

SetSchedule sets Schedule field to given value.

### HasSchedule

`func (o *SmsSendSms) HasSchedule() bool`

HasSchedule returns a boolean if a field has been set.

### GetMessageId

`func (o *SmsSendSms) GetMessageId() string`

GetMessageId returns the MessageId field if non-nil, zero value otherwise.

### GetMessageIdOk

`func (o *SmsSendSms) GetMessageIdOk() (*string, bool)`

GetMessageIdOk returns a tuple with the MessageId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetMessageId

`func (o *SmsSendSms) SetMessageId(v string)`

SetMessageId sets MessageId field to given value.

### HasMessageId

`func (o *SmsSendSms) HasMessageId() bool`

HasMessageId returns a boolean if a field has been set.

### GetMessageParts

`func (o *SmsSendSms) GetMessageParts() int32`

GetMessageParts returns the MessageParts field if non-nil, zero value otherwise.

### GetMessagePartsOk

`func (o *SmsSendSms) GetMessagePartsOk() (*int32, bool)`

GetMessagePartsOk returns a tuple with the MessageParts field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetMessageParts

`func (o *SmsSendSms) SetMessageParts(v int32)`

SetMessageParts sets MessageParts field to given value.

### HasMessageParts

`func (o *SmsSendSms) HasMessageParts() bool`

HasMessageParts returns a boolean if a field has been set.

### GetMessagePrice

`func (o *SmsSendSms) GetMessagePrice() float32`

GetMessagePrice returns the MessagePrice field if non-nil, zero value otherwise.

### GetMessagePriceOk

`func (o *SmsSendSms) GetMessagePriceOk() (*float32, bool)`

GetMessagePriceOk returns a tuple with the MessagePrice field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetMessagePrice

`func (o *SmsSendSms) SetMessagePrice(v float32)`

SetMessagePrice sets MessagePrice field to given value.

### HasMessagePrice

`func (o *SmsSendSms) HasMessagePrice() bool`

HasMessagePrice returns a boolean if a field has been set.

### GetFromEmail

`func (o *SmsSendSms) GetFromEmail() string`

GetFromEmail returns the FromEmail field if non-nil, zero value otherwise.

### GetFromEmailOk

`func (o *SmsSendSms) GetFromEmailOk() (*string, bool)`

GetFromEmailOk returns a tuple with the FromEmail field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetFromEmail

`func (o *SmsSendSms) SetFromEmail(v string)`

SetFromEmail sets FromEmail field to given value.

### HasFromEmail

`func (o *SmsSendSms) HasFromEmail() bool`

HasFromEmail returns a boolean if a field has been set.

### GetListId

`func (o *SmsSendSms) GetListId() string`

GetListId returns the ListId field if non-nil, zero value otherwise.

### GetListIdOk

`func (o *SmsSendSms) GetListIdOk() (*string, bool)`

GetListIdOk returns a tuple with the ListId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetListId

`func (o *SmsSendSms) SetListId(v string)`

SetListId sets ListId field to given value.

### HasListId

`func (o *SmsSendSms) HasListId() bool`

HasListId returns a boolean if a field has been set.

### GetCustomString

`func (o *SmsSendSms) GetCustomString() string`

GetCustomString returns the CustomString field if non-nil, zero value otherwise.

### GetCustomStringOk

`func (o *SmsSendSms) GetCustomStringOk() (*string, bool)`

GetCustomStringOk returns a tuple with the CustomString field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCustomString

`func (o *SmsSendSms) SetCustomString(v string)`

SetCustomString sets CustomString field to given value.

### HasCustomString

`func (o *SmsSendSms) HasCustomString() bool`

HasCustomString returns a boolean if a field has been set.

### GetContactId

`func (o *SmsSendSms) GetContactId() string`

GetContactId returns the ContactId field if non-nil, zero value otherwise.

### GetContactIdOk

`func (o *SmsSendSms) GetContactIdOk() (*string, bool)`

GetContactIdOk returns a tuple with the ContactId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetContactId

`func (o *SmsSendSms) SetContactId(v string)`

SetContactId sets ContactId field to given value.

### HasContactId

`func (o *SmsSendSms) HasContactId() bool`

HasContactId returns a boolean if a field has been set.

### GetUserId

`func (o *SmsSendSms) GetUserId() int32`

GetUserId returns the UserId field if non-nil, zero value otherwise.

### GetUserIdOk

`func (o *SmsSendSms) GetUserIdOk() (*int32, bool)`

GetUserIdOk returns a tuple with the UserId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetUserId

`func (o *SmsSendSms) SetUserId(v int32)`

SetUserId sets UserId field to given value.

### HasUserId

`func (o *SmsSendSms) HasUserId() bool`

HasUserId returns a boolean if a field has been set.

### GetSubaccountId

`func (o *SmsSendSms) GetSubaccountId() int32`

GetSubaccountId returns the SubaccountId field if non-nil, zero value otherwise.

### GetSubaccountIdOk

`func (o *SmsSendSms) GetSubaccountIdOk() (*int32, bool)`

GetSubaccountIdOk returns a tuple with the SubaccountId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSubaccountId

`func (o *SmsSendSms) SetSubaccountId(v int32)`

SetSubaccountId sets SubaccountId field to given value.

### HasSubaccountId

`func (o *SmsSendSms) HasSubaccountId() bool`

HasSubaccountId returns a boolean if a field has been set.

### GetIsSharedSystemNumber

`func (o *SmsSendSms) GetIsSharedSystemNumber() bool`

GetIsSharedSystemNumber returns the IsSharedSystemNumber field if non-nil, zero value otherwise.

### GetIsSharedSystemNumberOk

`func (o *SmsSendSms) GetIsSharedSystemNumberOk() (*bool, bool)`

GetIsSharedSystemNumberOk returns a tuple with the IsSharedSystemNumber field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetIsSharedSystemNumber

`func (o *SmsSendSms) SetIsSharedSystemNumber(v bool)`

SetIsSharedSystemNumber sets IsSharedSystemNumber field to given value.

### HasIsSharedSystemNumber

`func (o *SmsSendSms) HasIsSharedSystemNumber() bool`

HasIsSharedSystemNumber returns a boolean if a field has been set.

### GetCountry

`func (o *SmsSendSms) GetCountry() string`

GetCountry returns the Country field if non-nil, zero value otherwise.

### GetCountryOk

`func (o *SmsSendSms) GetCountryOk() (*string, bool)`

GetCountryOk returns a tuple with the Country field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCountry

`func (o *SmsSendSms) SetCountry(v string)`

SetCountry sets Country field to given value.

### HasCountry

`func (o *SmsSendSms) HasCountry() bool`

HasCountry returns a boolean if a field has been set.

### GetCarrier

`func (o *SmsSendSms) GetCarrier() string`

GetCarrier returns the Carrier field if non-nil, zero value otherwise.

### GetCarrierOk

`func (o *SmsSendSms) GetCarrierOk() (*string, bool)`

GetCarrierOk returns a tuple with the Carrier field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCarrier

`func (o *SmsSendSms) SetCarrier(v string)`

SetCarrier sets Carrier field to given value.

### HasCarrier

`func (o *SmsSendSms) HasCarrier() bool`

HasCarrier returns a boolean if a field has been set.

### GetStatus

`func (o *SmsSendSms) GetStatus() string`

GetStatus returns the Status field if non-nil, zero value otherwise.

### GetStatusOk

`func (o *SmsSendSms) GetStatusOk() (*string, bool)`

GetStatusOk returns a tuple with the Status field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetStatus

`func (o *SmsSendSms) SetStatus(v string)`

SetStatus sets Status field to given value.

### HasStatus

`func (o *SmsSendSms) HasStatus() bool`

HasStatus returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


