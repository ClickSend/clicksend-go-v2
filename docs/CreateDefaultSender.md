# CreateDefaultSender

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**HttpCode** | **int32** | HTTP status code of the response. | 
**ResponseCode** | **string** | Code indicating the result of the response. | 
**ResponseMsg** | **string** | Message providing additional information. | 
**Data** | [**DefaultSender**](DefaultSender.md) |  | 

## Methods

### NewCreateDefaultSender

`func NewCreateDefaultSender(httpCode int32, responseCode string, responseMsg string, data DefaultSender, ) *CreateDefaultSender`

NewCreateDefaultSender instantiates a new CreateDefaultSender object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewCreateDefaultSenderWithDefaults

`func NewCreateDefaultSenderWithDefaults() *CreateDefaultSender`

NewCreateDefaultSenderWithDefaults instantiates a new CreateDefaultSender object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetHttpCode

`func (o *CreateDefaultSender) GetHttpCode() int32`

GetHttpCode returns the HttpCode field if non-nil, zero value otherwise.

### GetHttpCodeOk

`func (o *CreateDefaultSender) GetHttpCodeOk() (*int32, bool)`

GetHttpCodeOk returns a tuple with the HttpCode field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetHttpCode

`func (o *CreateDefaultSender) SetHttpCode(v int32)`

SetHttpCode sets HttpCode field to given value.


### GetResponseCode

`func (o *CreateDefaultSender) GetResponseCode() string`

GetResponseCode returns the ResponseCode field if non-nil, zero value otherwise.

### GetResponseCodeOk

`func (o *CreateDefaultSender) GetResponseCodeOk() (*string, bool)`

GetResponseCodeOk returns a tuple with the ResponseCode field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetResponseCode

`func (o *CreateDefaultSender) SetResponseCode(v string)`

SetResponseCode sets ResponseCode field to given value.


### GetResponseMsg

`func (o *CreateDefaultSender) GetResponseMsg() string`

GetResponseMsg returns the ResponseMsg field if non-nil, zero value otherwise.

### GetResponseMsgOk

`func (o *CreateDefaultSender) GetResponseMsgOk() (*string, bool)`

GetResponseMsgOk returns a tuple with the ResponseMsg field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetResponseMsg

`func (o *CreateDefaultSender) SetResponseMsg(v string)`

SetResponseMsg sets ResponseMsg field to given value.


### GetData

`func (o *CreateDefaultSender) GetData() DefaultSender`

GetData returns the Data field if non-nil, zero value otherwise.

### GetDataOk

`func (o *CreateDefaultSender) GetDataOk() (*DefaultSender, bool)`

GetDataOk returns a tuple with the Data field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetData

`func (o *CreateDefaultSender) SetData(v DefaultSender)`

SetData sets Data field to given value.



[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


