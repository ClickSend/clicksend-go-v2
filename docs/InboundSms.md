# InboundSms

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Timestamp** | Pointer to **int32** | The time you receive the inbound message.. It’s in the &lt;a href&#x3D;\&quot;http://help.clicksend.com/what-is-a-unix-timestamp\&quot;&gt;Unix format.&lt;/a&gt; | [optional] 
**From** | Pointer to **string** | The sender of the message, which is the phone number of the recipient who replied to you. Your recipient can’t reply to an alpha tag (business name). | [optional] 
**Body** | Pointer to **string** | The message you received from your recipient. | [optional] 
**OriginalBody** | Pointer to **string** | The last message you sent to your recipient. | [optional] 
**OriginalMessageId** | Pointer to **string** | The generated ID of the message that you sent to your receipient. | [optional] 
**To** | Pointer to **string** | The receiver of the inbound message, which can be either the shared number or the dedicated number you used to send the message. | [optional] 
**CustomString** | Pointer to **string** | A note that was included with the inbound SMS. If no note was included, the value will be an empty string. | [optional] 
**MessageId** | Pointer to **string** | The generated ID of the inbound SMS. This ID is typically used as a reference for &lt;a href&#x3D;\&quot;https://www.clicksend.com/au/help/\&quot; target&#x3D;\&quot;_blank\&quot;&gt;customer support&lt;/a&gt; in case of any issues. | [optional] 
**Keyword** | Pointer to **string** | The keyword of the inbound SMS.  &lt;div class&#x3D;\&quot;warning-box\&quot;&gt;   &lt;h4&gt;&lt;i class&#x3D;\&quot;fas fa-exclamation-triangle\&quot;&gt;&lt;/i&gt; Warning:&lt;/h4&gt;   &lt;p&gt;This parameter is deprecated and will return the first word of the body message.&lt;/p&gt; &lt;/div&gt; | [optional] 

## Methods

### NewInboundSms

`func NewInboundSms() *InboundSms`

NewInboundSms instantiates a new InboundSms object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewInboundSmsWithDefaults

`func NewInboundSmsWithDefaults() *InboundSms`

NewInboundSmsWithDefaults instantiates a new InboundSms object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetTimestamp

`func (o *InboundSms) GetTimestamp() int32`

GetTimestamp returns the Timestamp field if non-nil, zero value otherwise.

### GetTimestampOk

`func (o *InboundSms) GetTimestampOk() (*int32, bool)`

GetTimestampOk returns a tuple with the Timestamp field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTimestamp

`func (o *InboundSms) SetTimestamp(v int32)`

SetTimestamp sets Timestamp field to given value.

### HasTimestamp

`func (o *InboundSms) HasTimestamp() bool`

HasTimestamp returns a boolean if a field has been set.

### GetFrom

`func (o *InboundSms) GetFrom() string`

GetFrom returns the From field if non-nil, zero value otherwise.

### GetFromOk

`func (o *InboundSms) GetFromOk() (*string, bool)`

GetFromOk returns a tuple with the From field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetFrom

`func (o *InboundSms) SetFrom(v string)`

SetFrom sets From field to given value.

### HasFrom

`func (o *InboundSms) HasFrom() bool`

HasFrom returns a boolean if a field has been set.

### GetBody

`func (o *InboundSms) GetBody() string`

GetBody returns the Body field if non-nil, zero value otherwise.

### GetBodyOk

`func (o *InboundSms) GetBodyOk() (*string, bool)`

GetBodyOk returns a tuple with the Body field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetBody

`func (o *InboundSms) SetBody(v string)`

SetBody sets Body field to given value.

### HasBody

`func (o *InboundSms) HasBody() bool`

HasBody returns a boolean if a field has been set.

### GetOriginalBody

`func (o *InboundSms) GetOriginalBody() string`

GetOriginalBody returns the OriginalBody field if non-nil, zero value otherwise.

### GetOriginalBodyOk

`func (o *InboundSms) GetOriginalBodyOk() (*string, bool)`

GetOriginalBodyOk returns a tuple with the OriginalBody field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetOriginalBody

`func (o *InboundSms) SetOriginalBody(v string)`

SetOriginalBody sets OriginalBody field to given value.

### HasOriginalBody

`func (o *InboundSms) HasOriginalBody() bool`

HasOriginalBody returns a boolean if a field has been set.

### GetOriginalMessageId

`func (o *InboundSms) GetOriginalMessageId() string`

GetOriginalMessageId returns the OriginalMessageId field if non-nil, zero value otherwise.

### GetOriginalMessageIdOk

`func (o *InboundSms) GetOriginalMessageIdOk() (*string, bool)`

GetOriginalMessageIdOk returns a tuple with the OriginalMessageId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetOriginalMessageId

`func (o *InboundSms) SetOriginalMessageId(v string)`

SetOriginalMessageId sets OriginalMessageId field to given value.

### HasOriginalMessageId

`func (o *InboundSms) HasOriginalMessageId() bool`

HasOriginalMessageId returns a boolean if a field has been set.

### GetTo

`func (o *InboundSms) GetTo() string`

GetTo returns the To field if non-nil, zero value otherwise.

### GetToOk

`func (o *InboundSms) GetToOk() (*string, bool)`

GetToOk returns a tuple with the To field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTo

`func (o *InboundSms) SetTo(v string)`

SetTo sets To field to given value.

### HasTo

`func (o *InboundSms) HasTo() bool`

HasTo returns a boolean if a field has been set.

### GetCustomString

`func (o *InboundSms) GetCustomString() string`

GetCustomString returns the CustomString field if non-nil, zero value otherwise.

### GetCustomStringOk

`func (o *InboundSms) GetCustomStringOk() (*string, bool)`

GetCustomStringOk returns a tuple with the CustomString field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCustomString

`func (o *InboundSms) SetCustomString(v string)`

SetCustomString sets CustomString field to given value.

### HasCustomString

`func (o *InboundSms) HasCustomString() bool`

HasCustomString returns a boolean if a field has been set.

### GetMessageId

`func (o *InboundSms) GetMessageId() string`

GetMessageId returns the MessageId field if non-nil, zero value otherwise.

### GetMessageIdOk

`func (o *InboundSms) GetMessageIdOk() (*string, bool)`

GetMessageIdOk returns a tuple with the MessageId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetMessageId

`func (o *InboundSms) SetMessageId(v string)`

SetMessageId sets MessageId field to given value.

### HasMessageId

`func (o *InboundSms) HasMessageId() bool`

HasMessageId returns a boolean if a field has been set.

### GetKeyword

`func (o *InboundSms) GetKeyword() string`

GetKeyword returns the Keyword field if non-nil, zero value otherwise.

### GetKeywordOk

`func (o *InboundSms) GetKeywordOk() (*string, bool)`

GetKeywordOk returns a tuple with the Keyword field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetKeyword

`func (o *InboundSms) SetKeyword(v string)`

SetKeyword sets Keyword field to given value.

### HasKeyword

`func (o *InboundSms) HasKeyword() bool`

HasKeyword returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


