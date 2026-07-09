# CalculateLetterPriceRequest

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**FileUrl** | Pointer to **string** |  | [optional] 
**TemplateUsed** | Pointer to **int32** |  | [optional] 
**Duplex** | Pointer to **int32** |  | [optional] 
**Colour** | Pointer to **int32** |  | [optional] 
**Source** | Pointer to **string** |  | [optional] 
**Recipients** | Pointer to [**[]SendPostcardRequestRecipientsInner**](SendPostcardRequestRecipientsInner.md) |  | [optional] 

## Methods

### NewCalculateLetterPriceRequest

`func NewCalculateLetterPriceRequest() *CalculateLetterPriceRequest`

NewCalculateLetterPriceRequest instantiates a new CalculateLetterPriceRequest object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewCalculateLetterPriceRequestWithDefaults

`func NewCalculateLetterPriceRequestWithDefaults() *CalculateLetterPriceRequest`

NewCalculateLetterPriceRequestWithDefaults instantiates a new CalculateLetterPriceRequest object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetFileUrl

`func (o *CalculateLetterPriceRequest) GetFileUrl() string`

GetFileUrl returns the FileUrl field if non-nil, zero value otherwise.

### GetFileUrlOk

`func (o *CalculateLetterPriceRequest) GetFileUrlOk() (*string, bool)`

GetFileUrlOk returns a tuple with the FileUrl field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetFileUrl

`func (o *CalculateLetterPriceRequest) SetFileUrl(v string)`

SetFileUrl sets FileUrl field to given value.

### HasFileUrl

`func (o *CalculateLetterPriceRequest) HasFileUrl() bool`

HasFileUrl returns a boolean if a field has been set.

### GetTemplateUsed

`func (o *CalculateLetterPriceRequest) GetTemplateUsed() int32`

GetTemplateUsed returns the TemplateUsed field if non-nil, zero value otherwise.

### GetTemplateUsedOk

`func (o *CalculateLetterPriceRequest) GetTemplateUsedOk() (*int32, bool)`

GetTemplateUsedOk returns a tuple with the TemplateUsed field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTemplateUsed

`func (o *CalculateLetterPriceRequest) SetTemplateUsed(v int32)`

SetTemplateUsed sets TemplateUsed field to given value.

### HasTemplateUsed

`func (o *CalculateLetterPriceRequest) HasTemplateUsed() bool`

HasTemplateUsed returns a boolean if a field has been set.

### GetDuplex

`func (o *CalculateLetterPriceRequest) GetDuplex() int32`

GetDuplex returns the Duplex field if non-nil, zero value otherwise.

### GetDuplexOk

`func (o *CalculateLetterPriceRequest) GetDuplexOk() (*int32, bool)`

GetDuplexOk returns a tuple with the Duplex field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDuplex

`func (o *CalculateLetterPriceRequest) SetDuplex(v int32)`

SetDuplex sets Duplex field to given value.

### HasDuplex

`func (o *CalculateLetterPriceRequest) HasDuplex() bool`

HasDuplex returns a boolean if a field has been set.

### GetColour

`func (o *CalculateLetterPriceRequest) GetColour() int32`

GetColour returns the Colour field if non-nil, zero value otherwise.

### GetColourOk

`func (o *CalculateLetterPriceRequest) GetColourOk() (*int32, bool)`

GetColourOk returns a tuple with the Colour field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetColour

`func (o *CalculateLetterPriceRequest) SetColour(v int32)`

SetColour sets Colour field to given value.

### HasColour

`func (o *CalculateLetterPriceRequest) HasColour() bool`

HasColour returns a boolean if a field has been set.

### GetSource

`func (o *CalculateLetterPriceRequest) GetSource() string`

GetSource returns the Source field if non-nil, zero value otherwise.

### GetSourceOk

`func (o *CalculateLetterPriceRequest) GetSourceOk() (*string, bool)`

GetSourceOk returns a tuple with the Source field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSource

`func (o *CalculateLetterPriceRequest) SetSource(v string)`

SetSource sets Source field to given value.

### HasSource

`func (o *CalculateLetterPriceRequest) HasSource() bool`

HasSource returns a boolean if a field has been set.

### GetRecipients

`func (o *CalculateLetterPriceRequest) GetRecipients() []SendPostcardRequestRecipientsInner`

GetRecipients returns the Recipients field if non-nil, zero value otherwise.

### GetRecipientsOk

`func (o *CalculateLetterPriceRequest) GetRecipientsOk() (*[]SendPostcardRequestRecipientsInner, bool)`

GetRecipientsOk returns a tuple with the Recipients field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetRecipients

`func (o *CalculateLetterPriceRequest) SetRecipients(v []SendPostcardRequestRecipientsInner)`

SetRecipients sets Recipients field to given value.

### HasRecipients

`func (o *CalculateLetterPriceRequest) HasRecipients() bool`

HasRecipients returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


