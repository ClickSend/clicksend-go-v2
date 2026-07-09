# SendEmailCampaignRequest

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
**CustomString** | Pointer to **string** |  | [optional] 
**Body** | Pointer to **string** |  | [optional] 

## Methods

### NewSendEmailCampaignRequest

`func NewSendEmailCampaignRequest() *SendEmailCampaignRequest`

NewSendEmailCampaignRequest instantiates a new SendEmailCampaignRequest object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewSendEmailCampaignRequestWithDefaults

`func NewSendEmailCampaignRequestWithDefaults() *SendEmailCampaignRequest`

NewSendEmailCampaignRequestWithDefaults instantiates a new SendEmailCampaignRequest object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetName

`func (o *SendEmailCampaignRequest) GetName() string`

GetName returns the Name field if non-nil, zero value otherwise.

### GetNameOk

`func (o *SendEmailCampaignRequest) GetNameOk() (*string, bool)`

GetNameOk returns a tuple with the Name field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetName

`func (o *SendEmailCampaignRequest) SetName(v string)`

SetName sets Name field to given value.

### HasName

`func (o *SendEmailCampaignRequest) HasName() bool`

HasName returns a boolean if a field has been set.

### GetSubject

`func (o *SendEmailCampaignRequest) GetSubject() string`

GetSubject returns the Subject field if non-nil, zero value otherwise.

### GetSubjectOk

`func (o *SendEmailCampaignRequest) GetSubjectOk() (*string, bool)`

GetSubjectOk returns a tuple with the Subject field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSubject

`func (o *SendEmailCampaignRequest) SetSubject(v string)`

SetSubject sets Subject field to given value.

### HasSubject

`func (o *SendEmailCampaignRequest) HasSubject() bool`

HasSubject returns a boolean if a field has been set.

### GetFromEmailAddressId

`func (o *SendEmailCampaignRequest) GetFromEmailAddressId() string`

GetFromEmailAddressId returns the FromEmailAddressId field if non-nil, zero value otherwise.

### GetFromEmailAddressIdOk

`func (o *SendEmailCampaignRequest) GetFromEmailAddressIdOk() (*string, bool)`

GetFromEmailAddressIdOk returns a tuple with the FromEmailAddressId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetFromEmailAddressId

`func (o *SendEmailCampaignRequest) SetFromEmailAddressId(v string)`

SetFromEmailAddressId sets FromEmailAddressId field to given value.

### HasFromEmailAddressId

`func (o *SendEmailCampaignRequest) HasFromEmailAddressId() bool`

HasFromEmailAddressId returns a boolean if a field has been set.

### GetTemplateId

`func (o *SendEmailCampaignRequest) GetTemplateId() string`

GetTemplateId returns the TemplateId field if non-nil, zero value otherwise.

### GetTemplateIdOk

`func (o *SendEmailCampaignRequest) GetTemplateIdOk() (*string, bool)`

GetTemplateIdOk returns a tuple with the TemplateId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTemplateId

`func (o *SendEmailCampaignRequest) SetTemplateId(v string)`

SetTemplateId sets TemplateId field to given value.

### HasTemplateId

`func (o *SendEmailCampaignRequest) HasTemplateId() bool`

HasTemplateId returns a boolean if a field has been set.

### GetListId

`func (o *SendEmailCampaignRequest) GetListId() string`

GetListId returns the ListId field if non-nil, zero value otherwise.

### GetListIdOk

`func (o *SendEmailCampaignRequest) GetListIdOk() (*string, bool)`

GetListIdOk returns a tuple with the ListId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetListId

`func (o *SendEmailCampaignRequest) SetListId(v string)`

SetListId sets ListId field to given value.

### HasListId

`func (o *SendEmailCampaignRequest) HasListId() bool`

HasListId returns a boolean if a field has been set.

### GetFromName

`func (o *SendEmailCampaignRequest) GetFromName() string`

GetFromName returns the FromName field if non-nil, zero value otherwise.

### GetFromNameOk

`func (o *SendEmailCampaignRequest) GetFromNameOk() (*string, bool)`

GetFromNameOk returns a tuple with the FromName field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetFromName

`func (o *SendEmailCampaignRequest) SetFromName(v string)`

SetFromName sets FromName field to given value.

### HasFromName

`func (o *SendEmailCampaignRequest) HasFromName() bool`

HasFromName returns a boolean if a field has been set.

### GetDraft

`func (o *SendEmailCampaignRequest) GetDraft() int32`

GetDraft returns the Draft field if non-nil, zero value otherwise.

### GetDraftOk

`func (o *SendEmailCampaignRequest) GetDraftOk() (*int32, bool)`

GetDraftOk returns a tuple with the Draft field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDraft

`func (o *SendEmailCampaignRequest) SetDraft(v int32)`

SetDraft sets Draft field to given value.

### HasDraft

`func (o *SendEmailCampaignRequest) HasDraft() bool`

HasDraft returns a boolean if a field has been set.

### GetCustomString

`func (o *SendEmailCampaignRequest) GetCustomString() string`

GetCustomString returns the CustomString field if non-nil, zero value otherwise.

### GetCustomStringOk

`func (o *SendEmailCampaignRequest) GetCustomStringOk() (*string, bool)`

GetCustomStringOk returns a tuple with the CustomString field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCustomString

`func (o *SendEmailCampaignRequest) SetCustomString(v string)`

SetCustomString sets CustomString field to given value.

### HasCustomString

`func (o *SendEmailCampaignRequest) HasCustomString() bool`

HasCustomString returns a boolean if a field has been set.

### GetBody

`func (o *SendEmailCampaignRequest) GetBody() string`

GetBody returns the Body field if non-nil, zero value otherwise.

### GetBodyOk

`func (o *SendEmailCampaignRequest) GetBodyOk() (*string, bool)`

GetBodyOk returns a tuple with the Body field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetBody

`func (o *SendEmailCampaignRequest) SetBody(v string)`

SetBody sets Body field to given value.

### HasBody

`func (o *SendEmailCampaignRequest) HasBody() bool`

HasBody returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


