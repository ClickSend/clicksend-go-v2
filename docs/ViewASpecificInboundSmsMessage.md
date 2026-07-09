# ViewASpecificInboundSmsMessage

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**HttpCode** | Pointer to **int32** | The HTTP code of the response. Visit [this page](/#status-codes) for more information. | [optional] 
**ResponseCode** | Pointer to **string** | The response code of the operation. Visit [this page](/#status-codes) for more information. | [optional] 
**ResponseMsg** | Pointer to **string** | A message describing the outcome of the operation. | [optional] 
**Data** | Pointer to [**InboundSms**](InboundSms.md) |  | [optional] 

## Methods

### NewViewASpecificInboundSmsMessage

`func NewViewASpecificInboundSmsMessage() *ViewASpecificInboundSmsMessage`

NewViewASpecificInboundSmsMessage instantiates a new ViewASpecificInboundSmsMessage object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewViewASpecificInboundSmsMessageWithDefaults

`func NewViewASpecificInboundSmsMessageWithDefaults() *ViewASpecificInboundSmsMessage`

NewViewASpecificInboundSmsMessageWithDefaults instantiates a new ViewASpecificInboundSmsMessage object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetHttpCode

`func (o *ViewASpecificInboundSmsMessage) GetHttpCode() int32`

GetHttpCode returns the HttpCode field if non-nil, zero value otherwise.

### GetHttpCodeOk

`func (o *ViewASpecificInboundSmsMessage) GetHttpCodeOk() (*int32, bool)`

GetHttpCodeOk returns a tuple with the HttpCode field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetHttpCode

`func (o *ViewASpecificInboundSmsMessage) SetHttpCode(v int32)`

SetHttpCode sets HttpCode field to given value.

### HasHttpCode

`func (o *ViewASpecificInboundSmsMessage) HasHttpCode() bool`

HasHttpCode returns a boolean if a field has been set.

### GetResponseCode

`func (o *ViewASpecificInboundSmsMessage) GetResponseCode() string`

GetResponseCode returns the ResponseCode field if non-nil, zero value otherwise.

### GetResponseCodeOk

`func (o *ViewASpecificInboundSmsMessage) GetResponseCodeOk() (*string, bool)`

GetResponseCodeOk returns a tuple with the ResponseCode field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetResponseCode

`func (o *ViewASpecificInboundSmsMessage) SetResponseCode(v string)`

SetResponseCode sets ResponseCode field to given value.

### HasResponseCode

`func (o *ViewASpecificInboundSmsMessage) HasResponseCode() bool`

HasResponseCode returns a boolean if a field has been set.

### GetResponseMsg

`func (o *ViewASpecificInboundSmsMessage) GetResponseMsg() string`

GetResponseMsg returns the ResponseMsg field if non-nil, zero value otherwise.

### GetResponseMsgOk

`func (o *ViewASpecificInboundSmsMessage) GetResponseMsgOk() (*string, bool)`

GetResponseMsgOk returns a tuple with the ResponseMsg field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetResponseMsg

`func (o *ViewASpecificInboundSmsMessage) SetResponseMsg(v string)`

SetResponseMsg sets ResponseMsg field to given value.

### HasResponseMsg

`func (o *ViewASpecificInboundSmsMessage) HasResponseMsg() bool`

HasResponseMsg returns a boolean if a field has been set.

### GetData

`func (o *ViewASpecificInboundSmsMessage) GetData() InboundSms`

GetData returns the Data field if non-nil, zero value otherwise.

### GetDataOk

`func (o *ViewASpecificInboundSmsMessage) GetDataOk() (*InboundSms, bool)`

GetDataOk returns a tuple with the Data field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetData

`func (o *ViewASpecificInboundSmsMessage) SetData(v InboundSms)`

SetData sets Data field to given value.

### HasData

`func (o *ViewASpecificInboundSmsMessage) HasData() bool`

HasData returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


