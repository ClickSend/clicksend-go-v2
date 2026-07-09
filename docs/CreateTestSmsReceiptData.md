# CreateTestSmsReceiptData

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**TimestampSend** | Pointer to **int32** | The time you sent the test message. It is in &lt;a target&#x3D;\&quot;_blank\&quot; href&#x3D;\&quot;http://help.clicksend.com/what-is-a-unix-timestamp\&quot;&gt;Unix format.&lt;/a&gt; | [optional] 
**Timestamp** | Pointer to **int32** | The time you receive the test message receipt. It is in &lt;a target&#x3D;\&quot;_blank\&quot; href&#x3D;\&quot;http://help.clicksend.com/what-is-a-unix-timestamp\&quot;&gt;Unix format.&lt;/a&gt; | [optional] 
**MessageId** | Pointer to **string** | The generated ID of the message. This ID is typically used as a reference for &lt;a target&#x3D;\&quot;_blank\&quot; href&#x3D;\&quot;https://www.clicksend.com/au/help/\&quot;&gt;customer support&lt;/a&gt; in case of any issues.  &lt;div class&#x3D;\&quot;info-box\&quot;&gt;   &lt;h4&gt;&lt;i class&#x3D;\&quot;fas fa-info-circle\&quot;&gt;&lt;/i&gt; Note:&lt;/h4&gt;   &lt;p&gt;This &lt;em&gt;message_id&lt;/em&gt; is different from the ID that is generated when sending or receving an actual SMS. This ID is used for testing only.&lt;/p&gt; &lt;/div&gt; | [optional] 
**StatusCode** | Pointer to **int32** | The status code that is sent from the &lt;a target&#x3D;\&quot;_blank\&quot; href&#x3D;\&quot;https://en.wikipedia.org/wiki/SMS_gateway\&quot;&gt;SMS gateway.&lt;/a&gt; Visit &lt;a target&#x3D;\&quot;_blank\&quot; href&#x3D;\&quot;https://help.clicksend.com/article/8cc479qlbb-list-of-sms-gateway-error-codes\&quot;&gt;this page&lt;/a&gt; for more information. | [optional] 
**StatusText** | Pointer to **string** | A message describing the _status_code_ of the operation. Visit &lt;a target&#x3D;\&quot;_blank\&quot; href&#x3D;\&quot;https://help.clicksend.com/article/8cc479qlbb-list-of-sms-gateway-error-codes\&quot;&gt;this&lt;/a&gt; page for more information. | [optional] 
**ErrorCode** | Pointer to **NullableInt32** | The error code of the operation. Visit &lt;a target&#x3D;\&quot;_blank\&quot; href&#x3D;\&quot;https://help.clicksend.com/article/8cc479qlbb-list-of-sms-gateway-error-codes\&quot;&gt;this page&lt;/a&gt; for more information. If no error occurred, the value is **null**. | [optional] 
**ErrorText** | Pointer to **NullableString** | A message describing the _error_code_ of the operation. Visit &lt;a target&#x3D;\&quot;_blank\&quot; href&#x3D;\&quot;https://help.clicksend.com/article/8cc479qlbb-list-of-sms-gateway-error-codes\&quot;&gt;this page&lt;/a&gt; for more information. If no error occurred, the value is **null**. | [optional] 
**CustomString** | Pointer to **NullableString** | A note that was sent from the request.  &lt;div class&#x3D;\&quot;warning-box\&quot;&gt;   &lt;h4&gt;&lt;i class&#x3D;\&quot;fas fa-exclamation-triangle\&quot;&gt;&lt;/i&gt; Warning:&lt;/h4&gt;   &lt;p&gt;This parameter is deprecated and will return &lt;strong&gt;null.&lt;/strong&gt;&lt;/p&gt; &lt;/div&gt; | [optional] 
**SubaccountId** | Pointer to **int32** | The sub-account of the user. A user can have multiple sub-accounts. | [optional] 
**MessageType** | Pointer to **string** | The type of message (e.g. SMS, MMS, etc). | [optional] 
**Digits** | Pointer to **NullableInt32** | The numbers that the recipient pressed on their keypad during the call. A **null** value is returned if the recipient didn&#39;t provide any input.  &lt;div class&#x3D;\&quot;info-box\&quot;&gt;   &lt;h4&gt;&lt;i class&#x3D;\&quot;fas fa-info-circle\&quot;&gt;&lt;/i&gt; Note:&lt;/h4&gt;   &lt;p&gt;This parameter is only relevant to &lt;a href&#x3D;\&quot;/messaging/voice-messaging/\&quot;&gt;&lt;strong&gt;Voice Messaging&lt;/strong&gt;&lt;/a&gt; receipts.&lt;/p&gt; &lt;/div&gt; | [optional] 

## Methods

### NewCreateTestSmsReceiptData

`func NewCreateTestSmsReceiptData() *CreateTestSmsReceiptData`

NewCreateTestSmsReceiptData instantiates a new CreateTestSmsReceiptData object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewCreateTestSmsReceiptDataWithDefaults

`func NewCreateTestSmsReceiptDataWithDefaults() *CreateTestSmsReceiptData`

NewCreateTestSmsReceiptDataWithDefaults instantiates a new CreateTestSmsReceiptData object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetTimestampSend

`func (o *CreateTestSmsReceiptData) GetTimestampSend() int32`

GetTimestampSend returns the TimestampSend field if non-nil, zero value otherwise.

### GetTimestampSendOk

`func (o *CreateTestSmsReceiptData) GetTimestampSendOk() (*int32, bool)`

GetTimestampSendOk returns a tuple with the TimestampSend field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTimestampSend

`func (o *CreateTestSmsReceiptData) SetTimestampSend(v int32)`

SetTimestampSend sets TimestampSend field to given value.

### HasTimestampSend

`func (o *CreateTestSmsReceiptData) HasTimestampSend() bool`

HasTimestampSend returns a boolean if a field has been set.

### GetTimestamp

`func (o *CreateTestSmsReceiptData) GetTimestamp() int32`

GetTimestamp returns the Timestamp field if non-nil, zero value otherwise.

### GetTimestampOk

`func (o *CreateTestSmsReceiptData) GetTimestampOk() (*int32, bool)`

GetTimestampOk returns a tuple with the Timestamp field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTimestamp

`func (o *CreateTestSmsReceiptData) SetTimestamp(v int32)`

SetTimestamp sets Timestamp field to given value.

### HasTimestamp

`func (o *CreateTestSmsReceiptData) HasTimestamp() bool`

HasTimestamp returns a boolean if a field has been set.

### GetMessageId

`func (o *CreateTestSmsReceiptData) GetMessageId() string`

GetMessageId returns the MessageId field if non-nil, zero value otherwise.

### GetMessageIdOk

`func (o *CreateTestSmsReceiptData) GetMessageIdOk() (*string, bool)`

GetMessageIdOk returns a tuple with the MessageId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetMessageId

`func (o *CreateTestSmsReceiptData) SetMessageId(v string)`

SetMessageId sets MessageId field to given value.

### HasMessageId

`func (o *CreateTestSmsReceiptData) HasMessageId() bool`

HasMessageId returns a boolean if a field has been set.

### GetStatusCode

`func (o *CreateTestSmsReceiptData) GetStatusCode() int32`

GetStatusCode returns the StatusCode field if non-nil, zero value otherwise.

### GetStatusCodeOk

`func (o *CreateTestSmsReceiptData) GetStatusCodeOk() (*int32, bool)`

GetStatusCodeOk returns a tuple with the StatusCode field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetStatusCode

`func (o *CreateTestSmsReceiptData) SetStatusCode(v int32)`

SetStatusCode sets StatusCode field to given value.

### HasStatusCode

`func (o *CreateTestSmsReceiptData) HasStatusCode() bool`

HasStatusCode returns a boolean if a field has been set.

### GetStatusText

`func (o *CreateTestSmsReceiptData) GetStatusText() string`

GetStatusText returns the StatusText field if non-nil, zero value otherwise.

### GetStatusTextOk

`func (o *CreateTestSmsReceiptData) GetStatusTextOk() (*string, bool)`

GetStatusTextOk returns a tuple with the StatusText field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetStatusText

`func (o *CreateTestSmsReceiptData) SetStatusText(v string)`

SetStatusText sets StatusText field to given value.

### HasStatusText

`func (o *CreateTestSmsReceiptData) HasStatusText() bool`

HasStatusText returns a boolean if a field has been set.

### GetErrorCode

`func (o *CreateTestSmsReceiptData) GetErrorCode() int32`

GetErrorCode returns the ErrorCode field if non-nil, zero value otherwise.

### GetErrorCodeOk

`func (o *CreateTestSmsReceiptData) GetErrorCodeOk() (*int32, bool)`

GetErrorCodeOk returns a tuple with the ErrorCode field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetErrorCode

`func (o *CreateTestSmsReceiptData) SetErrorCode(v int32)`

SetErrorCode sets ErrorCode field to given value.

### HasErrorCode

`func (o *CreateTestSmsReceiptData) HasErrorCode() bool`

HasErrorCode returns a boolean if a field has been set.

### SetErrorCodeNil

`func (o *CreateTestSmsReceiptData) SetErrorCodeNil(b bool)`

 SetErrorCodeNil sets the value for ErrorCode to be an explicit nil

### UnsetErrorCode
`func (o *CreateTestSmsReceiptData) UnsetErrorCode()`

UnsetErrorCode ensures that no value is present for ErrorCode, not even an explicit nil
### GetErrorText

`func (o *CreateTestSmsReceiptData) GetErrorText() string`

GetErrorText returns the ErrorText field if non-nil, zero value otherwise.

### GetErrorTextOk

`func (o *CreateTestSmsReceiptData) GetErrorTextOk() (*string, bool)`

GetErrorTextOk returns a tuple with the ErrorText field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetErrorText

`func (o *CreateTestSmsReceiptData) SetErrorText(v string)`

SetErrorText sets ErrorText field to given value.

### HasErrorText

`func (o *CreateTestSmsReceiptData) HasErrorText() bool`

HasErrorText returns a boolean if a field has been set.

### SetErrorTextNil

`func (o *CreateTestSmsReceiptData) SetErrorTextNil(b bool)`

 SetErrorTextNil sets the value for ErrorText to be an explicit nil

### UnsetErrorText
`func (o *CreateTestSmsReceiptData) UnsetErrorText()`

UnsetErrorText ensures that no value is present for ErrorText, not even an explicit nil
### GetCustomString

`func (o *CreateTestSmsReceiptData) GetCustomString() string`

GetCustomString returns the CustomString field if non-nil, zero value otherwise.

### GetCustomStringOk

`func (o *CreateTestSmsReceiptData) GetCustomStringOk() (*string, bool)`

GetCustomStringOk returns a tuple with the CustomString field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCustomString

`func (o *CreateTestSmsReceiptData) SetCustomString(v string)`

SetCustomString sets CustomString field to given value.

### HasCustomString

`func (o *CreateTestSmsReceiptData) HasCustomString() bool`

HasCustomString returns a boolean if a field has been set.

### SetCustomStringNil

`func (o *CreateTestSmsReceiptData) SetCustomStringNil(b bool)`

 SetCustomStringNil sets the value for CustomString to be an explicit nil

### UnsetCustomString
`func (o *CreateTestSmsReceiptData) UnsetCustomString()`

UnsetCustomString ensures that no value is present for CustomString, not even an explicit nil
### GetSubaccountId

`func (o *CreateTestSmsReceiptData) GetSubaccountId() int32`

GetSubaccountId returns the SubaccountId field if non-nil, zero value otherwise.

### GetSubaccountIdOk

`func (o *CreateTestSmsReceiptData) GetSubaccountIdOk() (*int32, bool)`

GetSubaccountIdOk returns a tuple with the SubaccountId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSubaccountId

`func (o *CreateTestSmsReceiptData) SetSubaccountId(v int32)`

SetSubaccountId sets SubaccountId field to given value.

### HasSubaccountId

`func (o *CreateTestSmsReceiptData) HasSubaccountId() bool`

HasSubaccountId returns a boolean if a field has been set.

### GetMessageType

`func (o *CreateTestSmsReceiptData) GetMessageType() string`

GetMessageType returns the MessageType field if non-nil, zero value otherwise.

### GetMessageTypeOk

`func (o *CreateTestSmsReceiptData) GetMessageTypeOk() (*string, bool)`

GetMessageTypeOk returns a tuple with the MessageType field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetMessageType

`func (o *CreateTestSmsReceiptData) SetMessageType(v string)`

SetMessageType sets MessageType field to given value.

### HasMessageType

`func (o *CreateTestSmsReceiptData) HasMessageType() bool`

HasMessageType returns a boolean if a field has been set.

### GetDigits

`func (o *CreateTestSmsReceiptData) GetDigits() int32`

GetDigits returns the Digits field if non-nil, zero value otherwise.

### GetDigitsOk

`func (o *CreateTestSmsReceiptData) GetDigitsOk() (*int32, bool)`

GetDigitsOk returns a tuple with the Digits field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDigits

`func (o *CreateTestSmsReceiptData) SetDigits(v int32)`

SetDigits sets Digits field to given value.

### HasDigits

`func (o *CreateTestSmsReceiptData) HasDigits() bool`

HasDigits returns a boolean if a field has been set.

### SetDigitsNil

`func (o *CreateTestSmsReceiptData) SetDigitsNil(b bool)`

 SetDigitsNil sets the value for Digits to be an explicit nil

### UnsetDigits
`func (o *CreateTestSmsReceiptData) UnsetDigits()`

UnsetDigits ensures that no value is present for Digits, not even an explicit nil

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


