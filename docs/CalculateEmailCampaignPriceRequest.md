# CalculateEmailCampaignPriceRequest

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Name** | Pointer to **string** |  | [optional] 
**Subject** | Pointer to **string** |  | [optional] 
**FromEmailAddressId** | Pointer to **string** |  | [optional] 
**TemplateId** | Pointer to **string** |  | [optional] 
**ListId** | Pointer to **string** |  | [optional] 
**FromName** | Pointer to **string** |  | [optional] 
**Draft** | Pointer to **int32** |  | [optional] 
**Schedule** | Pointer to **string** |  | [optional] 
**CustomString** | Pointer to **string** |  | [optional] 
**Body** | Pointer to **string** |  | [optional] 

## Methods

### NewCalculateEmailCampaignPriceRequest

`func NewCalculateEmailCampaignPriceRequest() *CalculateEmailCampaignPriceRequest`

NewCalculateEmailCampaignPriceRequest instantiates a new CalculateEmailCampaignPriceRequest object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewCalculateEmailCampaignPriceRequestWithDefaults

`func NewCalculateEmailCampaignPriceRequestWithDefaults() *CalculateEmailCampaignPriceRequest`

NewCalculateEmailCampaignPriceRequestWithDefaults instantiates a new CalculateEmailCampaignPriceRequest object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetName

`func (o *CalculateEmailCampaignPriceRequest) GetName() string`

GetName returns the Name field if non-nil, zero value otherwise.

### GetNameOk

`func (o *CalculateEmailCampaignPriceRequest) GetNameOk() (*string, bool)`

GetNameOk returns a tuple with the Name field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetName

`func (o *CalculateEmailCampaignPriceRequest) SetName(v string)`

SetName sets Name field to given value.

### HasName

`func (o *CalculateEmailCampaignPriceRequest) HasName() bool`

HasName returns a boolean if a field has been set.

### GetSubject

`func (o *CalculateEmailCampaignPriceRequest) GetSubject() string`

GetSubject returns the Subject field if non-nil, zero value otherwise.

### GetSubjectOk

`func (o *CalculateEmailCampaignPriceRequest) GetSubjectOk() (*string, bool)`

GetSubjectOk returns a tuple with the Subject field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSubject

`func (o *CalculateEmailCampaignPriceRequest) SetSubject(v string)`

SetSubject sets Subject field to given value.

### HasSubject

`func (o *CalculateEmailCampaignPriceRequest) HasSubject() bool`

HasSubject returns a boolean if a field has been set.

### GetFromEmailAddressId

`func (o *CalculateEmailCampaignPriceRequest) GetFromEmailAddressId() string`

GetFromEmailAddressId returns the FromEmailAddressId field if non-nil, zero value otherwise.

### GetFromEmailAddressIdOk

`func (o *CalculateEmailCampaignPriceRequest) GetFromEmailAddressIdOk() (*string, bool)`

GetFromEmailAddressIdOk returns a tuple with the FromEmailAddressId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetFromEmailAddressId

`func (o *CalculateEmailCampaignPriceRequest) SetFromEmailAddressId(v string)`

SetFromEmailAddressId sets FromEmailAddressId field to given value.

### HasFromEmailAddressId

`func (o *CalculateEmailCampaignPriceRequest) HasFromEmailAddressId() bool`

HasFromEmailAddressId returns a boolean if a field has been set.

### GetTemplateId

`func (o *CalculateEmailCampaignPriceRequest) GetTemplateId() string`

GetTemplateId returns the TemplateId field if non-nil, zero value otherwise.

### GetTemplateIdOk

`func (o *CalculateEmailCampaignPriceRequest) GetTemplateIdOk() (*string, bool)`

GetTemplateIdOk returns a tuple with the TemplateId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTemplateId

`func (o *CalculateEmailCampaignPriceRequest) SetTemplateId(v string)`

SetTemplateId sets TemplateId field to given value.

### HasTemplateId

`func (o *CalculateEmailCampaignPriceRequest) HasTemplateId() bool`

HasTemplateId returns a boolean if a field has been set.

### GetListId

`func (o *CalculateEmailCampaignPriceRequest) GetListId() string`

GetListId returns the ListId field if non-nil, zero value otherwise.

### GetListIdOk

`func (o *CalculateEmailCampaignPriceRequest) GetListIdOk() (*string, bool)`

GetListIdOk returns a tuple with the ListId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetListId

`func (o *CalculateEmailCampaignPriceRequest) SetListId(v string)`

SetListId sets ListId field to given value.

### HasListId

`func (o *CalculateEmailCampaignPriceRequest) HasListId() bool`

HasListId returns a boolean if a field has been set.

### GetFromName

`func (o *CalculateEmailCampaignPriceRequest) GetFromName() string`

GetFromName returns the FromName field if non-nil, zero value otherwise.

### GetFromNameOk

`func (o *CalculateEmailCampaignPriceRequest) GetFromNameOk() (*string, bool)`

GetFromNameOk returns a tuple with the FromName field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetFromName

`func (o *CalculateEmailCampaignPriceRequest) SetFromName(v string)`

SetFromName sets FromName field to given value.

### HasFromName

`func (o *CalculateEmailCampaignPriceRequest) HasFromName() bool`

HasFromName returns a boolean if a field has been set.

### GetDraft

`func (o *CalculateEmailCampaignPriceRequest) GetDraft() int32`

GetDraft returns the Draft field if non-nil, zero value otherwise.

### GetDraftOk

`func (o *CalculateEmailCampaignPriceRequest) GetDraftOk() (*int32, bool)`

GetDraftOk returns a tuple with the Draft field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDraft

`func (o *CalculateEmailCampaignPriceRequest) SetDraft(v int32)`

SetDraft sets Draft field to given value.

### HasDraft

`func (o *CalculateEmailCampaignPriceRequest) HasDraft() bool`

HasDraft returns a boolean if a field has been set.

### GetSchedule

`func (o *CalculateEmailCampaignPriceRequest) GetSchedule() string`

GetSchedule returns the Schedule field if non-nil, zero value otherwise.

### GetScheduleOk

`func (o *CalculateEmailCampaignPriceRequest) GetScheduleOk() (*string, bool)`

GetScheduleOk returns a tuple with the Schedule field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSchedule

`func (o *CalculateEmailCampaignPriceRequest) SetSchedule(v string)`

SetSchedule sets Schedule field to given value.

### HasSchedule

`func (o *CalculateEmailCampaignPriceRequest) HasSchedule() bool`

HasSchedule returns a boolean if a field has been set.

### GetCustomString

`func (o *CalculateEmailCampaignPriceRequest) GetCustomString() string`

GetCustomString returns the CustomString field if non-nil, zero value otherwise.

### GetCustomStringOk

`func (o *CalculateEmailCampaignPriceRequest) GetCustomStringOk() (*string, bool)`

GetCustomStringOk returns a tuple with the CustomString field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCustomString

`func (o *CalculateEmailCampaignPriceRequest) SetCustomString(v string)`

SetCustomString sets CustomString field to given value.

### HasCustomString

`func (o *CalculateEmailCampaignPriceRequest) HasCustomString() bool`

HasCustomString returns a boolean if a field has been set.

### GetBody

`func (o *CalculateEmailCampaignPriceRequest) GetBody() string`

GetBody returns the Body field if non-nil, zero value otherwise.

### GetBodyOk

`func (o *CalculateEmailCampaignPriceRequest) GetBodyOk() (*string, bool)`

GetBodyOk returns a tuple with the Body field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetBody

`func (o *CalculateEmailCampaignPriceRequest) SetBody(v string)`

SetBody sets Body field to given value.

### HasBody

`func (o *CalculateEmailCampaignPriceRequest) HasBody() bool`

HasBody returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


