# MarkSpecificInboundSmsMessageAsRead

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**HttpCode** | Pointer to **int32** | The HTTP code of the response. Visit [this page](/#status-codes) for more information. | [optional] 
**ResponseCode** | Pointer to **string** | The response code of the operation. Visit [this page](/#status-codes) for more information. | [optional] 
**ResponseMsg** | Pointer to **string** | A message describing the outcome of the operation. | [optional] 
**Data** | Pointer to **int32** | The number of SMS marked as read.  If you have multiple inbound rules set to POLL, you will receive the inbound message multiple times. Reading it will mark all those messages as read. | [optional] 

## Methods

### NewMarkSpecificInboundSmsMessageAsRead

`func NewMarkSpecificInboundSmsMessageAsRead() *MarkSpecificInboundSmsMessageAsRead`

NewMarkSpecificInboundSmsMessageAsRead instantiates a new MarkSpecificInboundSmsMessageAsRead object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewMarkSpecificInboundSmsMessageAsReadWithDefaults

`func NewMarkSpecificInboundSmsMessageAsReadWithDefaults() *MarkSpecificInboundSmsMessageAsRead`

NewMarkSpecificInboundSmsMessageAsReadWithDefaults instantiates a new MarkSpecificInboundSmsMessageAsRead object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetHttpCode

`func (o *MarkSpecificInboundSmsMessageAsRead) GetHttpCode() int32`

GetHttpCode returns the HttpCode field if non-nil, zero value otherwise.

### GetHttpCodeOk

`func (o *MarkSpecificInboundSmsMessageAsRead) GetHttpCodeOk() (*int32, bool)`

GetHttpCodeOk returns a tuple with the HttpCode field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetHttpCode

`func (o *MarkSpecificInboundSmsMessageAsRead) SetHttpCode(v int32)`

SetHttpCode sets HttpCode field to given value.

### HasHttpCode

`func (o *MarkSpecificInboundSmsMessageAsRead) HasHttpCode() bool`

HasHttpCode returns a boolean if a field has been set.

### GetResponseCode

`func (o *MarkSpecificInboundSmsMessageAsRead) GetResponseCode() string`

GetResponseCode returns the ResponseCode field if non-nil, zero value otherwise.

### GetResponseCodeOk

`func (o *MarkSpecificInboundSmsMessageAsRead) GetResponseCodeOk() (*string, bool)`

GetResponseCodeOk returns a tuple with the ResponseCode field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetResponseCode

`func (o *MarkSpecificInboundSmsMessageAsRead) SetResponseCode(v string)`

SetResponseCode sets ResponseCode field to given value.

### HasResponseCode

`func (o *MarkSpecificInboundSmsMessageAsRead) HasResponseCode() bool`

HasResponseCode returns a boolean if a field has been set.

### GetResponseMsg

`func (o *MarkSpecificInboundSmsMessageAsRead) GetResponseMsg() string`

GetResponseMsg returns the ResponseMsg field if non-nil, zero value otherwise.

### GetResponseMsgOk

`func (o *MarkSpecificInboundSmsMessageAsRead) GetResponseMsgOk() (*string, bool)`

GetResponseMsgOk returns a tuple with the ResponseMsg field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetResponseMsg

`func (o *MarkSpecificInboundSmsMessageAsRead) SetResponseMsg(v string)`

SetResponseMsg sets ResponseMsg field to given value.

### HasResponseMsg

`func (o *MarkSpecificInboundSmsMessageAsRead) HasResponseMsg() bool`

HasResponseMsg returns a boolean if a field has been set.

### GetData

`func (o *MarkSpecificInboundSmsMessageAsRead) GetData() int32`

GetData returns the Data field if non-nil, zero value otherwise.

### GetDataOk

`func (o *MarkSpecificInboundSmsMessageAsRead) GetDataOk() (*int32, bool)`

GetDataOk returns a tuple with the Data field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetData

`func (o *MarkSpecificInboundSmsMessageAsRead) SetData(v int32)`

SetData sets Data field to given value.

### HasData

`func (o *MarkSpecificInboundSmsMessageAsRead) HasData() bool`

HasData returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


