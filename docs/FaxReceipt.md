# FaxReceipt

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**TimestampSend** | Pointer to **string** | The timestamp when the message was sent. | [optional] 
**Timestamp** | Pointer to **string** | The timestamp associated with the message. | [optional] 
**MessageId** | Pointer to **string** | The ID of the message. | [optional] 
**StatusCode** | Pointer to **string** | The status code of the message. | [optional] 
**StatusText** | Pointer to **string** | The status text of the message. | [optional] 
**ErrorCode** | Pointer to **string** | The error code associated with the message. | [optional] 
**ErrorText** | Pointer to **string** | The error text associated with the message. | [optional] 
**CustomString** | Pointer to **string** | A custom string associated with the message. | [optional] 
**SubaccountId** | Pointer to **int32** | The ID of the subaccount. | [optional] 
**MessageType** | Pointer to **string** | The type of message. | [optional] 

## Methods

### NewFaxReceipt

`func NewFaxReceipt() *FaxReceipt`

NewFaxReceipt instantiates a new FaxReceipt object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewFaxReceiptWithDefaults

`func NewFaxReceiptWithDefaults() *FaxReceipt`

NewFaxReceiptWithDefaults instantiates a new FaxReceipt object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetTimestampSend

`func (o *FaxReceipt) GetTimestampSend() string`

GetTimestampSend returns the TimestampSend field if non-nil, zero value otherwise.

### GetTimestampSendOk

`func (o *FaxReceipt) GetTimestampSendOk() (*string, bool)`

GetTimestampSendOk returns a tuple with the TimestampSend field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTimestampSend

`func (o *FaxReceipt) SetTimestampSend(v string)`

SetTimestampSend sets TimestampSend field to given value.

### HasTimestampSend

`func (o *FaxReceipt) HasTimestampSend() bool`

HasTimestampSend returns a boolean if a field has been set.

### GetTimestamp

`func (o *FaxReceipt) GetTimestamp() string`

GetTimestamp returns the Timestamp field if non-nil, zero value otherwise.

### GetTimestampOk

`func (o *FaxReceipt) GetTimestampOk() (*string, bool)`

GetTimestampOk returns a tuple with the Timestamp field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTimestamp

`func (o *FaxReceipt) SetTimestamp(v string)`

SetTimestamp sets Timestamp field to given value.

### HasTimestamp

`func (o *FaxReceipt) HasTimestamp() bool`

HasTimestamp returns a boolean if a field has been set.

### GetMessageId

`func (o *FaxReceipt) GetMessageId() string`

GetMessageId returns the MessageId field if non-nil, zero value otherwise.

### GetMessageIdOk

`func (o *FaxReceipt) GetMessageIdOk() (*string, bool)`

GetMessageIdOk returns a tuple with the MessageId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetMessageId

`func (o *FaxReceipt) SetMessageId(v string)`

SetMessageId sets MessageId field to given value.

### HasMessageId

`func (o *FaxReceipt) HasMessageId() bool`

HasMessageId returns a boolean if a field has been set.

### GetStatusCode

`func (o *FaxReceipt) GetStatusCode() string`

GetStatusCode returns the StatusCode field if non-nil, zero value otherwise.

### GetStatusCodeOk

`func (o *FaxReceipt) GetStatusCodeOk() (*string, bool)`

GetStatusCodeOk returns a tuple with the StatusCode field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetStatusCode

`func (o *FaxReceipt) SetStatusCode(v string)`

SetStatusCode sets StatusCode field to given value.

### HasStatusCode

`func (o *FaxReceipt) HasStatusCode() bool`

HasStatusCode returns a boolean if a field has been set.

### GetStatusText

`func (o *FaxReceipt) GetStatusText() string`

GetStatusText returns the StatusText field if non-nil, zero value otherwise.

### GetStatusTextOk

`func (o *FaxReceipt) GetStatusTextOk() (*string, bool)`

GetStatusTextOk returns a tuple with the StatusText field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetStatusText

`func (o *FaxReceipt) SetStatusText(v string)`

SetStatusText sets StatusText field to given value.

### HasStatusText

`func (o *FaxReceipt) HasStatusText() bool`

HasStatusText returns a boolean if a field has been set.

### GetErrorCode

`func (o *FaxReceipt) GetErrorCode() string`

GetErrorCode returns the ErrorCode field if non-nil, zero value otherwise.

### GetErrorCodeOk

`func (o *FaxReceipt) GetErrorCodeOk() (*string, bool)`

GetErrorCodeOk returns a tuple with the ErrorCode field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetErrorCode

`func (o *FaxReceipt) SetErrorCode(v string)`

SetErrorCode sets ErrorCode field to given value.

### HasErrorCode

`func (o *FaxReceipt) HasErrorCode() bool`

HasErrorCode returns a boolean if a field has been set.

### GetErrorText

`func (o *FaxReceipt) GetErrorText() string`

GetErrorText returns the ErrorText field if non-nil, zero value otherwise.

### GetErrorTextOk

`func (o *FaxReceipt) GetErrorTextOk() (*string, bool)`

GetErrorTextOk returns a tuple with the ErrorText field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetErrorText

`func (o *FaxReceipt) SetErrorText(v string)`

SetErrorText sets ErrorText field to given value.

### HasErrorText

`func (o *FaxReceipt) HasErrorText() bool`

HasErrorText returns a boolean if a field has been set.

### GetCustomString

`func (o *FaxReceipt) GetCustomString() string`

GetCustomString returns the CustomString field if non-nil, zero value otherwise.

### GetCustomStringOk

`func (o *FaxReceipt) GetCustomStringOk() (*string, bool)`

GetCustomStringOk returns a tuple with the CustomString field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCustomString

`func (o *FaxReceipt) SetCustomString(v string)`

SetCustomString sets CustomString field to given value.

### HasCustomString

`func (o *FaxReceipt) HasCustomString() bool`

HasCustomString returns a boolean if a field has been set.

### GetSubaccountId

`func (o *FaxReceipt) GetSubaccountId() int32`

GetSubaccountId returns the SubaccountId field if non-nil, zero value otherwise.

### GetSubaccountIdOk

`func (o *FaxReceipt) GetSubaccountIdOk() (*int32, bool)`

GetSubaccountIdOk returns a tuple with the SubaccountId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSubaccountId

`func (o *FaxReceipt) SetSubaccountId(v int32)`

SetSubaccountId sets SubaccountId field to given value.

### HasSubaccountId

`func (o *FaxReceipt) HasSubaccountId() bool`

HasSubaccountId returns a boolean if a field has been set.

### GetMessageType

`func (o *FaxReceipt) GetMessageType() string`

GetMessageType returns the MessageType field if non-nil, zero value otherwise.

### GetMessageTypeOk

`func (o *FaxReceipt) GetMessageTypeOk() (*string, bool)`

GetMessageTypeOk returns a tuple with the MessageType field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetMessageType

`func (o *FaxReceipt) SetMessageType(v string)`

SetMessageType sets MessageType field to given value.

### HasMessageType

`func (o *FaxReceipt) HasMessageType() bool`

HasMessageType returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


