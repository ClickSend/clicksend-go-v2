# MasterEmailTemplate

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**TemplateIdMaster** | Pointer to **int32** | The unique identifier for the template. | [optional] 
**TemplateName** | Pointer to **string** | The name of the template. | [optional] 
**DateAdded** | Pointer to **string** | The date the template was added. | [optional] 
**Body** | Pointer to **NullableString** | The body of the template. | [optional] 
**Thumbnail** | Pointer to [**MasterEmailTemplateThumbnail**](MasterEmailTemplateThumbnail.md) |  | [optional] 

## Methods

### NewMasterEmailTemplate

`func NewMasterEmailTemplate() *MasterEmailTemplate`

NewMasterEmailTemplate instantiates a new MasterEmailTemplate object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewMasterEmailTemplateWithDefaults

`func NewMasterEmailTemplateWithDefaults() *MasterEmailTemplate`

NewMasterEmailTemplateWithDefaults instantiates a new MasterEmailTemplate object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetTemplateIdMaster

`func (o *MasterEmailTemplate) GetTemplateIdMaster() int32`

GetTemplateIdMaster returns the TemplateIdMaster field if non-nil, zero value otherwise.

### GetTemplateIdMasterOk

`func (o *MasterEmailTemplate) GetTemplateIdMasterOk() (*int32, bool)`

GetTemplateIdMasterOk returns a tuple with the TemplateIdMaster field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTemplateIdMaster

`func (o *MasterEmailTemplate) SetTemplateIdMaster(v int32)`

SetTemplateIdMaster sets TemplateIdMaster field to given value.

### HasTemplateIdMaster

`func (o *MasterEmailTemplate) HasTemplateIdMaster() bool`

HasTemplateIdMaster returns a boolean if a field has been set.

### GetTemplateName

`func (o *MasterEmailTemplate) GetTemplateName() string`

GetTemplateName returns the TemplateName field if non-nil, zero value otherwise.

### GetTemplateNameOk

`func (o *MasterEmailTemplate) GetTemplateNameOk() (*string, bool)`

GetTemplateNameOk returns a tuple with the TemplateName field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTemplateName

`func (o *MasterEmailTemplate) SetTemplateName(v string)`

SetTemplateName sets TemplateName field to given value.

### HasTemplateName

`func (o *MasterEmailTemplate) HasTemplateName() bool`

HasTemplateName returns a boolean if a field has been set.

### GetDateAdded

`func (o *MasterEmailTemplate) GetDateAdded() string`

GetDateAdded returns the DateAdded field if non-nil, zero value otherwise.

### GetDateAddedOk

`func (o *MasterEmailTemplate) GetDateAddedOk() (*string, bool)`

GetDateAddedOk returns a tuple with the DateAdded field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDateAdded

`func (o *MasterEmailTemplate) SetDateAdded(v string)`

SetDateAdded sets DateAdded field to given value.

### HasDateAdded

`func (o *MasterEmailTemplate) HasDateAdded() bool`

HasDateAdded returns a boolean if a field has been set.

### GetBody

`func (o *MasterEmailTemplate) GetBody() string`

GetBody returns the Body field if non-nil, zero value otherwise.

### GetBodyOk

`func (o *MasterEmailTemplate) GetBodyOk() (*string, bool)`

GetBodyOk returns a tuple with the Body field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetBody

`func (o *MasterEmailTemplate) SetBody(v string)`

SetBody sets Body field to given value.

### HasBody

`func (o *MasterEmailTemplate) HasBody() bool`

HasBody returns a boolean if a field has been set.

### SetBodyNil

`func (o *MasterEmailTemplate) SetBodyNil(b bool)`

 SetBodyNil sets the value for Body to be an explicit nil

### UnsetBody
`func (o *MasterEmailTemplate) UnsetBody()`

UnsetBody ensures that no value is present for Body, not even an explicit nil
### GetThumbnail

`func (o *MasterEmailTemplate) GetThumbnail() MasterEmailTemplateThumbnail`

GetThumbnail returns the Thumbnail field if non-nil, zero value otherwise.

### GetThumbnailOk

`func (o *MasterEmailTemplate) GetThumbnailOk() (*MasterEmailTemplateThumbnail, bool)`

GetThumbnailOk returns a tuple with the Thumbnail field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetThumbnail

`func (o *MasterEmailTemplate) SetThumbnail(v MasterEmailTemplateThumbnail)`

SetThumbnail sets Thumbnail field to given value.

### HasThumbnail

`func (o *MasterEmailTemplate) HasThumbnail() bool`

HasThumbnail returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


