# SmsReceipt

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**TimestampSend** | Pointer to **int32** | The time you sent the test message. It’s in the &lt;a target&#x3D;\&quot;_blank\&quot; href&#x3D;\&quot;http://help.clicksend.com/what-is-a-unix-timestamp\&quot;&gt;Unix format&lt;/a&gt;. | [optional] 
**Timestamp** | Pointer to **int32** | The time you receive the test message receipt. It’s in the &lt;a target&#x3D;\&quot;_blank\&quot; href&#x3D;\&quot;http://help.clicksend.com/what-is-a-unix-timestamp\&quot;&gt;Unix format&lt;/a&gt;. | [optional] 
**MessageId** | Pointer to **string** | The generated ID of the message. This ID is typically used as a reference for &lt;a target&#x3D;\&quot;_blank\&quot; href&#x3D;\&quot;https://www.clicksend.com/au/help/\&quot;&gt;customer support&lt;/a&gt; in case of any issues. | [optional] 
**StatusCode** | Pointer to **int32** | The status code sent from the &lt;a target&#x3D;\&quot;_blank\&quot; href&#x3D;\&quot;https://en.wikipedia.org/wiki/SMS_gateway\&quot;&gt;SMS gateway&lt;/a&gt;. Visit &lt;a href&#x3D;\&quot;https://help.clicksend.com/article/8cc479qlbb-list-of-sms-gateway-error-codes\&quot;&gt;this page&lt;/a&gt; for more information. | [optional] 
**StatusText** | Pointer to **string** | A message describing the status_code of the operation. Visit &lt;a href&#x3D;\&quot;https://help.clicksend.com/article/8cc479qlbb-list-of-sms-gateway-error-codes\&quot;&gt;this page&lt;/a&gt; for more information. | [optional] 
**ErrorCode** | Pointer to **NullableInt32** | The error code of the operation. Visit &lt;a href&#x3D;\&quot;https://help.clicksend.com/article/8cc479qlbb-list-of-sms-gateway-error-codes\&quot;&gt;this page&lt;/a&gt; for more information. If no error occurred, the value is **null**. | [optional] 
**ErrorText** | Pointer to **NullableString** | A message describing the _error_code_ of the operation. Visit &lt;a href&#x3D;\&quot;https://help.clicksend.com/article/8cc479qlbb-list-of-sms-gateway-error-codes\&quot;&gt;this page&lt;/a&gt; for more information. If no error occurred, the value is **null**. | [optional] 
**CustomString** | Pointer to **NullableString** | A note that was included with the outgoing SMS. If no note was included, the value is **null**. | [optional] 
**SubaccountId** | Pointer to **int32** | The sub-account of the user. A user can have multiple sub-accounts. | [optional] 
**MessageType** | Pointer to **string** | The type of message (e.g. SMS, MMS, etc). | [optional] 
**Digits** | Pointer to **int32** | The numbers that the recipient pressed on their keypad during the call. A **null** value is returned if the recipient didn&#39;t provide any input.  &lt;div class&#x3D;\&quot;info-box\&quot;&gt;   &lt;h4&gt;&lt;i class&#x3D;\&quot;fas fa-info-circle\&quot;&gt;&lt;/i&gt; Note:&lt;/h4&gt;   &lt;p&gt;This parameter is only relevant to &lt;a target&#x3D;\&quot;_blank\&quot; href&#x3D;\&quot;/messaging/voice-messaging/\&quot;&gt;&lt;strong&gt;Voice Messaging&lt;/strong&gt;&lt;/a&gt; receipts.&lt;/p&gt; &lt;/div&gt; | [optional] 

## Methods

### NewSmsReceipt

`func NewSmsReceipt() *SmsReceipt`

NewSmsReceipt instantiates a new SmsReceipt object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewSmsReceiptWithDefaults

`func NewSmsReceiptWithDefaults() *SmsReceipt`

NewSmsReceiptWithDefaults instantiates a new SmsReceipt object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetTimestampSend

`func (o *SmsReceipt) GetTimestampSend() int32`

GetTimestampSend returns the TimestampSend field if non-nil, zero value otherwise.

### GetTimestampSendOk

`func (o *SmsReceipt) GetTimestampSendOk() (*int32, bool)`

GetTimestampSendOk returns a tuple with the TimestampSend field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTimestampSend

`func (o *SmsReceipt) SetTimestampSend(v int32)`

SetTimestampSend sets TimestampSend field to given value.

### HasTimestampSend

`func (o *SmsReceipt) HasTimestampSend() bool`

HasTimestampSend returns a boolean if a field has been set.

### GetTimestamp

`func (o *SmsReceipt) GetTimestamp() int32`

GetTimestamp returns the Timestamp field if non-nil, zero value otherwise.

### GetTimestampOk

`func (o *SmsReceipt) GetTimestampOk() (*int32, bool)`

GetTimestampOk returns a tuple with the Timestamp field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTimestamp

`func (o *SmsReceipt) SetTimestamp(v int32)`

SetTimestamp sets Timestamp field to given value.

### HasTimestamp

`func (o *SmsReceipt) HasTimestamp() bool`

HasTimestamp returns a boolean if a field has been set.

### GetMessageId

`func (o *SmsReceipt) GetMessageId() string`

GetMessageId returns the MessageId field if non-nil, zero value otherwise.

### GetMessageIdOk

`func (o *SmsReceipt) GetMessageIdOk() (*string, bool)`

GetMessageIdOk returns a tuple with the MessageId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetMessageId

`func (o *SmsReceipt) SetMessageId(v string)`

SetMessageId sets MessageId field to given value.

### HasMessageId

`func (o *SmsReceipt) HasMessageId() bool`

HasMessageId returns a boolean if a field has been set.

### GetStatusCode

`func (o *SmsReceipt) GetStatusCode() int32`

GetStatusCode returns the StatusCode field if non-nil, zero value otherwise.

### GetStatusCodeOk

`func (o *SmsReceipt) GetStatusCodeOk() (*int32, bool)`

GetStatusCodeOk returns a tuple with the StatusCode field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetStatusCode

`func (o *SmsReceipt) SetStatusCode(v int32)`

SetStatusCode sets StatusCode field to given value.

### HasStatusCode

`func (o *SmsReceipt) HasStatusCode() bool`

HasStatusCode returns a boolean if a field has been set.

### GetStatusText

`func (o *SmsReceipt) GetStatusText() string`

GetStatusText returns the StatusText field if non-nil, zero value otherwise.

### GetStatusTextOk

`func (o *SmsReceipt) GetStatusTextOk() (*string, bool)`

GetStatusTextOk returns a tuple with the StatusText field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetStatusText

`func (o *SmsReceipt) SetStatusText(v string)`

SetStatusText sets StatusText field to given value.

### HasStatusText

`func (o *SmsReceipt) HasStatusText() bool`

HasStatusText returns a boolean if a field has been set.

### GetErrorCode

`func (o *SmsReceipt) GetErrorCode() int32`

GetErrorCode returns the ErrorCode field if non-nil, zero value otherwise.

### GetErrorCodeOk

`func (o *SmsReceipt) GetErrorCodeOk() (*int32, bool)`

GetErrorCodeOk returns a tuple with the ErrorCode field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetErrorCode

`func (o *SmsReceipt) SetErrorCode(v int32)`

SetErrorCode sets ErrorCode field to given value.

### HasErrorCode

`func (o *SmsReceipt) HasErrorCode() bool`

HasErrorCode returns a boolean if a field has been set.

### SetErrorCodeNil

`func (o *SmsReceipt) SetErrorCodeNil(b bool)`

 SetErrorCodeNil sets the value for ErrorCode to be an explicit nil

### UnsetErrorCode
`func (o *SmsReceipt) UnsetErrorCode()`

UnsetErrorCode ensures that no value is present for ErrorCode, not even an explicit nil
### GetErrorText

`func (o *SmsReceipt) GetErrorText() string`

GetErrorText returns the ErrorText field if non-nil, zero value otherwise.

### GetErrorTextOk

`func (o *SmsReceipt) GetErrorTextOk() (*string, bool)`

GetErrorTextOk returns a tuple with the ErrorText field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetErrorText

`func (o *SmsReceipt) SetErrorText(v string)`

SetErrorText sets ErrorText field to given value.

### HasErrorText

`func (o *SmsReceipt) HasErrorText() bool`

HasErrorText returns a boolean if a field has been set.

### SetErrorTextNil

`func (o *SmsReceipt) SetErrorTextNil(b bool)`

 SetErrorTextNil sets the value for ErrorText to be an explicit nil

### UnsetErrorText
`func (o *SmsReceipt) UnsetErrorText()`

UnsetErrorText ensures that no value is present for ErrorText, not even an explicit nil
### GetCustomString

`func (o *SmsReceipt) GetCustomString() string`

GetCustomString returns the CustomString field if non-nil, zero value otherwise.

### GetCustomStringOk

`func (o *SmsReceipt) GetCustomStringOk() (*string, bool)`

GetCustomStringOk returns a tuple with the CustomString field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCustomString

`func (o *SmsReceipt) SetCustomString(v string)`

SetCustomString sets CustomString field to given value.

### HasCustomString

`func (o *SmsReceipt) HasCustomString() bool`

HasCustomString returns a boolean if a field has been set.

### SetCustomStringNil

`func (o *SmsReceipt) SetCustomStringNil(b bool)`

 SetCustomStringNil sets the value for CustomString to be an explicit nil

### UnsetCustomString
`func (o *SmsReceipt) UnsetCustomString()`

UnsetCustomString ensures that no value is present for CustomString, not even an explicit nil
### GetSubaccountId

`func (o *SmsReceipt) GetSubaccountId() int32`

GetSubaccountId returns the SubaccountId field if non-nil, zero value otherwise.

### GetSubaccountIdOk

`func (o *SmsReceipt) GetSubaccountIdOk() (*int32, bool)`

GetSubaccountIdOk returns a tuple with the SubaccountId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSubaccountId

`func (o *SmsReceipt) SetSubaccountId(v int32)`

SetSubaccountId sets SubaccountId field to given value.

### HasSubaccountId

`func (o *SmsReceipt) HasSubaccountId() bool`

HasSubaccountId returns a boolean if a field has been set.

### GetMessageType

`func (o *SmsReceipt) GetMessageType() string`

GetMessageType returns the MessageType field if non-nil, zero value otherwise.

### GetMessageTypeOk

`func (o *SmsReceipt) GetMessageTypeOk() (*string, bool)`

GetMessageTypeOk returns a tuple with the MessageType field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetMessageType

`func (o *SmsReceipt) SetMessageType(v string)`

SetMessageType sets MessageType field to given value.

### HasMessageType

`func (o *SmsReceipt) HasMessageType() bool`

HasMessageType returns a boolean if a field has been set.

### GetDigits

`func (o *SmsReceipt) GetDigits() int32`

GetDigits returns the Digits field if non-nil, zero value otherwise.

### GetDigitsOk

`func (o *SmsReceipt) GetDigitsOk() (*int32, bool)`

GetDigitsOk returns a tuple with the Digits field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDigits

`func (o *SmsReceipt) SetDigits(v int32)`

SetDigits sets Digits field to given value.

### HasDigits

`func (o *SmsReceipt) HasDigits() bool`

HasDigits returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


