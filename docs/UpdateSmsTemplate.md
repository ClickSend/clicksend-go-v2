# UpdateSmsTemplate

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**HttpCode** | Pointer to **string** | The HTTP code of the response. Visit [this page](/#status-codes) for more information. | [optional] 
**ResponseCode** | Pointer to **string** | The response code of the operation. Visit [this page](/#status-codes) for more information. | [optional] 
**ResponseMsg** | Pointer to **string** | A message describing the outcome of the operation. | [optional] 
**Data** | Pointer to [**SmsTemplateUpdate**](SmsTemplateUpdate.md) |  | [optional] 

## Methods

### NewUpdateSmsTemplate

`func NewUpdateSmsTemplate() *UpdateSmsTemplate`

NewUpdateSmsTemplate instantiates a new UpdateSmsTemplate object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewUpdateSmsTemplateWithDefaults

`func NewUpdateSmsTemplateWithDefaults() *UpdateSmsTemplate`

NewUpdateSmsTemplateWithDefaults instantiates a new UpdateSmsTemplate object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetHttpCode

`func (o *UpdateSmsTemplate) GetHttpCode() string`

GetHttpCode returns the HttpCode field if non-nil, zero value otherwise.

### GetHttpCodeOk

`func (o *UpdateSmsTemplate) GetHttpCodeOk() (*string, bool)`

GetHttpCodeOk returns a tuple with the HttpCode field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetHttpCode

`func (o *UpdateSmsTemplate) SetHttpCode(v string)`

SetHttpCode sets HttpCode field to given value.

### HasHttpCode

`func (o *UpdateSmsTemplate) HasHttpCode() bool`

HasHttpCode returns a boolean if a field has been set.

### GetResponseCode

`func (o *UpdateSmsTemplate) GetResponseCode() string`

GetResponseCode returns the ResponseCode field if non-nil, zero value otherwise.

### GetResponseCodeOk

`func (o *UpdateSmsTemplate) GetResponseCodeOk() (*string, bool)`

GetResponseCodeOk returns a tuple with the ResponseCode field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetResponseCode

`func (o *UpdateSmsTemplate) SetResponseCode(v string)`

SetResponseCode sets ResponseCode field to given value.

### HasResponseCode

`func (o *UpdateSmsTemplate) HasResponseCode() bool`

HasResponseCode returns a boolean if a field has been set.

### GetResponseMsg

`func (o *UpdateSmsTemplate) GetResponseMsg() string`

GetResponseMsg returns the ResponseMsg field if non-nil, zero value otherwise.

### GetResponseMsgOk

`func (o *UpdateSmsTemplate) GetResponseMsgOk() (*string, bool)`

GetResponseMsgOk returns a tuple with the ResponseMsg field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetResponseMsg

`func (o *UpdateSmsTemplate) SetResponseMsg(v string)`

SetResponseMsg sets ResponseMsg field to given value.

### HasResponseMsg

`func (o *UpdateSmsTemplate) HasResponseMsg() bool`

HasResponseMsg returns a boolean if a field has been set.

### GetData

`func (o *UpdateSmsTemplate) GetData() SmsTemplateUpdate`

GetData returns the Data field if non-nil, zero value otherwise.

### GetDataOk

`func (o *UpdateSmsTemplate) GetDataOk() (*SmsTemplateUpdate, bool)`

GetDataOk returns a tuple with the Data field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetData

`func (o *UpdateSmsTemplate) SetData(v SmsTemplateUpdate)`

SetData sets Data field to given value.

### HasData

`func (o *UpdateSmsTemplate) HasData() bool`

HasData returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


