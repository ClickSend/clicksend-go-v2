# RegisterNumbers

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**HttpCode** | **int32** | HTTP status code of the response. | 
**ResponseCode** | **string** | Code indicating the result of the response. | 
**ResponseMsg** | **string** | Message providing additional information. | 
**Data** | Pointer to **map[string]interface{}** |  | [optional] 

## Methods

### NewRegisterNumbers

`func NewRegisterNumbers(httpCode int32, responseCode string, responseMsg string, ) *RegisterNumbers`

NewRegisterNumbers instantiates a new RegisterNumbers object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewRegisterNumbersWithDefaults

`func NewRegisterNumbersWithDefaults() *RegisterNumbers`

NewRegisterNumbersWithDefaults instantiates a new RegisterNumbers object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetHttpCode

`func (o *RegisterNumbers) GetHttpCode() int32`

GetHttpCode returns the HttpCode field if non-nil, zero value otherwise.

### GetHttpCodeOk

`func (o *RegisterNumbers) GetHttpCodeOk() (*int32, bool)`

GetHttpCodeOk returns a tuple with the HttpCode field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetHttpCode

`func (o *RegisterNumbers) SetHttpCode(v int32)`

SetHttpCode sets HttpCode field to given value.


### GetResponseCode

`func (o *RegisterNumbers) GetResponseCode() string`

GetResponseCode returns the ResponseCode field if non-nil, zero value otherwise.

### GetResponseCodeOk

`func (o *RegisterNumbers) GetResponseCodeOk() (*string, bool)`

GetResponseCodeOk returns a tuple with the ResponseCode field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetResponseCode

`func (o *RegisterNumbers) SetResponseCode(v string)`

SetResponseCode sets ResponseCode field to given value.


### GetResponseMsg

`func (o *RegisterNumbers) GetResponseMsg() string`

GetResponseMsg returns the ResponseMsg field if non-nil, zero value otherwise.

### GetResponseMsgOk

`func (o *RegisterNumbers) GetResponseMsgOk() (*string, bool)`

GetResponseMsgOk returns a tuple with the ResponseMsg field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetResponseMsg

`func (o *RegisterNumbers) SetResponseMsg(v string)`

SetResponseMsg sets ResponseMsg field to given value.


### GetData

`func (o *RegisterNumbers) GetData() map[string]interface{}`

GetData returns the Data field if non-nil, zero value otherwise.

### GetDataOk

`func (o *RegisterNumbers) GetDataOk() (*map[string]interface{}, bool)`

GetDataOk returns a tuple with the Data field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetData

`func (o *RegisterNumbers) SetData(v map[string]interface{})`

SetData sets Data field to given value.

### HasData

`func (o *RegisterNumbers) HasData() bool`

HasData returns a boolean if a field has been set.

### SetDataNil

`func (o *RegisterNumbers) SetDataNil(b bool)`

 SetDataNil sets the value for Data to be an explicit nil

### UnsetData
`func (o *RegisterNumbers) UnsetData()`

UnsetData ensures that no value is present for Data, not even an explicit nil

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


