# SendSms

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**HttpCode** | Pointer to **int32** | The HTTP code of the response. Visit [this page](/#status-codes) for more information.  This parameter doesn’t reflect the status of each message. Check the status parameter of the message object to view the status of the individual message. | [optional] 
**ResponseCode** | Pointer to **string** | The response code of the operation. Visit [this page](/#status-codes) for more information. | [optional] 
**ResponseMsg** | Pointer to **string** | A message describing the outcome of the operation. | [optional] 
**Data** | Pointer to [**SendSmsData**](SendSmsData.md) |  | [optional] 

## Methods

### NewSendSms

`func NewSendSms() *SendSms`

NewSendSms instantiates a new SendSms object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewSendSmsWithDefaults

`func NewSendSmsWithDefaults() *SendSms`

NewSendSmsWithDefaults instantiates a new SendSms object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetHttpCode

`func (o *SendSms) GetHttpCode() int32`

GetHttpCode returns the HttpCode field if non-nil, zero value otherwise.

### GetHttpCodeOk

`func (o *SendSms) GetHttpCodeOk() (*int32, bool)`

GetHttpCodeOk returns a tuple with the HttpCode field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetHttpCode

`func (o *SendSms) SetHttpCode(v int32)`

SetHttpCode sets HttpCode field to given value.

### HasHttpCode

`func (o *SendSms) HasHttpCode() bool`

HasHttpCode returns a boolean if a field has been set.

### GetResponseCode

`func (o *SendSms) GetResponseCode() string`

GetResponseCode returns the ResponseCode field if non-nil, zero value otherwise.

### GetResponseCodeOk

`func (o *SendSms) GetResponseCodeOk() (*string, bool)`

GetResponseCodeOk returns a tuple with the ResponseCode field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetResponseCode

`func (o *SendSms) SetResponseCode(v string)`

SetResponseCode sets ResponseCode field to given value.

### HasResponseCode

`func (o *SendSms) HasResponseCode() bool`

HasResponseCode returns a boolean if a field has been set.

### GetResponseMsg

`func (o *SendSms) GetResponseMsg() string`

GetResponseMsg returns the ResponseMsg field if non-nil, zero value otherwise.

### GetResponseMsgOk

`func (o *SendSms) GetResponseMsgOk() (*string, bool)`

GetResponseMsgOk returns a tuple with the ResponseMsg field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetResponseMsg

`func (o *SendSms) SetResponseMsg(v string)`

SetResponseMsg sets ResponseMsg field to given value.

### HasResponseMsg

`func (o *SendSms) HasResponseMsg() bool`

HasResponseMsg returns a boolean if a field has been set.

### GetData

`func (o *SendSms) GetData() SendSmsData`

GetData returns the Data field if non-nil, zero value otherwise.

### GetDataOk

`func (o *SendSms) GetDataOk() (*SendSmsData, bool)`

GetDataOk returns a tuple with the Data field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetData

`func (o *SendSms) SetData(v SendSmsData)`

SetData sets Data field to given value.

### HasData

`func (o *SendSms) HasData() bool`

HasData returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


