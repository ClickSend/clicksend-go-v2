# VoiceReceipt

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**TimestampSend** | Pointer to **string** | Timestamp of the original send request in UNIX format. e.g 1439173980 | [optional] 
**Timestamp** | Pointer to **string** | Timestamp of delivery report in UNIX format. e.g 1439173981 | [optional] 
**MessageId** | Pointer to **string** | Message ID, returned when originally sending the message. | [optional] 
**StatusCode** | Pointer to **string** | Status code. Refer to &#39;Voice Delivery Status Codes&#39; in docs. | [optional] 
**StatusText** | Pointer to **string** | Status text. | [optional] 
**ErrorCode** | Pointer to **NullableString** | Error code. | [optional] 
**ErrorText** | Pointer to **NullableString** | Error text. | [optional] 
**CustomString** | Pointer to **NullableString** | A custom string used when sending the original message. | [optional] 
**MessageType** | Pointer to **string** | voice (constant). | [optional] 
**Digits** | Pointer to **string** | Numbers the recipient pressed on their keypad during the call. A blank string will be used if they didn&#39;t provide any input. | [optional] 

## Methods

### NewVoiceReceipt

`func NewVoiceReceipt() *VoiceReceipt`

NewVoiceReceipt instantiates a new VoiceReceipt object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewVoiceReceiptWithDefaults

`func NewVoiceReceiptWithDefaults() *VoiceReceipt`

NewVoiceReceiptWithDefaults instantiates a new VoiceReceipt object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetTimestampSend

`func (o *VoiceReceipt) GetTimestampSend() string`

GetTimestampSend returns the TimestampSend field if non-nil, zero value otherwise.

### GetTimestampSendOk

`func (o *VoiceReceipt) GetTimestampSendOk() (*string, bool)`

GetTimestampSendOk returns a tuple with the TimestampSend field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTimestampSend

`func (o *VoiceReceipt) SetTimestampSend(v string)`

SetTimestampSend sets TimestampSend field to given value.

### HasTimestampSend

`func (o *VoiceReceipt) HasTimestampSend() bool`

HasTimestampSend returns a boolean if a field has been set.

### GetTimestamp

`func (o *VoiceReceipt) GetTimestamp() string`

GetTimestamp returns the Timestamp field if non-nil, zero value otherwise.

### GetTimestampOk

`func (o *VoiceReceipt) GetTimestampOk() (*string, bool)`

GetTimestampOk returns a tuple with the Timestamp field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTimestamp

`func (o *VoiceReceipt) SetTimestamp(v string)`

SetTimestamp sets Timestamp field to given value.

### HasTimestamp

`func (o *VoiceReceipt) HasTimestamp() bool`

HasTimestamp returns a boolean if a field has been set.

### GetMessageId

`func (o *VoiceReceipt) GetMessageId() string`

GetMessageId returns the MessageId field if non-nil, zero value otherwise.

### GetMessageIdOk

`func (o *VoiceReceipt) GetMessageIdOk() (*string, bool)`

GetMessageIdOk returns a tuple with the MessageId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetMessageId

`func (o *VoiceReceipt) SetMessageId(v string)`

SetMessageId sets MessageId field to given value.

### HasMessageId

`func (o *VoiceReceipt) HasMessageId() bool`

HasMessageId returns a boolean if a field has been set.

### GetStatusCode

`func (o *VoiceReceipt) GetStatusCode() string`

GetStatusCode returns the StatusCode field if non-nil, zero value otherwise.

### GetStatusCodeOk

`func (o *VoiceReceipt) GetStatusCodeOk() (*string, bool)`

GetStatusCodeOk returns a tuple with the StatusCode field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetStatusCode

`func (o *VoiceReceipt) SetStatusCode(v string)`

SetStatusCode sets StatusCode field to given value.

### HasStatusCode

`func (o *VoiceReceipt) HasStatusCode() bool`

HasStatusCode returns a boolean if a field has been set.

### GetStatusText

`func (o *VoiceReceipt) GetStatusText() string`

GetStatusText returns the StatusText field if non-nil, zero value otherwise.

### GetStatusTextOk

`func (o *VoiceReceipt) GetStatusTextOk() (*string, bool)`

GetStatusTextOk returns a tuple with the StatusText field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetStatusText

`func (o *VoiceReceipt) SetStatusText(v string)`

SetStatusText sets StatusText field to given value.

### HasStatusText

`func (o *VoiceReceipt) HasStatusText() bool`

HasStatusText returns a boolean if a field has been set.

### GetErrorCode

`func (o *VoiceReceipt) GetErrorCode() string`

GetErrorCode returns the ErrorCode field if non-nil, zero value otherwise.

### GetErrorCodeOk

`func (o *VoiceReceipt) GetErrorCodeOk() (*string, bool)`

GetErrorCodeOk returns a tuple with the ErrorCode field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetErrorCode

`func (o *VoiceReceipt) SetErrorCode(v string)`

SetErrorCode sets ErrorCode field to given value.

### HasErrorCode

`func (o *VoiceReceipt) HasErrorCode() bool`

HasErrorCode returns a boolean if a field has been set.

### SetErrorCodeNil

`func (o *VoiceReceipt) SetErrorCodeNil(b bool)`

 SetErrorCodeNil sets the value for ErrorCode to be an explicit nil

### UnsetErrorCode
`func (o *VoiceReceipt) UnsetErrorCode()`

UnsetErrorCode ensures that no value is present for ErrorCode, not even an explicit nil
### GetErrorText

`func (o *VoiceReceipt) GetErrorText() string`

GetErrorText returns the ErrorText field if non-nil, zero value otherwise.

### GetErrorTextOk

`func (o *VoiceReceipt) GetErrorTextOk() (*string, bool)`

GetErrorTextOk returns a tuple with the ErrorText field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetErrorText

`func (o *VoiceReceipt) SetErrorText(v string)`

SetErrorText sets ErrorText field to given value.

### HasErrorText

`func (o *VoiceReceipt) HasErrorText() bool`

HasErrorText returns a boolean if a field has been set.

### SetErrorTextNil

`func (o *VoiceReceipt) SetErrorTextNil(b bool)`

 SetErrorTextNil sets the value for ErrorText to be an explicit nil

### UnsetErrorText
`func (o *VoiceReceipt) UnsetErrorText()`

UnsetErrorText ensures that no value is present for ErrorText, not even an explicit nil
### GetCustomString

`func (o *VoiceReceipt) GetCustomString() string`

GetCustomString returns the CustomString field if non-nil, zero value otherwise.

### GetCustomStringOk

`func (o *VoiceReceipt) GetCustomStringOk() (*string, bool)`

GetCustomStringOk returns a tuple with the CustomString field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCustomString

`func (o *VoiceReceipt) SetCustomString(v string)`

SetCustomString sets CustomString field to given value.

### HasCustomString

`func (o *VoiceReceipt) HasCustomString() bool`

HasCustomString returns a boolean if a field has been set.

### SetCustomStringNil

`func (o *VoiceReceipt) SetCustomStringNil(b bool)`

 SetCustomStringNil sets the value for CustomString to be an explicit nil

### UnsetCustomString
`func (o *VoiceReceipt) UnsetCustomString()`

UnsetCustomString ensures that no value is present for CustomString, not even an explicit nil
### GetMessageType

`func (o *VoiceReceipt) GetMessageType() string`

GetMessageType returns the MessageType field if non-nil, zero value otherwise.

### GetMessageTypeOk

`func (o *VoiceReceipt) GetMessageTypeOk() (*string, bool)`

GetMessageTypeOk returns a tuple with the MessageType field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetMessageType

`func (o *VoiceReceipt) SetMessageType(v string)`

SetMessageType sets MessageType field to given value.

### HasMessageType

`func (o *VoiceReceipt) HasMessageType() bool`

HasMessageType returns a boolean if a field has been set.

### GetDigits

`func (o *VoiceReceipt) GetDigits() string`

GetDigits returns the Digits field if non-nil, zero value otherwise.

### GetDigitsOk

`func (o *VoiceReceipt) GetDigitsOk() (*string, bool)`

GetDigitsOk returns a tuple with the Digits field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDigits

`func (o *VoiceReceipt) SetDigits(v string)`

SetDigits sets Digits field to given value.

### HasDigits

`func (o *VoiceReceipt) HasDigits() bool`

HasDigits returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


