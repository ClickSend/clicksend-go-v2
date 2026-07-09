# SmsTemplateUpdate

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**TemplateId** | Pointer to **int32** | The generated ID of the template. This remains the same and can’t be updated. | [optional] 
**Body** | Pointer to **string** | The new updated content of the template. | [optional] 
**TemplateName** | Pointer to **string** | The new updated name of the template. | [optional] 

## Methods

### NewSmsTemplateUpdate

`func NewSmsTemplateUpdate() *SmsTemplateUpdate`

NewSmsTemplateUpdate instantiates a new SmsTemplateUpdate object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewSmsTemplateUpdateWithDefaults

`func NewSmsTemplateUpdateWithDefaults() *SmsTemplateUpdate`

NewSmsTemplateUpdateWithDefaults instantiates a new SmsTemplateUpdate object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetTemplateId

`func (o *SmsTemplateUpdate) GetTemplateId() int32`

GetTemplateId returns the TemplateId field if non-nil, zero value otherwise.

### GetTemplateIdOk

`func (o *SmsTemplateUpdate) GetTemplateIdOk() (*int32, bool)`

GetTemplateIdOk returns a tuple with the TemplateId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTemplateId

`func (o *SmsTemplateUpdate) SetTemplateId(v int32)`

SetTemplateId sets TemplateId field to given value.

### HasTemplateId

`func (o *SmsTemplateUpdate) HasTemplateId() bool`

HasTemplateId returns a boolean if a field has been set.

### GetBody

`func (o *SmsTemplateUpdate) GetBody() string`

GetBody returns the Body field if non-nil, zero value otherwise.

### GetBodyOk

`func (o *SmsTemplateUpdate) GetBodyOk() (*string, bool)`

GetBodyOk returns a tuple with the Body field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetBody

`func (o *SmsTemplateUpdate) SetBody(v string)`

SetBody sets Body field to given value.

### HasBody

`func (o *SmsTemplateUpdate) HasBody() bool`

HasBody returns a boolean if a field has been set.

### GetTemplateName

`func (o *SmsTemplateUpdate) GetTemplateName() string`

GetTemplateName returns the TemplateName field if non-nil, zero value otherwise.

### GetTemplateNameOk

`func (o *SmsTemplateUpdate) GetTemplateNameOk() (*string, bool)`

GetTemplateNameOk returns a tuple with the TemplateName field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTemplateName

`func (o *SmsTemplateUpdate) SetTemplateName(v string)`

SetTemplateName sets TemplateName field to given value.

### HasTemplateName

`func (o *SmsTemplateUpdate) HasTemplateName() bool`

HasTemplateName returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


