# Attachment

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**FileName** | Pointer to **string** | The name of the attached file. | [optional] 
**ContentType** | Pointer to **string** | The MIME type of the attached file. | [optional] 
**ContentDisposition** | Pointer to **string** | The content disposition of the attached file. | [optional] 
**ContentId** | Pointer to **string** | The content ID of the attached file. | [optional] 
**AttachmentFileUrl** | Pointer to **string** | The URL to download the attached file. | [optional] 

## Methods

### NewAttachment

`func NewAttachment() *Attachment`

NewAttachment instantiates a new Attachment object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewAttachmentWithDefaults

`func NewAttachmentWithDefaults() *Attachment`

NewAttachmentWithDefaults instantiates a new Attachment object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetFileName

`func (o *Attachment) GetFileName() string`

GetFileName returns the FileName field if non-nil, zero value otherwise.

### GetFileNameOk

`func (o *Attachment) GetFileNameOk() (*string, bool)`

GetFileNameOk returns a tuple with the FileName field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetFileName

`func (o *Attachment) SetFileName(v string)`

SetFileName sets FileName field to given value.

### HasFileName

`func (o *Attachment) HasFileName() bool`

HasFileName returns a boolean if a field has been set.

### GetContentType

`func (o *Attachment) GetContentType() string`

GetContentType returns the ContentType field if non-nil, zero value otherwise.

### GetContentTypeOk

`func (o *Attachment) GetContentTypeOk() (*string, bool)`

GetContentTypeOk returns a tuple with the ContentType field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetContentType

`func (o *Attachment) SetContentType(v string)`

SetContentType sets ContentType field to given value.

### HasContentType

`func (o *Attachment) HasContentType() bool`

HasContentType returns a boolean if a field has been set.

### GetContentDisposition

`func (o *Attachment) GetContentDisposition() string`

GetContentDisposition returns the ContentDisposition field if non-nil, zero value otherwise.

### GetContentDispositionOk

`func (o *Attachment) GetContentDispositionOk() (*string, bool)`

GetContentDispositionOk returns a tuple with the ContentDisposition field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetContentDisposition

`func (o *Attachment) SetContentDisposition(v string)`

SetContentDisposition sets ContentDisposition field to given value.

### HasContentDisposition

`func (o *Attachment) HasContentDisposition() bool`

HasContentDisposition returns a boolean if a field has been set.

### GetContentId

`func (o *Attachment) GetContentId() string`

GetContentId returns the ContentId field if non-nil, zero value otherwise.

### GetContentIdOk

`func (o *Attachment) GetContentIdOk() (*string, bool)`

GetContentIdOk returns a tuple with the ContentId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetContentId

`func (o *Attachment) SetContentId(v string)`

SetContentId sets ContentId field to given value.

### HasContentId

`func (o *Attachment) HasContentId() bool`

HasContentId returns a boolean if a field has been set.

### GetAttachmentFileUrl

`func (o *Attachment) GetAttachmentFileUrl() string`

GetAttachmentFileUrl returns the AttachmentFileUrl field if non-nil, zero value otherwise.

### GetAttachmentFileUrlOk

`func (o *Attachment) GetAttachmentFileUrlOk() (*string, bool)`

GetAttachmentFileUrlOk returns a tuple with the AttachmentFileUrl field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAttachmentFileUrl

`func (o *Attachment) SetAttachmentFileUrl(v string)`

SetAttachmentFileUrl sets AttachmentFileUrl field to given value.

### HasAttachmentFileUrl

`func (o *Attachment) HasAttachmentFileUrl() bool`

HasAttachmentFileUrl returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


