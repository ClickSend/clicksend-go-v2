# InboundSmsTest

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**TimestampSend** | Pointer to **int32** | The time you sent the test message. It’s in the &lt;a href&#x3D;\&quot;http://help.clicksend.com/what-is-a-unix-timestamp\&quot;&gt;Unix format.&lt;/a&gt; | [optional] 
**From** | Pointer to **string** | This is a random number used for testing purposes. | [optional] 
**Body** | Pointer to **string** | The sample test message. | [optional] 
**OriginalBody** | Pointer to **string** | The sample test message you sent to your recipient. | [optional] 
**OriginalMessageId** | Pointer to **string** | The generated ID of the message that you sent to your receipient.  &lt;div class&#x3D;\&quot;info-box\&quot;&gt;   &lt;h4&gt;&lt;i class&#x3D;\&quot;fas fa-info-circle\&quot;&gt;&lt;/i&gt; Note:&lt;/h4&gt;   &lt;p&gt;This &lt;em&gt;original_message_id&lt;/em&gt; is different from the ID that is generated when sending an actual SMS. This ID is used for testing only.&lt;/p&gt; &lt;/div&gt; | [optional] 
**To** | Pointer to **string** | The receiver of the inbound message, which can be either the shared number or the dedicated number you used to send the message. | [optional] 
**CustomString** | Pointer to **string** | The sample test note that was included with the inbound SMS. | [optional] 
**MessageId** | Pointer to **string** | The generated ID of the inbound SMS. This ID is typically used as a reference for &lt;a href&#x3D;\&quot;https://www.clicksend.com/au/help/\&quot; target&#x3D;\&quot;_blank\&quot;&gt;customer support&lt;/a&gt; in case of any issues. | [optional] 
**Keyword** | Pointer to **string** | The keyword of the inbound SMS.  &lt;div class&#x3D;\&quot;warning-box\&quot;&gt;   &lt;h4&gt;&lt;i class&#x3D;\&quot;fas fa-exclamation-triangle\&quot;&gt;&lt;/i&gt; Warning:&lt;/h4&gt;   &lt;p&gt;This parameter is deprecated and will return &lt;strong&gt;null.&lt;/strong&gt;&lt;/p&gt; &lt;/div&gt; | [optional] 

## Methods

### NewInboundSmsTest

`func NewInboundSmsTest() *InboundSmsTest`

NewInboundSmsTest instantiates a new InboundSmsTest object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewInboundSmsTestWithDefaults

`func NewInboundSmsTestWithDefaults() *InboundSmsTest`

NewInboundSmsTestWithDefaults instantiates a new InboundSmsTest object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetTimestampSend

`func (o *InboundSmsTest) GetTimestampSend() int32`

GetTimestampSend returns the TimestampSend field if non-nil, zero value otherwise.

### GetTimestampSendOk

`func (o *InboundSmsTest) GetTimestampSendOk() (*int32, bool)`

GetTimestampSendOk returns a tuple with the TimestampSend field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTimestampSend

`func (o *InboundSmsTest) SetTimestampSend(v int32)`

SetTimestampSend sets TimestampSend field to given value.

### HasTimestampSend

`func (o *InboundSmsTest) HasTimestampSend() bool`

HasTimestampSend returns a boolean if a field has been set.

### GetFrom

`func (o *InboundSmsTest) GetFrom() string`

GetFrom returns the From field if non-nil, zero value otherwise.

### GetFromOk

`func (o *InboundSmsTest) GetFromOk() (*string, bool)`

GetFromOk returns a tuple with the From field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetFrom

`func (o *InboundSmsTest) SetFrom(v string)`

SetFrom sets From field to given value.

### HasFrom

`func (o *InboundSmsTest) HasFrom() bool`

HasFrom returns a boolean if a field has been set.

### GetBody

`func (o *InboundSmsTest) GetBody() string`

GetBody returns the Body field if non-nil, zero value otherwise.

### GetBodyOk

`func (o *InboundSmsTest) GetBodyOk() (*string, bool)`

GetBodyOk returns a tuple with the Body field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetBody

`func (o *InboundSmsTest) SetBody(v string)`

SetBody sets Body field to given value.

### HasBody

`func (o *InboundSmsTest) HasBody() bool`

HasBody returns a boolean if a field has been set.

### GetOriginalBody

`func (o *InboundSmsTest) GetOriginalBody() string`

GetOriginalBody returns the OriginalBody field if non-nil, zero value otherwise.

### GetOriginalBodyOk

`func (o *InboundSmsTest) GetOriginalBodyOk() (*string, bool)`

GetOriginalBodyOk returns a tuple with the OriginalBody field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetOriginalBody

`func (o *InboundSmsTest) SetOriginalBody(v string)`

SetOriginalBody sets OriginalBody field to given value.

### HasOriginalBody

`func (o *InboundSmsTest) HasOriginalBody() bool`

HasOriginalBody returns a boolean if a field has been set.

### GetOriginalMessageId

`func (o *InboundSmsTest) GetOriginalMessageId() string`

GetOriginalMessageId returns the OriginalMessageId field if non-nil, zero value otherwise.

### GetOriginalMessageIdOk

`func (o *InboundSmsTest) GetOriginalMessageIdOk() (*string, bool)`

GetOriginalMessageIdOk returns a tuple with the OriginalMessageId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetOriginalMessageId

`func (o *InboundSmsTest) SetOriginalMessageId(v string)`

SetOriginalMessageId sets OriginalMessageId field to given value.

### HasOriginalMessageId

`func (o *InboundSmsTest) HasOriginalMessageId() bool`

HasOriginalMessageId returns a boolean if a field has been set.

### GetTo

`func (o *InboundSmsTest) GetTo() string`

GetTo returns the To field if non-nil, zero value otherwise.

### GetToOk

`func (o *InboundSmsTest) GetToOk() (*string, bool)`

GetToOk returns a tuple with the To field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTo

`func (o *InboundSmsTest) SetTo(v string)`

SetTo sets To field to given value.

### HasTo

`func (o *InboundSmsTest) HasTo() bool`

HasTo returns a boolean if a field has been set.

### GetCustomString

`func (o *InboundSmsTest) GetCustomString() string`

GetCustomString returns the CustomString field if non-nil, zero value otherwise.

### GetCustomStringOk

`func (o *InboundSmsTest) GetCustomStringOk() (*string, bool)`

GetCustomStringOk returns a tuple with the CustomString field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCustomString

`func (o *InboundSmsTest) SetCustomString(v string)`

SetCustomString sets CustomString field to given value.

### HasCustomString

`func (o *InboundSmsTest) HasCustomString() bool`

HasCustomString returns a boolean if a field has been set.

### GetMessageId

`func (o *InboundSmsTest) GetMessageId() string`

GetMessageId returns the MessageId field if non-nil, zero value otherwise.

### GetMessageIdOk

`func (o *InboundSmsTest) GetMessageIdOk() (*string, bool)`

GetMessageIdOk returns a tuple with the MessageId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetMessageId

`func (o *InboundSmsTest) SetMessageId(v string)`

SetMessageId sets MessageId field to given value.

### HasMessageId

`func (o *InboundSmsTest) HasMessageId() bool`

HasMessageId returns a boolean if a field has been set.

### GetKeyword

`func (o *InboundSmsTest) GetKeyword() string`

GetKeyword returns the Keyword field if non-nil, zero value otherwise.

### GetKeywordOk

`func (o *InboundSmsTest) GetKeywordOk() (*string, bool)`

GetKeywordOk returns a tuple with the Keyword field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetKeyword

`func (o *InboundSmsTest) SetKeyword(v string)`

SetKeyword sets Keyword field to given value.

### HasKeyword

`func (o *InboundSmsTest) HasKeyword() bool`

HasKeyword returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


