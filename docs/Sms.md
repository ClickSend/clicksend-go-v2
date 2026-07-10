# Sms

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Date** | Pointer to **int32** | The date you sent the message. It is in &lt;a href&#x3D;\&quot;http://help.clicksend.com/what-is-a-unix-timestamp\&quot; target&#x3D;\&quot;_blank\&quot;&gt;Unix format&lt;/a&gt;. | [optional] 
**To** | Pointer to **string** | The phone number of the recipient. It should be in &lt;a href&#x3D;\&quot;https://en.wikipedia.org/wiki/E.164\&quot; target&#x3D;\&quot;_blank\&quot;&gt;E.164 format&lt;/a&gt;. | [optional] 
**Body** | Pointer to **string** | The message sent. The price of sending a message depends on the number of characters and the type of message. There are two types:  - Standard message - Contains only characters in the &lt;a href&#x3D;\&quot;https://en.wikipedia.org/wiki/GSM_03.38\&quot; target&#x3D;\&quot;_blank\&quot;&gt;GSM&lt;/a&gt; set, with a maximum of 160 characters.      - Unicode message - Contains characters outside the &lt;a href&#x3D;\&quot;https://en.wikipedia.org/wiki/GSM_03.38\&quot; target&#x3D;\&quot;_blank\&quot;&gt;GSM&lt;/a&gt; set, with a maximum of 70 characters.       Longer messages will be sent as multiple messages (parts), but the recipient will receive them as a single long message. Visit &lt;a href&#x3D;\&quot;https://help.clicksend.com/article/h474eseq3a-how-many-characters-can-i-send-in-an-sms\&quot; target&#x3D;\&quot;_blank\&quot;&gt;this page&lt;/a&gt; to learn more about the number of characters per message, and &lt;a href&#x3D;\&quot;http://smscharactercount.com/\&quot; target&#x3D;\&quot;_blank\&quot;&gt;this page&lt;/a&gt; to count the number of characters. | [optional] 
**From** | Pointer to **string** | The sender of the message. This is also referred to as the **Sender ID**. If your **Sender ID** has a different country code to the recipient’s, it&#39;ll be replaced by a local number, except in &lt;a href&#x3D;\&quot;https://help.clicksend.com/category/mfdctha7f0-country-specific-features-and-restrictions\&quot; target&#x3D;\&quot;_blank\&quot;&gt;certain countries&lt;/a&gt;. If the sender number is blocked, a different number will replace it. | [optional] 
**Schedule** | Pointer to **string** | The scheduled date of the message. It is in &lt;a href&#x3D;\&quot;http://help.clicksend.com/what-is-a-unix-timestamp\&quot; target&#x3D;\&quot;_blank\&quot;&gt;Unix format&lt;/a&gt;. | [optional] 
**MessageId** | Pointer to **string** | The generated ID of the message. This ID is typically used as a reference for &lt;a href&#x3D;\&quot;https://www.clicksend.com/au/help/\&quot; target&#x3D;\&quot;_blank\&quot;&gt;customer support&lt;/a&gt; in case of any issues. | [optional] 
**MessageParts** | Pointer to **int32** | The number of parts the message was broken into. To look at how many parts your message is broken down into, use the **&lt;a href&#x3D;\&quot;http://smscharactercount.com/\&quot;&gt;SMS Character Count&lt;/a&gt;**. | [optional] 
**MessagePrice** | Pointer to **string** | The price of this message. This depends on the total number of parts of the message. | [optional] 
**CustomString** | Pointer to **string** | A note that was sent from the request. | [optional] 
**ContactId** | Pointer to **string** | This is the ID of the contact. This parameter will have a **null** value if you didn’t provide a _contact_id_ in the request. | [optional] 
**IsSharedSystemNumber** | Pointer to **bool** | Indicates whether you use a shared number to send a message:  - **True** \\- if the sender is randomly selected.      - **False** \\- if the sender is specified and passed the validation process. | [optional] 
**Country** | Pointer to **string** | The country of the recipient in two-letter format (e.g. US, UK, AU, NZ, etc). | [optional] 
**Status** | Pointer to **string** | The response code of the operation. Visit [this page](/#application-status-codes) for more information. This reflects the actual status of the individual message. | [optional] 

## Methods

### NewSms

`func NewSms() *Sms`

NewSms instantiates a new Sms object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewSmsWithDefaults

`func NewSmsWithDefaults() *Sms`

NewSmsWithDefaults instantiates a new Sms object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetDate

`func (o *Sms) GetDate() int32`

GetDate returns the Date field if non-nil, zero value otherwise.

### GetDateOk

`func (o *Sms) GetDateOk() (*int32, bool)`

GetDateOk returns a tuple with the Date field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDate

`func (o *Sms) SetDate(v int32)`

SetDate sets Date field to given value.

### HasDate

`func (o *Sms) HasDate() bool`

HasDate returns a boolean if a field has been set.

### GetTo

`func (o *Sms) GetTo() string`

GetTo returns the To field if non-nil, zero value otherwise.

### GetToOk

`func (o *Sms) GetToOk() (*string, bool)`

GetToOk returns a tuple with the To field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTo

`func (o *Sms) SetTo(v string)`

SetTo sets To field to given value.

### HasTo

`func (o *Sms) HasTo() bool`

HasTo returns a boolean if a field has been set.

### GetBody

`func (o *Sms) GetBody() string`

GetBody returns the Body field if non-nil, zero value otherwise.

### GetBodyOk

`func (o *Sms) GetBodyOk() (*string, bool)`

GetBodyOk returns a tuple with the Body field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetBody

`func (o *Sms) SetBody(v string)`

SetBody sets Body field to given value.

### HasBody

`func (o *Sms) HasBody() bool`

HasBody returns a boolean if a field has been set.

### GetFrom

`func (o *Sms) GetFrom() string`

GetFrom returns the From field if non-nil, zero value otherwise.

### GetFromOk

`func (o *Sms) GetFromOk() (*string, bool)`

GetFromOk returns a tuple with the From field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetFrom

`func (o *Sms) SetFrom(v string)`

SetFrom sets From field to given value.

### HasFrom

`func (o *Sms) HasFrom() bool`

HasFrom returns a boolean if a field has been set.

### GetSchedule

`func (o *Sms) GetSchedule() string`

GetSchedule returns the Schedule field if non-nil, zero value otherwise.

### GetScheduleOk

`func (o *Sms) GetScheduleOk() (*string, bool)`

GetScheduleOk returns a tuple with the Schedule field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSchedule

`func (o *Sms) SetSchedule(v string)`

SetSchedule sets Schedule field to given value.

### HasSchedule

`func (o *Sms) HasSchedule() bool`

HasSchedule returns a boolean if a field has been set.

### GetMessageId

`func (o *Sms) GetMessageId() string`

GetMessageId returns the MessageId field if non-nil, zero value otherwise.

### GetMessageIdOk

`func (o *Sms) GetMessageIdOk() (*string, bool)`

GetMessageIdOk returns a tuple with the MessageId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetMessageId

`func (o *Sms) SetMessageId(v string)`

SetMessageId sets MessageId field to given value.

### HasMessageId

`func (o *Sms) HasMessageId() bool`

HasMessageId returns a boolean if a field has been set.

### GetMessageParts

`func (o *Sms) GetMessageParts() int32`

GetMessageParts returns the MessageParts field if non-nil, zero value otherwise.

### GetMessagePartsOk

`func (o *Sms) GetMessagePartsOk() (*int32, bool)`

GetMessagePartsOk returns a tuple with the MessageParts field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetMessageParts

`func (o *Sms) SetMessageParts(v int32)`

SetMessageParts sets MessageParts field to given value.

### HasMessageParts

`func (o *Sms) HasMessageParts() bool`

HasMessageParts returns a boolean if a field has been set.

### GetMessagePrice

`func (o *Sms) GetMessagePrice() string`

GetMessagePrice returns the MessagePrice field if non-nil, zero value otherwise.

### GetMessagePriceOk

`func (o *Sms) GetMessagePriceOk() (*string, bool)`

GetMessagePriceOk returns a tuple with the MessagePrice field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetMessagePrice

`func (o *Sms) SetMessagePrice(v string)`

SetMessagePrice sets MessagePrice field to given value.

### HasMessagePrice

`func (o *Sms) HasMessagePrice() bool`

HasMessagePrice returns a boolean if a field has been set.

### GetCustomString

`func (o *Sms) GetCustomString() string`

GetCustomString returns the CustomString field if non-nil, zero value otherwise.

### GetCustomStringOk

`func (o *Sms) GetCustomStringOk() (*string, bool)`

GetCustomStringOk returns a tuple with the CustomString field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCustomString

`func (o *Sms) SetCustomString(v string)`

SetCustomString sets CustomString field to given value.

### HasCustomString

`func (o *Sms) HasCustomString() bool`

HasCustomString returns a boolean if a field has been set.

### GetContactId

`func (o *Sms) GetContactId() string`

GetContactId returns the ContactId field if non-nil, zero value otherwise.

### GetContactIdOk

`func (o *Sms) GetContactIdOk() (*string, bool)`

GetContactIdOk returns a tuple with the ContactId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetContactId

`func (o *Sms) SetContactId(v string)`

SetContactId sets ContactId field to given value.

### HasContactId

`func (o *Sms) HasContactId() bool`

HasContactId returns a boolean if a field has been set.

### GetIsSharedSystemNumber

`func (o *Sms) GetIsSharedSystemNumber() bool`

GetIsSharedSystemNumber returns the IsSharedSystemNumber field if non-nil, zero value otherwise.

### GetIsSharedSystemNumberOk

`func (o *Sms) GetIsSharedSystemNumberOk() (*bool, bool)`

GetIsSharedSystemNumberOk returns a tuple with the IsSharedSystemNumber field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetIsSharedSystemNumber

`func (o *Sms) SetIsSharedSystemNumber(v bool)`

SetIsSharedSystemNumber sets IsSharedSystemNumber field to given value.

### HasIsSharedSystemNumber

`func (o *Sms) HasIsSharedSystemNumber() bool`

HasIsSharedSystemNumber returns a boolean if a field has been set.

### GetCountry

`func (o *Sms) GetCountry() string`

GetCountry returns the Country field if non-nil, zero value otherwise.

### GetCountryOk

`func (o *Sms) GetCountryOk() (*string, bool)`

GetCountryOk returns a tuple with the Country field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCountry

`func (o *Sms) SetCountry(v string)`

SetCountry sets Country field to given value.

### HasCountry

`func (o *Sms) HasCountry() bool`

HasCountry returns a boolean if a field has been set.

### GetStatus

`func (o *Sms) GetStatus() string`

GetStatus returns the Status field if non-nil, zero value otherwise.

### GetStatusOk

`func (o *Sms) GetStatusOk() (*string, bool)`

GetStatusOk returns a tuple with the Status field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetStatus

`func (o *Sms) SetStatus(v string)`

SetStatus sets Status field to given value.

### HasStatus

`func (o *Sms) HasStatus() bool`

HasStatus returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


