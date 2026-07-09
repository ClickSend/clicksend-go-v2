# GetDefaultSendersList

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**HttpCode** | **int32** | HTTP status code of the response. | 
**ResponseCode** | **string** | Code indicating the result of the response. | 
**ResponseMsg** | **string** | Message providing additional information. | 
**Data** | [**GetDefaultSendersListData**](GetDefaultSendersListData.md) |  | 

## Methods

### NewGetDefaultSendersList

`func NewGetDefaultSendersList(httpCode int32, responseCode string, responseMsg string, data GetDefaultSendersListData, ) *GetDefaultSendersList`

NewGetDefaultSendersList instantiates a new GetDefaultSendersList object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewGetDefaultSendersListWithDefaults

`func NewGetDefaultSendersListWithDefaults() *GetDefaultSendersList`

NewGetDefaultSendersListWithDefaults instantiates a new GetDefaultSendersList object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetHttpCode

`func (o *GetDefaultSendersList) GetHttpCode() int32`

GetHttpCode returns the HttpCode field if non-nil, zero value otherwise.

### GetHttpCodeOk

`func (o *GetDefaultSendersList) GetHttpCodeOk() (*int32, bool)`

GetHttpCodeOk returns a tuple with the HttpCode field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetHttpCode

`func (o *GetDefaultSendersList) SetHttpCode(v int32)`

SetHttpCode sets HttpCode field to given value.


### GetResponseCode

`func (o *GetDefaultSendersList) GetResponseCode() string`

GetResponseCode returns the ResponseCode field if non-nil, zero value otherwise.

### GetResponseCodeOk

`func (o *GetDefaultSendersList) GetResponseCodeOk() (*string, bool)`

GetResponseCodeOk returns a tuple with the ResponseCode field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetResponseCode

`func (o *GetDefaultSendersList) SetResponseCode(v string)`

SetResponseCode sets ResponseCode field to given value.


### GetResponseMsg

`func (o *GetDefaultSendersList) GetResponseMsg() string`

GetResponseMsg returns the ResponseMsg field if non-nil, zero value otherwise.

### GetResponseMsgOk

`func (o *GetDefaultSendersList) GetResponseMsgOk() (*string, bool)`

GetResponseMsgOk returns a tuple with the ResponseMsg field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetResponseMsg

`func (o *GetDefaultSendersList) SetResponseMsg(v string)`

SetResponseMsg sets ResponseMsg field to given value.


### GetData

`func (o *GetDefaultSendersList) GetData() GetDefaultSendersListData`

GetData returns the Data field if non-nil, zero value otherwise.

### GetDataOk

`func (o *GetDefaultSendersList) GetDataOk() (*GetDefaultSendersListData, bool)`

GetDataOk returns a tuple with the Data field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetData

`func (o *GetDefaultSendersList) SetData(v GetDefaultSendersListData)`

SetData sets Data field to given value.



[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


