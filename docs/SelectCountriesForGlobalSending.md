# SelectCountriesForGlobalSending

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**HttpCode** | Pointer to **int32** | The HTTP status code of the response. | [optional] 
**ResponseCode** | Pointer to **string** | The response code indicating the status of the operation. | [optional] 
**ResponseMsg** | Pointer to **string** | A message describing the outcome of the operation. | [optional] 
**Data** | Pointer to [**[]GlobalSending**](GlobalSending.md) |  | [optional] 

## Methods

### NewSelectCountriesForGlobalSending

`func NewSelectCountriesForGlobalSending() *SelectCountriesForGlobalSending`

NewSelectCountriesForGlobalSending instantiates a new SelectCountriesForGlobalSending object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewSelectCountriesForGlobalSendingWithDefaults

`func NewSelectCountriesForGlobalSendingWithDefaults() *SelectCountriesForGlobalSending`

NewSelectCountriesForGlobalSendingWithDefaults instantiates a new SelectCountriesForGlobalSending object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetHttpCode

`func (o *SelectCountriesForGlobalSending) GetHttpCode() int32`

GetHttpCode returns the HttpCode field if non-nil, zero value otherwise.

### GetHttpCodeOk

`func (o *SelectCountriesForGlobalSending) GetHttpCodeOk() (*int32, bool)`

GetHttpCodeOk returns a tuple with the HttpCode field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetHttpCode

`func (o *SelectCountriesForGlobalSending) SetHttpCode(v int32)`

SetHttpCode sets HttpCode field to given value.

### HasHttpCode

`func (o *SelectCountriesForGlobalSending) HasHttpCode() bool`

HasHttpCode returns a boolean if a field has been set.

### GetResponseCode

`func (o *SelectCountriesForGlobalSending) GetResponseCode() string`

GetResponseCode returns the ResponseCode field if non-nil, zero value otherwise.

### GetResponseCodeOk

`func (o *SelectCountriesForGlobalSending) GetResponseCodeOk() (*string, bool)`

GetResponseCodeOk returns a tuple with the ResponseCode field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetResponseCode

`func (o *SelectCountriesForGlobalSending) SetResponseCode(v string)`

SetResponseCode sets ResponseCode field to given value.

### HasResponseCode

`func (o *SelectCountriesForGlobalSending) HasResponseCode() bool`

HasResponseCode returns a boolean if a field has been set.

### GetResponseMsg

`func (o *SelectCountriesForGlobalSending) GetResponseMsg() string`

GetResponseMsg returns the ResponseMsg field if non-nil, zero value otherwise.

### GetResponseMsgOk

`func (o *SelectCountriesForGlobalSending) GetResponseMsgOk() (*string, bool)`

GetResponseMsgOk returns a tuple with the ResponseMsg field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetResponseMsg

`func (o *SelectCountriesForGlobalSending) SetResponseMsg(v string)`

SetResponseMsg sets ResponseMsg field to given value.

### HasResponseMsg

`func (o *SelectCountriesForGlobalSending) HasResponseMsg() bool`

HasResponseMsg returns a boolean if a field has been set.

### GetData

`func (o *SelectCountriesForGlobalSending) GetData() []GlobalSending`

GetData returns the Data field if non-nil, zero value otherwise.

### GetDataOk

`func (o *SelectCountriesForGlobalSending) GetDataOk() (*[]GlobalSending, bool)`

GetDataOk returns a tuple with the Data field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetData

`func (o *SelectCountriesForGlobalSending) SetData(v []GlobalSending)`

SetData sets Data field to given value.

### HasData

`func (o *SelectCountriesForGlobalSending) HasData() bool`

HasData returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


