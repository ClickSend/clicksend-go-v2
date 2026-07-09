# DeleteSmsTemplate

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**HttpCode** | Pointer to **int32** | The HTTP code of the response. Visit [this page](/#status-codes) for more information | [optional] 
**ResponseCode** | Pointer to **string** | The response code of the operation. Visit [this page](/#status-codes) for more information. | [optional] 
**ResponseMsg** | Pointer to **string** | A message describing the outcome of the operation. | [optional] 
**Data** | Pointer to **[]string** | The parameters related to the SMS template.  &lt;div class&#x3D;\&quot;warning-box\&quot;&gt;   &lt;h4&gt;&lt;i class&#x3D;\&quot;fas fa-exclamation-triangle\&quot;&gt;&lt;/i&gt; Warning:&lt;/h4&gt;   &lt;p&gt;This parameter is deprecated and will return &lt;strong&gt;null&lt;/strong&gt;.&lt;/p&gt; &lt;/div&gt; | [optional] 

## Methods

### NewDeleteSmsTemplate

`func NewDeleteSmsTemplate() *DeleteSmsTemplate`

NewDeleteSmsTemplate instantiates a new DeleteSmsTemplate object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewDeleteSmsTemplateWithDefaults

`func NewDeleteSmsTemplateWithDefaults() *DeleteSmsTemplate`

NewDeleteSmsTemplateWithDefaults instantiates a new DeleteSmsTemplate object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetHttpCode

`func (o *DeleteSmsTemplate) GetHttpCode() int32`

GetHttpCode returns the HttpCode field if non-nil, zero value otherwise.

### GetHttpCodeOk

`func (o *DeleteSmsTemplate) GetHttpCodeOk() (*int32, bool)`

GetHttpCodeOk returns a tuple with the HttpCode field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetHttpCode

`func (o *DeleteSmsTemplate) SetHttpCode(v int32)`

SetHttpCode sets HttpCode field to given value.

### HasHttpCode

`func (o *DeleteSmsTemplate) HasHttpCode() bool`

HasHttpCode returns a boolean if a field has been set.

### GetResponseCode

`func (o *DeleteSmsTemplate) GetResponseCode() string`

GetResponseCode returns the ResponseCode field if non-nil, zero value otherwise.

### GetResponseCodeOk

`func (o *DeleteSmsTemplate) GetResponseCodeOk() (*string, bool)`

GetResponseCodeOk returns a tuple with the ResponseCode field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetResponseCode

`func (o *DeleteSmsTemplate) SetResponseCode(v string)`

SetResponseCode sets ResponseCode field to given value.

### HasResponseCode

`func (o *DeleteSmsTemplate) HasResponseCode() bool`

HasResponseCode returns a boolean if a field has been set.

### GetResponseMsg

`func (o *DeleteSmsTemplate) GetResponseMsg() string`

GetResponseMsg returns the ResponseMsg field if non-nil, zero value otherwise.

### GetResponseMsgOk

`func (o *DeleteSmsTemplate) GetResponseMsgOk() (*string, bool)`

GetResponseMsgOk returns a tuple with the ResponseMsg field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetResponseMsg

`func (o *DeleteSmsTemplate) SetResponseMsg(v string)`

SetResponseMsg sets ResponseMsg field to given value.

### HasResponseMsg

`func (o *DeleteSmsTemplate) HasResponseMsg() bool`

HasResponseMsg returns a boolean if a field has been set.

### GetData

`func (o *DeleteSmsTemplate) GetData() []string`

GetData returns the Data field if non-nil, zero value otherwise.

### GetDataOk

`func (o *DeleteSmsTemplate) GetDataOk() (*[]string, bool)`

GetDataOk returns a tuple with the Data field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetData

`func (o *DeleteSmsTemplate) SetData(v []string)`

SetData sets Data field to given value.

### HasData

`func (o *DeleteSmsTemplate) HasData() bool`

HasData returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


