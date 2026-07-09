# CreateSmsTemplateRequest

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**TemplateName** | Pointer to **string** | The name of the template. | [optional] 
**Body** | Pointer to **string** | body String The main content of your template. | [optional] 

## Methods

### NewCreateSmsTemplateRequest

`func NewCreateSmsTemplateRequest() *CreateSmsTemplateRequest`

NewCreateSmsTemplateRequest instantiates a new CreateSmsTemplateRequest object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewCreateSmsTemplateRequestWithDefaults

`func NewCreateSmsTemplateRequestWithDefaults() *CreateSmsTemplateRequest`

NewCreateSmsTemplateRequestWithDefaults instantiates a new CreateSmsTemplateRequest object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetTemplateName

`func (o *CreateSmsTemplateRequest) GetTemplateName() string`

GetTemplateName returns the TemplateName field if non-nil, zero value otherwise.

### GetTemplateNameOk

`func (o *CreateSmsTemplateRequest) GetTemplateNameOk() (*string, bool)`

GetTemplateNameOk returns a tuple with the TemplateName field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTemplateName

`func (o *CreateSmsTemplateRequest) SetTemplateName(v string)`

SetTemplateName sets TemplateName field to given value.

### HasTemplateName

`func (o *CreateSmsTemplateRequest) HasTemplateName() bool`

HasTemplateName returns a boolean if a field has been set.

### GetBody

`func (o *CreateSmsTemplateRequest) GetBody() string`

GetBody returns the Body field if non-nil, zero value otherwise.

### GetBodyOk

`func (o *CreateSmsTemplateRequest) GetBodyOk() (*string, bool)`

GetBodyOk returns a tuple with the Body field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetBody

`func (o *CreateSmsTemplateRequest) SetBody(v string)`

SetBody sets Body field to given value.

### HasBody

`func (o *CreateSmsTemplateRequest) HasBody() bool`

HasBody returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


