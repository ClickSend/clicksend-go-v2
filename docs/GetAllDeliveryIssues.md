# GetAllDeliveryIssues

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**HttpCode** | Pointer to **int32** | The HTTP status code of the response. | [optional] 
**ResponseCode** | Pointer to **string** | The response code indicating the status of the operation. | [optional] 
**ResponseMsg** | Pointer to **string** | A message describing the outcome of the operation. | [optional] 
**Data** | Pointer to [**GetAllDeliveryIssuesData**](GetAllDeliveryIssuesData.md) |  | [optional] 

## Methods

### NewGetAllDeliveryIssues

`func NewGetAllDeliveryIssues() *GetAllDeliveryIssues`

NewGetAllDeliveryIssues instantiates a new GetAllDeliveryIssues object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewGetAllDeliveryIssuesWithDefaults

`func NewGetAllDeliveryIssuesWithDefaults() *GetAllDeliveryIssues`

NewGetAllDeliveryIssuesWithDefaults instantiates a new GetAllDeliveryIssues object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetHttpCode

`func (o *GetAllDeliveryIssues) GetHttpCode() int32`

GetHttpCode returns the HttpCode field if non-nil, zero value otherwise.

### GetHttpCodeOk

`func (o *GetAllDeliveryIssues) GetHttpCodeOk() (*int32, bool)`

GetHttpCodeOk returns a tuple with the HttpCode field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetHttpCode

`func (o *GetAllDeliveryIssues) SetHttpCode(v int32)`

SetHttpCode sets HttpCode field to given value.

### HasHttpCode

`func (o *GetAllDeliveryIssues) HasHttpCode() bool`

HasHttpCode returns a boolean if a field has been set.

### GetResponseCode

`func (o *GetAllDeliveryIssues) GetResponseCode() string`

GetResponseCode returns the ResponseCode field if non-nil, zero value otherwise.

### GetResponseCodeOk

`func (o *GetAllDeliveryIssues) GetResponseCodeOk() (*string, bool)`

GetResponseCodeOk returns a tuple with the ResponseCode field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetResponseCode

`func (o *GetAllDeliveryIssues) SetResponseCode(v string)`

SetResponseCode sets ResponseCode field to given value.

### HasResponseCode

`func (o *GetAllDeliveryIssues) HasResponseCode() bool`

HasResponseCode returns a boolean if a field has been set.

### GetResponseMsg

`func (o *GetAllDeliveryIssues) GetResponseMsg() string`

GetResponseMsg returns the ResponseMsg field if non-nil, zero value otherwise.

### GetResponseMsgOk

`func (o *GetAllDeliveryIssues) GetResponseMsgOk() (*string, bool)`

GetResponseMsgOk returns a tuple with the ResponseMsg field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetResponseMsg

`func (o *GetAllDeliveryIssues) SetResponseMsg(v string)`

SetResponseMsg sets ResponseMsg field to given value.

### HasResponseMsg

`func (o *GetAllDeliveryIssues) HasResponseMsg() bool`

HasResponseMsg returns a boolean if a field has been set.

### GetData

`func (o *GetAllDeliveryIssues) GetData() GetAllDeliveryIssuesData`

GetData returns the Data field if non-nil, zero value otherwise.

### GetDataOk

`func (o *GetAllDeliveryIssues) GetDataOk() (*GetAllDeliveryIssuesData, bool)`

GetDataOk returns a tuple with the Data field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetData

`func (o *GetAllDeliveryIssues) SetData(v GetAllDeliveryIssuesData)`

SetData sets Data field to given value.

### HasData

`func (o *GetAllDeliveryIssues) HasData() bool`

HasData returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


