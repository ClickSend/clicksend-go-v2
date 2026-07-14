# GlobalSending

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Id** | Pointer to **int32** | The ID of the country. | [optional] 
**Name** | Pointer to **string** | The name of the country. | [optional] 
**Code** | Pointer to **string** | The country code. | [optional] 
**Region** | Pointer to **string** | The region of the country. | [optional] 
**AgreedAt** | Pointer to **NullableString** | The date when the country was agreed upon. | [optional] 
**RegistrationEntity** | Pointer to [**NullableAccountReferrerChosen**](AccountReferrerChosen.md) |  | [optional] 
**RegistrationStatus** | Pointer to [**GlobalSendingRegistrationStatus**](GlobalSendingRegistrationStatus.md) |  | [optional] 
**JotformId** | Pointer to **string** | The ID of the country in JotForm. | [optional] 
**SmsRegistrationType** | Pointer to **int32** | The type of SMS registration. | [optional] 
**BlockRegistration** | Pointer to **bool** | Indicates if registration is blocked. | [optional] 
**BlockLeads** | Pointer to **bool** | Indicates if leads are blocked. | [optional] 
**TrialFromAddress** | Pointer to **string** | The trial from address. | [optional] 
**RestrictedSending** | Pointer to **bool** | Indicates if sending is restricted. | [optional] 
**TrialSending** | Pointer to **int32** | Indicates if trial sending is allowed. | [optional] 
**TrialSendingDescription** | Pointer to **string** | Description of trial sending. | [optional] 
**HasRegulationRequirements** | Pointer to **int32** | Indicates if there are regulation requirements. | [optional] 
**RegistrationStepsUrl** | Pointer to **string** | URL for registration steps. | [optional] 
**RegulationRequirementsDescription** | Pointer to **string** | Description of regulation requirements. | [optional] 

## Methods

### NewGlobalSending

`func NewGlobalSending() *GlobalSending`

NewGlobalSending instantiates a new GlobalSending object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewGlobalSendingWithDefaults

`func NewGlobalSendingWithDefaults() *GlobalSending`

NewGlobalSendingWithDefaults instantiates a new GlobalSending object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetId

`func (o *GlobalSending) GetId() int32`

GetId returns the Id field if non-nil, zero value otherwise.

### GetIdOk

`func (o *GlobalSending) GetIdOk() (*int32, bool)`

GetIdOk returns a tuple with the Id field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetId

`func (o *GlobalSending) SetId(v int32)`

SetId sets Id field to given value.

### HasId

`func (o *GlobalSending) HasId() bool`

HasId returns a boolean if a field has been set.

### GetName

`func (o *GlobalSending) GetName() string`

GetName returns the Name field if non-nil, zero value otherwise.

### GetNameOk

`func (o *GlobalSending) GetNameOk() (*string, bool)`

GetNameOk returns a tuple with the Name field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetName

`func (o *GlobalSending) SetName(v string)`

SetName sets Name field to given value.

### HasName

`func (o *GlobalSending) HasName() bool`

HasName returns a boolean if a field has been set.

### GetCode

`func (o *GlobalSending) GetCode() string`

GetCode returns the Code field if non-nil, zero value otherwise.

### GetCodeOk

`func (o *GlobalSending) GetCodeOk() (*string, bool)`

GetCodeOk returns a tuple with the Code field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCode

`func (o *GlobalSending) SetCode(v string)`

SetCode sets Code field to given value.

### HasCode

`func (o *GlobalSending) HasCode() bool`

HasCode returns a boolean if a field has been set.

### GetRegion

`func (o *GlobalSending) GetRegion() string`

GetRegion returns the Region field if non-nil, zero value otherwise.

### GetRegionOk

`func (o *GlobalSending) GetRegionOk() (*string, bool)`

GetRegionOk returns a tuple with the Region field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetRegion

`func (o *GlobalSending) SetRegion(v string)`

SetRegion sets Region field to given value.

### HasRegion

`func (o *GlobalSending) HasRegion() bool`

HasRegion returns a boolean if a field has been set.

### GetAgreedAt

`func (o *GlobalSending) GetAgreedAt() string`

GetAgreedAt returns the AgreedAt field if non-nil, zero value otherwise.

### GetAgreedAtOk

`func (o *GlobalSending) GetAgreedAtOk() (*string, bool)`

GetAgreedAtOk returns a tuple with the AgreedAt field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAgreedAt

`func (o *GlobalSending) SetAgreedAt(v string)`

SetAgreedAt sets AgreedAt field to given value.

### HasAgreedAt

`func (o *GlobalSending) HasAgreedAt() bool`

HasAgreedAt returns a boolean if a field has been set.

### SetAgreedAtNil

`func (o *GlobalSending) SetAgreedAtNil(b bool)`

 SetAgreedAtNil sets the value for AgreedAt to be an explicit nil

### UnsetAgreedAt
`func (o *GlobalSending) UnsetAgreedAt()`

UnsetAgreedAt ensures that no value is present for AgreedAt, not even an explicit nil
### GetRegistrationEntity

`func (o *GlobalSending) GetRegistrationEntity() AccountReferrerChosen`

GetRegistrationEntity returns the RegistrationEntity field if non-nil, zero value otherwise.

### GetRegistrationEntityOk

`func (o *GlobalSending) GetRegistrationEntityOk() (*AccountReferrerChosen, bool)`

GetRegistrationEntityOk returns a tuple with the RegistrationEntity field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetRegistrationEntity

`func (o *GlobalSending) SetRegistrationEntity(v AccountReferrerChosen)`

SetRegistrationEntity sets RegistrationEntity field to given value.

### HasRegistrationEntity

`func (o *GlobalSending) HasRegistrationEntity() bool`

HasRegistrationEntity returns a boolean if a field has been set.

### SetRegistrationEntityNil

`func (o *GlobalSending) SetRegistrationEntityNil(b bool)`

 SetRegistrationEntityNil sets the value for RegistrationEntity to be an explicit nil

### UnsetRegistrationEntity
`func (o *GlobalSending) UnsetRegistrationEntity()`

UnsetRegistrationEntity ensures that no value is present for RegistrationEntity, not even an explicit nil
### GetRegistrationStatus

`func (o *GlobalSending) GetRegistrationStatus() GlobalSendingRegistrationStatus`

GetRegistrationStatus returns the RegistrationStatus field if non-nil, zero value otherwise.

### GetRegistrationStatusOk

`func (o *GlobalSending) GetRegistrationStatusOk() (*GlobalSendingRegistrationStatus, bool)`

GetRegistrationStatusOk returns a tuple with the RegistrationStatus field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetRegistrationStatus

`func (o *GlobalSending) SetRegistrationStatus(v GlobalSendingRegistrationStatus)`

SetRegistrationStatus sets RegistrationStatus field to given value.

### HasRegistrationStatus

`func (o *GlobalSending) HasRegistrationStatus() bool`

HasRegistrationStatus returns a boolean if a field has been set.

### GetJotformId

`func (o *GlobalSending) GetJotformId() string`

GetJotformId returns the JotformId field if non-nil, zero value otherwise.

### GetJotformIdOk

`func (o *GlobalSending) GetJotformIdOk() (*string, bool)`

GetJotformIdOk returns a tuple with the JotformId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetJotformId

`func (o *GlobalSending) SetJotformId(v string)`

SetJotformId sets JotformId field to given value.

### HasJotformId

`func (o *GlobalSending) HasJotformId() bool`

HasJotformId returns a boolean if a field has been set.

### GetSmsRegistrationType

`func (o *GlobalSending) GetSmsRegistrationType() int32`

GetSmsRegistrationType returns the SmsRegistrationType field if non-nil, zero value otherwise.

### GetSmsRegistrationTypeOk

`func (o *GlobalSending) GetSmsRegistrationTypeOk() (*int32, bool)`

GetSmsRegistrationTypeOk returns a tuple with the SmsRegistrationType field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSmsRegistrationType

`func (o *GlobalSending) SetSmsRegistrationType(v int32)`

SetSmsRegistrationType sets SmsRegistrationType field to given value.

### HasSmsRegistrationType

`func (o *GlobalSending) HasSmsRegistrationType() bool`

HasSmsRegistrationType returns a boolean if a field has been set.

### GetBlockRegistration

`func (o *GlobalSending) GetBlockRegistration() bool`

GetBlockRegistration returns the BlockRegistration field if non-nil, zero value otherwise.

### GetBlockRegistrationOk

`func (o *GlobalSending) GetBlockRegistrationOk() (*bool, bool)`

GetBlockRegistrationOk returns a tuple with the BlockRegistration field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetBlockRegistration

`func (o *GlobalSending) SetBlockRegistration(v bool)`

SetBlockRegistration sets BlockRegistration field to given value.

### HasBlockRegistration

`func (o *GlobalSending) HasBlockRegistration() bool`

HasBlockRegistration returns a boolean if a field has been set.

### GetBlockLeads

`func (o *GlobalSending) GetBlockLeads() bool`

GetBlockLeads returns the BlockLeads field if non-nil, zero value otherwise.

### GetBlockLeadsOk

`func (o *GlobalSending) GetBlockLeadsOk() (*bool, bool)`

GetBlockLeadsOk returns a tuple with the BlockLeads field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetBlockLeads

`func (o *GlobalSending) SetBlockLeads(v bool)`

SetBlockLeads sets BlockLeads field to given value.

### HasBlockLeads

`func (o *GlobalSending) HasBlockLeads() bool`

HasBlockLeads returns a boolean if a field has been set.

### GetTrialFromAddress

`func (o *GlobalSending) GetTrialFromAddress() string`

GetTrialFromAddress returns the TrialFromAddress field if non-nil, zero value otherwise.

### GetTrialFromAddressOk

`func (o *GlobalSending) GetTrialFromAddressOk() (*string, bool)`

GetTrialFromAddressOk returns a tuple with the TrialFromAddress field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTrialFromAddress

`func (o *GlobalSending) SetTrialFromAddress(v string)`

SetTrialFromAddress sets TrialFromAddress field to given value.

### HasTrialFromAddress

`func (o *GlobalSending) HasTrialFromAddress() bool`

HasTrialFromAddress returns a boolean if a field has been set.

### GetRestrictedSending

`func (o *GlobalSending) GetRestrictedSending() bool`

GetRestrictedSending returns the RestrictedSending field if non-nil, zero value otherwise.

### GetRestrictedSendingOk

`func (o *GlobalSending) GetRestrictedSendingOk() (*bool, bool)`

GetRestrictedSendingOk returns a tuple with the RestrictedSending field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetRestrictedSending

`func (o *GlobalSending) SetRestrictedSending(v bool)`

SetRestrictedSending sets RestrictedSending field to given value.

### HasRestrictedSending

`func (o *GlobalSending) HasRestrictedSending() bool`

HasRestrictedSending returns a boolean if a field has been set.

### GetTrialSending

`func (o *GlobalSending) GetTrialSending() int32`

GetTrialSending returns the TrialSending field if non-nil, zero value otherwise.

### GetTrialSendingOk

`func (o *GlobalSending) GetTrialSendingOk() (*int32, bool)`

GetTrialSendingOk returns a tuple with the TrialSending field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTrialSending

`func (o *GlobalSending) SetTrialSending(v int32)`

SetTrialSending sets TrialSending field to given value.

### HasTrialSending

`func (o *GlobalSending) HasTrialSending() bool`

HasTrialSending returns a boolean if a field has been set.

### GetTrialSendingDescription

`func (o *GlobalSending) GetTrialSendingDescription() string`

GetTrialSendingDescription returns the TrialSendingDescription field if non-nil, zero value otherwise.

### GetTrialSendingDescriptionOk

`func (o *GlobalSending) GetTrialSendingDescriptionOk() (*string, bool)`

GetTrialSendingDescriptionOk returns a tuple with the TrialSendingDescription field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTrialSendingDescription

`func (o *GlobalSending) SetTrialSendingDescription(v string)`

SetTrialSendingDescription sets TrialSendingDescription field to given value.

### HasTrialSendingDescription

`func (o *GlobalSending) HasTrialSendingDescription() bool`

HasTrialSendingDescription returns a boolean if a field has been set.

### GetHasRegulationRequirements

`func (o *GlobalSending) GetHasRegulationRequirements() int32`

GetHasRegulationRequirements returns the HasRegulationRequirements field if non-nil, zero value otherwise.

### GetHasRegulationRequirementsOk

`func (o *GlobalSending) GetHasRegulationRequirementsOk() (*int32, bool)`

GetHasRegulationRequirementsOk returns a tuple with the HasRegulationRequirements field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetHasRegulationRequirements

`func (o *GlobalSending) SetHasRegulationRequirements(v int32)`

SetHasRegulationRequirements sets HasRegulationRequirements field to given value.

### HasHasRegulationRequirements

`func (o *GlobalSending) HasHasRegulationRequirements() bool`

HasHasRegulationRequirements returns a boolean if a field has been set.

### GetRegistrationStepsUrl

`func (o *GlobalSending) GetRegistrationStepsUrl() string`

GetRegistrationStepsUrl returns the RegistrationStepsUrl field if non-nil, zero value otherwise.

### GetRegistrationStepsUrlOk

`func (o *GlobalSending) GetRegistrationStepsUrlOk() (*string, bool)`

GetRegistrationStepsUrlOk returns a tuple with the RegistrationStepsUrl field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetRegistrationStepsUrl

`func (o *GlobalSending) SetRegistrationStepsUrl(v string)`

SetRegistrationStepsUrl sets RegistrationStepsUrl field to given value.

### HasRegistrationStepsUrl

`func (o *GlobalSending) HasRegistrationStepsUrl() bool`

HasRegistrationStepsUrl returns a boolean if a field has been set.

### GetRegulationRequirementsDescription

`func (o *GlobalSending) GetRegulationRequirementsDescription() string`

GetRegulationRequirementsDescription returns the RegulationRequirementsDescription field if non-nil, zero value otherwise.

### GetRegulationRequirementsDescriptionOk

`func (o *GlobalSending) GetRegulationRequirementsDescriptionOk() (*string, bool)`

GetRegulationRequirementsDescriptionOk returns a tuple with the RegulationRequirementsDescription field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetRegulationRequirementsDescription

`func (o *GlobalSending) SetRegulationRequirementsDescription(v string)`

SetRegulationRequirementsDescription sets RegulationRequirementsDescription field to given value.

### HasRegulationRequirementsDescription

`func (o *GlobalSending) HasRegulationRequirementsDescription() bool`

HasRegulationRequirementsDescription returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


