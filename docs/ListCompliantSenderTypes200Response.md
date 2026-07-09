# ListCompliantSenderTypes200Response

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**HttpCode** | **int32** | HTTP status code of the response | 
**ResponseCode** | **string** | Code indicating the result of the response | 
**ResponseMsg** | **string** | Message providing additional information | 
**Data** | [**ListCompliantSenderTypes200ResponseData**](ListCompliantSenderTypes200ResponseData.md) |  | 

## Methods

### NewListCompliantSenderTypes200Response

`func NewListCompliantSenderTypes200Response(httpCode int32, responseCode string, responseMsg string, data ListCompliantSenderTypes200ResponseData, ) *ListCompliantSenderTypes200Response`

NewListCompliantSenderTypes200Response instantiates a new ListCompliantSenderTypes200Response object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewListCompliantSenderTypes200ResponseWithDefaults

`func NewListCompliantSenderTypes200ResponseWithDefaults() *ListCompliantSenderTypes200Response`

NewListCompliantSenderTypes200ResponseWithDefaults instantiates a new ListCompliantSenderTypes200Response object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetHttpCode

`func (o *ListCompliantSenderTypes200Response) GetHttpCode() int32`

GetHttpCode returns the HttpCode field if non-nil, zero value otherwise.

### GetHttpCodeOk

`func (o *ListCompliantSenderTypes200Response) GetHttpCodeOk() (*int32, bool)`

GetHttpCodeOk returns a tuple with the HttpCode field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetHttpCode

`func (o *ListCompliantSenderTypes200Response) SetHttpCode(v int32)`

SetHttpCode sets HttpCode field to given value.


### GetResponseCode

`func (o *ListCompliantSenderTypes200Response) GetResponseCode() string`

GetResponseCode returns the ResponseCode field if non-nil, zero value otherwise.

### GetResponseCodeOk

`func (o *ListCompliantSenderTypes200Response) GetResponseCodeOk() (*string, bool)`

GetResponseCodeOk returns a tuple with the ResponseCode field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetResponseCode

`func (o *ListCompliantSenderTypes200Response) SetResponseCode(v string)`

SetResponseCode sets ResponseCode field to given value.


### GetResponseMsg

`func (o *ListCompliantSenderTypes200Response) GetResponseMsg() string`

GetResponseMsg returns the ResponseMsg field if non-nil, zero value otherwise.

### GetResponseMsgOk

`func (o *ListCompliantSenderTypes200Response) GetResponseMsgOk() (*string, bool)`

GetResponseMsgOk returns a tuple with the ResponseMsg field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetResponseMsg

`func (o *ListCompliantSenderTypes200Response) SetResponseMsg(v string)`

SetResponseMsg sets ResponseMsg field to given value.


### GetData

`func (o *ListCompliantSenderTypes200Response) GetData() ListCompliantSenderTypes200ResponseData`

GetData returns the Data field if non-nil, zero value otherwise.

### GetDataOk

`func (o *ListCompliantSenderTypes200Response) GetDataOk() (*ListCompliantSenderTypes200ResponseData, bool)`

GetDataOk returns a tuple with the Data field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetData

`func (o *ListCompliantSenderTypes200Response) SetData(v ListCompliantSenderTypes200ResponseData)`

SetData sets Data field to given value.



[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


