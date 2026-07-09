# CancelEmailCampaignRequest

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Name** | Pointer to **string** |  | [optional] 
**Subject** | Pointer to **string** |  | [optional] 
**FromEmailAddressId** | Pointer to **int32** |  | [optional] 
**TemplateId** | Pointer to **int32** |  | [optional] 
**ListId** | Pointer to **int32** |  | [optional] 
**FromName** | Pointer to **string** |  | [optional] 
**Draft** | Pointer to **int32** |  | [optional] 
**Schedule** | Pointer to **string** |  | [optional] 
**CustomString** | Pointer to **string** |  | [optional] 
**Body** | Pointer to **string** |  | [optional] 

## Methods

### NewCancelEmailCampaignRequest

`func NewCancelEmailCampaignRequest() *CancelEmailCampaignRequest`

NewCancelEmailCampaignRequest instantiates a new CancelEmailCampaignRequest object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewCancelEmailCampaignRequestWithDefaults

`func NewCancelEmailCampaignRequestWithDefaults() *CancelEmailCampaignRequest`

NewCancelEmailCampaignRequestWithDefaults instantiates a new CancelEmailCampaignRequest object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetName

`func (o *CancelEmailCampaignRequest) GetName() string`

GetName returns the Name field if non-nil, zero value otherwise.

### GetNameOk

`func (o *CancelEmailCampaignRequest) GetNameOk() (*string, bool)`

GetNameOk returns a tuple with the Name field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetName

`func (o *CancelEmailCampaignRequest) SetName(v string)`

SetName sets Name field to given value.

### HasName

`func (o *CancelEmailCampaignRequest) HasName() bool`

HasName returns a boolean if a field has been set.

### GetSubject

`func (o *CancelEmailCampaignRequest) GetSubject() string`

GetSubject returns the Subject field if non-nil, zero value otherwise.

### GetSubjectOk

`func (o *CancelEmailCampaignRequest) GetSubjectOk() (*string, bool)`

GetSubjectOk returns a tuple with the Subject field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSubject

`func (o *CancelEmailCampaignRequest) SetSubject(v string)`

SetSubject sets Subject field to given value.

### HasSubject

`func (o *CancelEmailCampaignRequest) HasSubject() bool`

HasSubject returns a boolean if a field has been set.

### GetFromEmailAddressId

`func (o *CancelEmailCampaignRequest) GetFromEmailAddressId() int32`

GetFromEmailAddressId returns the FromEmailAddressId field if non-nil, zero value otherwise.

### GetFromEmailAddressIdOk

`func (o *CancelEmailCampaignRequest) GetFromEmailAddressIdOk() (*int32, bool)`

GetFromEmailAddressIdOk returns a tuple with the FromEmailAddressId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetFromEmailAddressId

`func (o *CancelEmailCampaignRequest) SetFromEmailAddressId(v int32)`

SetFromEmailAddressId sets FromEmailAddressId field to given value.

### HasFromEmailAddressId

`func (o *CancelEmailCampaignRequest) HasFromEmailAddressId() bool`

HasFromEmailAddressId returns a boolean if a field has been set.

### GetTemplateId

`func (o *CancelEmailCampaignRequest) GetTemplateId() int32`

GetTemplateId returns the TemplateId field if non-nil, zero value otherwise.

### GetTemplateIdOk

`func (o *CancelEmailCampaignRequest) GetTemplateIdOk() (*int32, bool)`

GetTemplateIdOk returns a tuple with the TemplateId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTemplateId

`func (o *CancelEmailCampaignRequest) SetTemplateId(v int32)`

SetTemplateId sets TemplateId field to given value.

### HasTemplateId

`func (o *CancelEmailCampaignRequest) HasTemplateId() bool`

HasTemplateId returns a boolean if a field has been set.

### GetListId

`func (o *CancelEmailCampaignRequest) GetListId() int32`

GetListId returns the ListId field if non-nil, zero value otherwise.

### GetListIdOk

`func (o *CancelEmailCampaignRequest) GetListIdOk() (*int32, bool)`

GetListIdOk returns a tuple with the ListId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetListId

`func (o *CancelEmailCampaignRequest) SetListId(v int32)`

SetListId sets ListId field to given value.

### HasListId

`func (o *CancelEmailCampaignRequest) HasListId() bool`

HasListId returns a boolean if a field has been set.

### GetFromName

`func (o *CancelEmailCampaignRequest) GetFromName() string`

GetFromName returns the FromName field if non-nil, zero value otherwise.

### GetFromNameOk

`func (o *CancelEmailCampaignRequest) GetFromNameOk() (*string, bool)`

GetFromNameOk returns a tuple with the FromName field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetFromName

`func (o *CancelEmailCampaignRequest) SetFromName(v string)`

SetFromName sets FromName field to given value.

### HasFromName

`func (o *CancelEmailCampaignRequest) HasFromName() bool`

HasFromName returns a boolean if a field has been set.

### GetDraft

`func (o *CancelEmailCampaignRequest) GetDraft() int32`

GetDraft returns the Draft field if non-nil, zero value otherwise.

### GetDraftOk

`func (o *CancelEmailCampaignRequest) GetDraftOk() (*int32, bool)`

GetDraftOk returns a tuple with the Draft field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDraft

`func (o *CancelEmailCampaignRequest) SetDraft(v int32)`

SetDraft sets Draft field to given value.

### HasDraft

`func (o *CancelEmailCampaignRequest) HasDraft() bool`

HasDraft returns a boolean if a field has been set.

### GetSchedule

`func (o *CancelEmailCampaignRequest) GetSchedule() string`

GetSchedule returns the Schedule field if non-nil, zero value otherwise.

### GetScheduleOk

`func (o *CancelEmailCampaignRequest) GetScheduleOk() (*string, bool)`

GetScheduleOk returns a tuple with the Schedule field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSchedule

`func (o *CancelEmailCampaignRequest) SetSchedule(v string)`

SetSchedule sets Schedule field to given value.

### HasSchedule

`func (o *CancelEmailCampaignRequest) HasSchedule() bool`

HasSchedule returns a boolean if a field has been set.

### GetCustomString

`func (o *CancelEmailCampaignRequest) GetCustomString() string`

GetCustomString returns the CustomString field if non-nil, zero value otherwise.

### GetCustomStringOk

`func (o *CancelEmailCampaignRequest) GetCustomStringOk() (*string, bool)`

GetCustomStringOk returns a tuple with the CustomString field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCustomString

`func (o *CancelEmailCampaignRequest) SetCustomString(v string)`

SetCustomString sets CustomString field to given value.

### HasCustomString

`func (o *CancelEmailCampaignRequest) HasCustomString() bool`

HasCustomString returns a boolean if a field has been set.

### GetBody

`func (o *CancelEmailCampaignRequest) GetBody() string`

GetBody returns the Body field if non-nil, zero value otherwise.

### GetBodyOk

`func (o *CancelEmailCampaignRequest) GetBodyOk() (*string, bool)`

GetBodyOk returns a tuple with the Body field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetBody

`func (o *CancelEmailCampaignRequest) SetBody(v string)`

SetBody sets Body field to given value.

### HasBody

`func (o *CancelEmailCampaignRequest) HasBody() bool`

HasBody returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


