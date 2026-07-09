# ViewSmsInboundAutomations

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**HttpCode** | Pointer to **int32** | The HTTP status code of the response. | [optional] 
**ResponseCode** | Pointer to **string** | The response code indicating the status of the operation. | [optional] 
**ResponseMsg** | Pointer to **string** | A message describing the outcome of the operation. | [optional] 
**Data** | Pointer to [**ViewSmsInboundAutomationsData**](ViewSmsInboundAutomationsData.md) |  | [optional] 

## Methods

### NewViewSmsInboundAutomations

`func NewViewSmsInboundAutomations() *ViewSmsInboundAutomations`

NewViewSmsInboundAutomations instantiates a new ViewSmsInboundAutomations object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewViewSmsInboundAutomationsWithDefaults

`func NewViewSmsInboundAutomationsWithDefaults() *ViewSmsInboundAutomations`

NewViewSmsInboundAutomationsWithDefaults instantiates a new ViewSmsInboundAutomations object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetHttpCode

`func (o *ViewSmsInboundAutomations) GetHttpCode() int32`

GetHttpCode returns the HttpCode field if non-nil, zero value otherwise.

### GetHttpCodeOk

`func (o *ViewSmsInboundAutomations) GetHttpCodeOk() (*int32, bool)`

GetHttpCodeOk returns a tuple with the HttpCode field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetHttpCode

`func (o *ViewSmsInboundAutomations) SetHttpCode(v int32)`

SetHttpCode sets HttpCode field to given value.

### HasHttpCode

`func (o *ViewSmsInboundAutomations) HasHttpCode() bool`

HasHttpCode returns a boolean if a field has been set.

### GetResponseCode

`func (o *ViewSmsInboundAutomations) GetResponseCode() string`

GetResponseCode returns the ResponseCode field if non-nil, zero value otherwise.

### GetResponseCodeOk

`func (o *ViewSmsInboundAutomations) GetResponseCodeOk() (*string, bool)`

GetResponseCodeOk returns a tuple with the ResponseCode field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetResponseCode

`func (o *ViewSmsInboundAutomations) SetResponseCode(v string)`

SetResponseCode sets ResponseCode field to given value.

### HasResponseCode

`func (o *ViewSmsInboundAutomations) HasResponseCode() bool`

HasResponseCode returns a boolean if a field has been set.

### GetResponseMsg

`func (o *ViewSmsInboundAutomations) GetResponseMsg() string`

GetResponseMsg returns the ResponseMsg field if non-nil, zero value otherwise.

### GetResponseMsgOk

`func (o *ViewSmsInboundAutomations) GetResponseMsgOk() (*string, bool)`

GetResponseMsgOk returns a tuple with the ResponseMsg field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetResponseMsg

`func (o *ViewSmsInboundAutomations) SetResponseMsg(v string)`

SetResponseMsg sets ResponseMsg field to given value.

### HasResponseMsg

`func (o *ViewSmsInboundAutomations) HasResponseMsg() bool`

HasResponseMsg returns a boolean if a field has been set.

### GetData

`func (o *ViewSmsInboundAutomations) GetData() ViewSmsInboundAutomationsData`

GetData returns the Data field if non-nil, zero value otherwise.

### GetDataOk

`func (o *ViewSmsInboundAutomations) GetDataOk() (*ViewSmsInboundAutomationsData, bool)`

GetDataOk returns a tuple with the Data field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetData

`func (o *ViewSmsInboundAutomations) SetData(v ViewSmsInboundAutomationsData)`

SetData sets Data field to given value.

### HasData

`func (o *ViewSmsInboundAutomations) HasData() bool`

HasData returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


