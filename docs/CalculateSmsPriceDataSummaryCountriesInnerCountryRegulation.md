# CalculateSmsPriceDataSummaryCountriesInnerCountryRegulation

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**CountryUserId** | Pointer to **int32** | Your identifier for the country regulation. | [optional] 
**SmsRegistrationType** | Pointer to **int32** | The global sending requirement for this country. It can be one of the following:  - **0:** No number or account registration required.      - **1:** Number registration required. You can purchase a registered number from ClickSend. Examples: US and CA.      - **2:** Account registration required. You can register your company details or business details to register your account. Examples: NZ, SG and UAE.  This parameter is a duplicate of registration_type.  &lt;div class&#x3D;\&quot;info-box\&quot;&gt;   &lt;h4&gt;&lt;i class&#x3D;\&quot;fas fa-info-circle\&quot;&gt;&lt;/i&gt; Note:&lt;/h4&gt;   &lt;p&gt;This parameter is fixed and can&#39;t be changed based on your settings.&lt;/p&gt; &lt;/div&gt; | [optional] 
**RestrictedSending** | Pointer to **bool** | Indicates whether you have any restriction for sending the message to this country:  - **True:** You&#39;re restricted from sending messages to this country, possibly due to not having a registered number.      - **False:** You&#39;re not restricted from sending messages to this country. | [optional] 
**TrialSending** | Pointer to **bool** | Indicates whether the country supports trial sending or not:  - **True:** This country supports trial sending      - **False:** This country doesn’t support trial sending  Countries with restricted sending typically offers trial sending. With trial sending, you can send messages to the country without registering your number or account.  &lt;div class&#x3D;\&quot;info-box\&quot;&gt;   &lt;h4&gt;&lt;i class&#x3D;\&quot;fas fa-info-circle\&quot;&gt;&lt;/i&gt; Note:&lt;/h4&gt;   &lt;p&gt;Trial sending has limitations, such as a daily limit of 200 messages in some countries. The limitations vary by country. &lt;br/&gt;&lt;br/&gt; This parameter is fixed and can&#39;t be changed based on your settings.&lt;/p&gt; &lt;/div&gt; | [optional] 
**RegulationRequirementsDescription** | Pointer to **string** | The text description of the regulatory requirements. | [optional] 
**CreatedAt** | Pointer to [**CalculateSmsPriceDataSummaryCountriesInnerCountryRegulationCreatedAt**](CalculateSmsPriceDataSummaryCountriesInnerCountryRegulationCreatedAt.md) |  | [optional] 
**UpdatedAt** | Pointer to [**CalculateSmsPriceDataSummaryCountriesInnerCountryRegulationCreatedAt**](CalculateSmsPriceDataSummaryCountriesInnerCountryRegulationCreatedAt.md) |  | [optional] 

## Methods

### NewCalculateSmsPriceDataSummaryCountriesInnerCountryRegulation

`func NewCalculateSmsPriceDataSummaryCountriesInnerCountryRegulation() *CalculateSmsPriceDataSummaryCountriesInnerCountryRegulation`

NewCalculateSmsPriceDataSummaryCountriesInnerCountryRegulation instantiates a new CalculateSmsPriceDataSummaryCountriesInnerCountryRegulation object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewCalculateSmsPriceDataSummaryCountriesInnerCountryRegulationWithDefaults

`func NewCalculateSmsPriceDataSummaryCountriesInnerCountryRegulationWithDefaults() *CalculateSmsPriceDataSummaryCountriesInnerCountryRegulation`

NewCalculateSmsPriceDataSummaryCountriesInnerCountryRegulationWithDefaults instantiates a new CalculateSmsPriceDataSummaryCountriesInnerCountryRegulation object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetCountryUserId

`func (o *CalculateSmsPriceDataSummaryCountriesInnerCountryRegulation) GetCountryUserId() int32`

GetCountryUserId returns the CountryUserId field if non-nil, zero value otherwise.

### GetCountryUserIdOk

`func (o *CalculateSmsPriceDataSummaryCountriesInnerCountryRegulation) GetCountryUserIdOk() (*int32, bool)`

GetCountryUserIdOk returns a tuple with the CountryUserId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCountryUserId

`func (o *CalculateSmsPriceDataSummaryCountriesInnerCountryRegulation) SetCountryUserId(v int32)`

SetCountryUserId sets CountryUserId field to given value.

### HasCountryUserId

`func (o *CalculateSmsPriceDataSummaryCountriesInnerCountryRegulation) HasCountryUserId() bool`

HasCountryUserId returns a boolean if a field has been set.

### GetSmsRegistrationType

`func (o *CalculateSmsPriceDataSummaryCountriesInnerCountryRegulation) GetSmsRegistrationType() int32`

GetSmsRegistrationType returns the SmsRegistrationType field if non-nil, zero value otherwise.

### GetSmsRegistrationTypeOk

`func (o *CalculateSmsPriceDataSummaryCountriesInnerCountryRegulation) GetSmsRegistrationTypeOk() (*int32, bool)`

GetSmsRegistrationTypeOk returns a tuple with the SmsRegistrationType field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSmsRegistrationType

`func (o *CalculateSmsPriceDataSummaryCountriesInnerCountryRegulation) SetSmsRegistrationType(v int32)`

SetSmsRegistrationType sets SmsRegistrationType field to given value.

### HasSmsRegistrationType

`func (o *CalculateSmsPriceDataSummaryCountriesInnerCountryRegulation) HasSmsRegistrationType() bool`

HasSmsRegistrationType returns a boolean if a field has been set.

### GetRestrictedSending

`func (o *CalculateSmsPriceDataSummaryCountriesInnerCountryRegulation) GetRestrictedSending() bool`

GetRestrictedSending returns the RestrictedSending field if non-nil, zero value otherwise.

### GetRestrictedSendingOk

`func (o *CalculateSmsPriceDataSummaryCountriesInnerCountryRegulation) GetRestrictedSendingOk() (*bool, bool)`

GetRestrictedSendingOk returns a tuple with the RestrictedSending field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetRestrictedSending

`func (o *CalculateSmsPriceDataSummaryCountriesInnerCountryRegulation) SetRestrictedSending(v bool)`

SetRestrictedSending sets RestrictedSending field to given value.

### HasRestrictedSending

`func (o *CalculateSmsPriceDataSummaryCountriesInnerCountryRegulation) HasRestrictedSending() bool`

HasRestrictedSending returns a boolean if a field has been set.

### GetTrialSending

`func (o *CalculateSmsPriceDataSummaryCountriesInnerCountryRegulation) GetTrialSending() bool`

GetTrialSending returns the TrialSending field if non-nil, zero value otherwise.

### GetTrialSendingOk

`func (o *CalculateSmsPriceDataSummaryCountriesInnerCountryRegulation) GetTrialSendingOk() (*bool, bool)`

GetTrialSendingOk returns a tuple with the TrialSending field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTrialSending

`func (o *CalculateSmsPriceDataSummaryCountriesInnerCountryRegulation) SetTrialSending(v bool)`

SetTrialSending sets TrialSending field to given value.

### HasTrialSending

`func (o *CalculateSmsPriceDataSummaryCountriesInnerCountryRegulation) HasTrialSending() bool`

HasTrialSending returns a boolean if a field has been set.

### GetRegulationRequirementsDescription

`func (o *CalculateSmsPriceDataSummaryCountriesInnerCountryRegulation) GetRegulationRequirementsDescription() string`

GetRegulationRequirementsDescription returns the RegulationRequirementsDescription field if non-nil, zero value otherwise.

### GetRegulationRequirementsDescriptionOk

`func (o *CalculateSmsPriceDataSummaryCountriesInnerCountryRegulation) GetRegulationRequirementsDescriptionOk() (*string, bool)`

GetRegulationRequirementsDescriptionOk returns a tuple with the RegulationRequirementsDescription field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetRegulationRequirementsDescription

`func (o *CalculateSmsPriceDataSummaryCountriesInnerCountryRegulation) SetRegulationRequirementsDescription(v string)`

SetRegulationRequirementsDescription sets RegulationRequirementsDescription field to given value.

### HasRegulationRequirementsDescription

`func (o *CalculateSmsPriceDataSummaryCountriesInnerCountryRegulation) HasRegulationRequirementsDescription() bool`

HasRegulationRequirementsDescription returns a boolean if a field has been set.

### GetCreatedAt

`func (o *CalculateSmsPriceDataSummaryCountriesInnerCountryRegulation) GetCreatedAt() CalculateSmsPriceDataSummaryCountriesInnerCountryRegulationCreatedAt`

GetCreatedAt returns the CreatedAt field if non-nil, zero value otherwise.

### GetCreatedAtOk

`func (o *CalculateSmsPriceDataSummaryCountriesInnerCountryRegulation) GetCreatedAtOk() (*CalculateSmsPriceDataSummaryCountriesInnerCountryRegulationCreatedAt, bool)`

GetCreatedAtOk returns a tuple with the CreatedAt field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCreatedAt

`func (o *CalculateSmsPriceDataSummaryCountriesInnerCountryRegulation) SetCreatedAt(v CalculateSmsPriceDataSummaryCountriesInnerCountryRegulationCreatedAt)`

SetCreatedAt sets CreatedAt field to given value.

### HasCreatedAt

`func (o *CalculateSmsPriceDataSummaryCountriesInnerCountryRegulation) HasCreatedAt() bool`

HasCreatedAt returns a boolean if a field has been set.

### GetUpdatedAt

`func (o *CalculateSmsPriceDataSummaryCountriesInnerCountryRegulation) GetUpdatedAt() CalculateSmsPriceDataSummaryCountriesInnerCountryRegulationCreatedAt`

GetUpdatedAt returns the UpdatedAt field if non-nil, zero value otherwise.

### GetUpdatedAtOk

`func (o *CalculateSmsPriceDataSummaryCountriesInnerCountryRegulation) GetUpdatedAtOk() (*CalculateSmsPriceDataSummaryCountriesInnerCountryRegulationCreatedAt, bool)`

GetUpdatedAtOk returns a tuple with the UpdatedAt field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetUpdatedAt

`func (o *CalculateSmsPriceDataSummaryCountriesInnerCountryRegulation) SetUpdatedAt(v CalculateSmsPriceDataSummaryCountriesInnerCountryRegulationCreatedAt)`

SetUpdatedAt sets UpdatedAt field to given value.

### HasUpdatedAt

`func (o *CalculateSmsPriceDataSummaryCountriesInnerCountryRegulation) HasUpdatedAt() bool`

HasUpdatedAt returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


