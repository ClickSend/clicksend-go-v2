# MarkSmsReceiptAsReadRequest

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**DateBefore** | Pointer to **int32** | The cutoff date. Receipts sent before this time will be marked as read. It’s in the &lt;a target&#x3D;\&quot;_blank\&quot; href&#x3D;\&quot;http://help.clicksend.com/what-is-a-unix-timestamp\&quot;&gt;Unix format&lt;/a&gt;. | [optional] 

## Methods

### NewMarkSmsReceiptAsReadRequest

`func NewMarkSmsReceiptAsReadRequest() *MarkSmsReceiptAsReadRequest`

NewMarkSmsReceiptAsReadRequest instantiates a new MarkSmsReceiptAsReadRequest object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewMarkSmsReceiptAsReadRequestWithDefaults

`func NewMarkSmsReceiptAsReadRequestWithDefaults() *MarkSmsReceiptAsReadRequest`

NewMarkSmsReceiptAsReadRequestWithDefaults instantiates a new MarkSmsReceiptAsReadRequest object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetDateBefore

`func (o *MarkSmsReceiptAsReadRequest) GetDateBefore() int32`

GetDateBefore returns the DateBefore field if non-nil, zero value otherwise.

### GetDateBeforeOk

`func (o *MarkSmsReceiptAsReadRequest) GetDateBeforeOk() (*int32, bool)`

GetDateBeforeOk returns a tuple with the DateBefore field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDateBefore

`func (o *MarkSmsReceiptAsReadRequest) SetDateBefore(v int32)`

SetDateBefore sets DateBefore field to given value.

### HasDateBefore

`func (o *MarkSmsReceiptAsReadRequest) HasDateBefore() bool`

HasDateBefore returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


