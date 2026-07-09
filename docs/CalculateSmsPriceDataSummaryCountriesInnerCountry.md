# CalculateSmsPriceDataSummaryCountriesInnerCountry

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**RegistrationType** | Pointer to **int32** | The global sending requirement for this country. It can be one of the following:  - **0:** No number or account registration required.      - **1:** Number registration required. You can purchase a registered number from ClickSend. Examples: US and CA.      - **2:** Account registration required. You can register your company details or business details to register your account. Examples: NZ, SG and UAE.  &lt;div class&#x3D;\&quot;info-box\&quot;&gt;   &lt;h4&gt;&lt;i class&#x3D;\&quot;fas fa-info-circle\&quot;&gt;&lt;/i&gt; Note:&lt;/h4&gt;   &lt;p&gt;This parameter is fixed and can&#39;t be changed based on your settings.&lt;/p&gt; &lt;/div&gt; | [optional] 
**ReceipientCount** | Pointer to **int32** | The number of messages you are sending to this country. The system can count up to 1000 messages. | [optional] 
**UsableSenderId** | Pointer to **bool** | Indicates whether you have a usable ***Sender ID** for this country:  - **True:** A **Sender ID** is available for you to use.      - **False:** No **Sender ID** is available for you to use.  &lt;div class&#x3D;\&quot;info-box\&quot;&gt;     &lt;h4&gt;&lt;i class&#x3D;\&quot;fas fa-info-circle\&quot;&gt;&lt;/i&gt; Note:&lt;/h4&gt;     &lt;p&gt;Countries with &lt;em&gt;registration_type&lt;/em&gt; set to &lt;strong&gt;0&lt;/strong&gt; will have the &lt;em&gt;usable_sender_id&lt;/em&gt; set as &lt;strong&gt;True&lt;/strong&gt;, and messages will be sent from shared numbers.&lt;/p&gt; &lt;/div&gt; | [optional] 
**Selected** | Pointer to **bool** | Indicates whether you have enabled the global sending for this country:  - **True:** You have selected this country for global sending and can send messages here.      - **False:** You haven’t selected this country for global sending and can’t send messages here. | [optional] 
**Name** | Pointer to **string** | The name of the country. | [optional] 
**Regulation** | Pointer to [**CalculateSmsPriceDataSummaryCountriesInnerCountryRegulation**](CalculateSmsPriceDataSummaryCountriesInnerCountryRegulation.md) |  | [optional] 
**RegistrationStatusId** | Pointer to **int32** | Your current registration status for this country. This parameter is used by the internal team to track the status of your registration. | [optional] 
**RegistrationEntityId** | Pointer to **int32** | The global sending requirement for this country. It can be one of the following:  - **0:** No number or account registration required.      - **1:** Number registration required. You can purchase a registered number from ClickSend. Examples: US and CA.      - **2:** Account registration required. You can register your company details or business details to register your account. Examples: NZ, SG and UAE.    This parameter is a duplicate of registration_type. It determines which form you need for the global sending registration process.  &lt;div class&#x3D;\&quot;info-box\&quot;&gt;   &lt;h4&gt;&lt;i class&#x3D;\&quot;fas fa-info-circle\&quot;&gt;&lt;/i&gt; Note:&lt;/h4&gt;   &lt;p&gt;This parameter is static. Its value can’t change based on your settings.&lt;/p&gt; &lt;/div&gt; | [optional] 
**JotformId** | Pointer to **int32** | The Jotform identifier for your account. It’s used to track the global sending registration form. If it is **null**, no Jotform is assigned to you. It is used only for number and account registration. | [optional] 

## Methods

### NewCalculateSmsPriceDataSummaryCountriesInnerCountry

`func NewCalculateSmsPriceDataSummaryCountriesInnerCountry() *CalculateSmsPriceDataSummaryCountriesInnerCountry`

NewCalculateSmsPriceDataSummaryCountriesInnerCountry instantiates a new CalculateSmsPriceDataSummaryCountriesInnerCountry object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewCalculateSmsPriceDataSummaryCountriesInnerCountryWithDefaults

`func NewCalculateSmsPriceDataSummaryCountriesInnerCountryWithDefaults() *CalculateSmsPriceDataSummaryCountriesInnerCountry`

NewCalculateSmsPriceDataSummaryCountriesInnerCountryWithDefaults instantiates a new CalculateSmsPriceDataSummaryCountriesInnerCountry object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetRegistrationType

`func (o *CalculateSmsPriceDataSummaryCountriesInnerCountry) GetRegistrationType() int32`

GetRegistrationType returns the RegistrationType field if non-nil, zero value otherwise.

### GetRegistrationTypeOk

`func (o *CalculateSmsPriceDataSummaryCountriesInnerCountry) GetRegistrationTypeOk() (*int32, bool)`

GetRegistrationTypeOk returns a tuple with the RegistrationType field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetRegistrationType

`func (o *CalculateSmsPriceDataSummaryCountriesInnerCountry) SetRegistrationType(v int32)`

SetRegistrationType sets RegistrationType field to given value.

### HasRegistrationType

`func (o *CalculateSmsPriceDataSummaryCountriesInnerCountry) HasRegistrationType() bool`

HasRegistrationType returns a boolean if a field has been set.

### GetReceipientCount

`func (o *CalculateSmsPriceDataSummaryCountriesInnerCountry) GetReceipientCount() int32`

GetReceipientCount returns the ReceipientCount field if non-nil, zero value otherwise.

### GetReceipientCountOk

`func (o *CalculateSmsPriceDataSummaryCountriesInnerCountry) GetReceipientCountOk() (*int32, bool)`

GetReceipientCountOk returns a tuple with the ReceipientCount field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetReceipientCount

`func (o *CalculateSmsPriceDataSummaryCountriesInnerCountry) SetReceipientCount(v int32)`

SetReceipientCount sets ReceipientCount field to given value.

### HasReceipientCount

`func (o *CalculateSmsPriceDataSummaryCountriesInnerCountry) HasReceipientCount() bool`

HasReceipientCount returns a boolean if a field has been set.

### GetUsableSenderId

`func (o *CalculateSmsPriceDataSummaryCountriesInnerCountry) GetUsableSenderId() bool`

GetUsableSenderId returns the UsableSenderId field if non-nil, zero value otherwise.

### GetUsableSenderIdOk

`func (o *CalculateSmsPriceDataSummaryCountriesInnerCountry) GetUsableSenderIdOk() (*bool, bool)`

GetUsableSenderIdOk returns a tuple with the UsableSenderId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetUsableSenderId

`func (o *CalculateSmsPriceDataSummaryCountriesInnerCountry) SetUsableSenderId(v bool)`

SetUsableSenderId sets UsableSenderId field to given value.

### HasUsableSenderId

`func (o *CalculateSmsPriceDataSummaryCountriesInnerCountry) HasUsableSenderId() bool`

HasUsableSenderId returns a boolean if a field has been set.

### GetSelected

`func (o *CalculateSmsPriceDataSummaryCountriesInnerCountry) GetSelected() bool`

GetSelected returns the Selected field if non-nil, zero value otherwise.

### GetSelectedOk

`func (o *CalculateSmsPriceDataSummaryCountriesInnerCountry) GetSelectedOk() (*bool, bool)`

GetSelectedOk returns a tuple with the Selected field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSelected

`func (o *CalculateSmsPriceDataSummaryCountriesInnerCountry) SetSelected(v bool)`

SetSelected sets Selected field to given value.

### HasSelected

`func (o *CalculateSmsPriceDataSummaryCountriesInnerCountry) HasSelected() bool`

HasSelected returns a boolean if a field has been set.

### GetName

`func (o *CalculateSmsPriceDataSummaryCountriesInnerCountry) GetName() string`

GetName returns the Name field if non-nil, zero value otherwise.

### GetNameOk

`func (o *CalculateSmsPriceDataSummaryCountriesInnerCountry) GetNameOk() (*string, bool)`

GetNameOk returns a tuple with the Name field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetName

`func (o *CalculateSmsPriceDataSummaryCountriesInnerCountry) SetName(v string)`

SetName sets Name field to given value.

### HasName

`func (o *CalculateSmsPriceDataSummaryCountriesInnerCountry) HasName() bool`

HasName returns a boolean if a field has been set.

### GetRegulation

`func (o *CalculateSmsPriceDataSummaryCountriesInnerCountry) GetRegulation() CalculateSmsPriceDataSummaryCountriesInnerCountryRegulation`

GetRegulation returns the Regulation field if non-nil, zero value otherwise.

### GetRegulationOk

`func (o *CalculateSmsPriceDataSummaryCountriesInnerCountry) GetRegulationOk() (*CalculateSmsPriceDataSummaryCountriesInnerCountryRegulation, bool)`

GetRegulationOk returns a tuple with the Regulation field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetRegulation

`func (o *CalculateSmsPriceDataSummaryCountriesInnerCountry) SetRegulation(v CalculateSmsPriceDataSummaryCountriesInnerCountryRegulation)`

SetRegulation sets Regulation field to given value.

### HasRegulation

`func (o *CalculateSmsPriceDataSummaryCountriesInnerCountry) HasRegulation() bool`

HasRegulation returns a boolean if a field has been set.

### GetRegistrationStatusId

`func (o *CalculateSmsPriceDataSummaryCountriesInnerCountry) GetRegistrationStatusId() int32`

GetRegistrationStatusId returns the RegistrationStatusId field if non-nil, zero value otherwise.

### GetRegistrationStatusIdOk

`func (o *CalculateSmsPriceDataSummaryCountriesInnerCountry) GetRegistrationStatusIdOk() (*int32, bool)`

GetRegistrationStatusIdOk returns a tuple with the RegistrationStatusId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetRegistrationStatusId

`func (o *CalculateSmsPriceDataSummaryCountriesInnerCountry) SetRegistrationStatusId(v int32)`

SetRegistrationStatusId sets RegistrationStatusId field to given value.

### HasRegistrationStatusId

`func (o *CalculateSmsPriceDataSummaryCountriesInnerCountry) HasRegistrationStatusId() bool`

HasRegistrationStatusId returns a boolean if a field has been set.

### GetRegistrationEntityId

`func (o *CalculateSmsPriceDataSummaryCountriesInnerCountry) GetRegistrationEntityId() int32`

GetRegistrationEntityId returns the RegistrationEntityId field if non-nil, zero value otherwise.

### GetRegistrationEntityIdOk

`func (o *CalculateSmsPriceDataSummaryCountriesInnerCountry) GetRegistrationEntityIdOk() (*int32, bool)`

GetRegistrationEntityIdOk returns a tuple with the RegistrationEntityId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetRegistrationEntityId

`func (o *CalculateSmsPriceDataSummaryCountriesInnerCountry) SetRegistrationEntityId(v int32)`

SetRegistrationEntityId sets RegistrationEntityId field to given value.

### HasRegistrationEntityId

`func (o *CalculateSmsPriceDataSummaryCountriesInnerCountry) HasRegistrationEntityId() bool`

HasRegistrationEntityId returns a boolean if a field has been set.

### GetJotformId

`func (o *CalculateSmsPriceDataSummaryCountriesInnerCountry) GetJotformId() int32`

GetJotformId returns the JotformId field if non-nil, zero value otherwise.

### GetJotformIdOk

`func (o *CalculateSmsPriceDataSummaryCountriesInnerCountry) GetJotformIdOk() (*int32, bool)`

GetJotformIdOk returns a tuple with the JotformId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetJotformId

`func (o *CalculateSmsPriceDataSummaryCountriesInnerCountry) SetJotformId(v int32)`

SetJotformId sets JotformId field to given value.

### HasJotformId

`func (o *CalculateSmsPriceDataSummaryCountriesInnerCountry) HasJotformId() bool`

HasJotformId returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


