# ViewEmailDeliveryReceiptRules

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**HttpCode** | Pointer to **int32** | The HTTP status code of the response. | [optional] 
**ResponseCode** | Pointer to **string** | The response code indicating the status of the operation. | [optional] 
**ResponseMsg** | Pointer to **string** | A message describing the outcome of the operation. | [optional] 
**Data** | Pointer to [**ViewEmailDeliveryReceiptRulesData**](ViewEmailDeliveryReceiptRulesData.md) |  | [optional] 

## Methods

### NewViewEmailDeliveryReceiptRules

`func NewViewEmailDeliveryReceiptRules() *ViewEmailDeliveryReceiptRules`

NewViewEmailDeliveryReceiptRules instantiates a new ViewEmailDeliveryReceiptRules object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewViewEmailDeliveryReceiptRulesWithDefaults

`func NewViewEmailDeliveryReceiptRulesWithDefaults() *ViewEmailDeliveryReceiptRules`

NewViewEmailDeliveryReceiptRulesWithDefaults instantiates a new ViewEmailDeliveryReceiptRules object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetHttpCode

`func (o *ViewEmailDeliveryReceiptRules) GetHttpCode() int32`

GetHttpCode returns the HttpCode field if non-nil, zero value otherwise.

### GetHttpCodeOk

`func (o *ViewEmailDeliveryReceiptRules) GetHttpCodeOk() (*int32, bool)`

GetHttpCodeOk returns a tuple with the HttpCode field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetHttpCode

`func (o *ViewEmailDeliveryReceiptRules) SetHttpCode(v int32)`

SetHttpCode sets HttpCode field to given value.

### HasHttpCode

`func (o *ViewEmailDeliveryReceiptRules) HasHttpCode() bool`

HasHttpCode returns a boolean if a field has been set.

### GetResponseCode

`func (o *ViewEmailDeliveryReceiptRules) GetResponseCode() string`

GetResponseCode returns the ResponseCode field if non-nil, zero value otherwise.

### GetResponseCodeOk

`func (o *ViewEmailDeliveryReceiptRules) GetResponseCodeOk() (*string, bool)`

GetResponseCodeOk returns a tuple with the ResponseCode field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetResponseCode

`func (o *ViewEmailDeliveryReceiptRules) SetResponseCode(v string)`

SetResponseCode sets ResponseCode field to given value.

### HasResponseCode

`func (o *ViewEmailDeliveryReceiptRules) HasResponseCode() bool`

HasResponseCode returns a boolean if a field has been set.

### GetResponseMsg

`func (o *ViewEmailDeliveryReceiptRules) GetResponseMsg() string`

GetResponseMsg returns the ResponseMsg field if non-nil, zero value otherwise.

### GetResponseMsgOk

`func (o *ViewEmailDeliveryReceiptRules) GetResponseMsgOk() (*string, bool)`

GetResponseMsgOk returns a tuple with the ResponseMsg field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetResponseMsg

`func (o *ViewEmailDeliveryReceiptRules) SetResponseMsg(v string)`

SetResponseMsg sets ResponseMsg field to given value.

### HasResponseMsg

`func (o *ViewEmailDeliveryReceiptRules) HasResponseMsg() bool`

HasResponseMsg returns a boolean if a field has been set.

### GetData

`func (o *ViewEmailDeliveryReceiptRules) GetData() ViewEmailDeliveryReceiptRulesData`

GetData returns the Data field if non-nil, zero value otherwise.

### GetDataOk

`func (o *ViewEmailDeliveryReceiptRules) GetDataOk() (*ViewEmailDeliveryReceiptRulesData, bool)`

GetDataOk returns a tuple with the Data field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetData

`func (o *ViewEmailDeliveryReceiptRules) SetData(v ViewEmailDeliveryReceiptRulesData)`

SetData sets Data field to given value.

### HasData

`func (o *ViewEmailDeliveryReceiptRules) HasData() bool`

HasData returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


