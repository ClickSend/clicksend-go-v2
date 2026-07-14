# Subaccount

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**SubaccountId** | Pointer to **int32** | The unique identifier for the subaccount. | [optional] 
**ApiUsername** | Pointer to **string** | The API username of the subaccount. | [optional] 
**Email** | Pointer to **string** | The email address of the subaccount. | [optional] 
**PhoneNumber** | Pointer to **string** | The phone number of the subaccount. | [optional] 
**FirstName** | Pointer to **string** | The first name of the subaccount. | [optional] 
**LastName** | Pointer to **string** | The last name of the subaccount. | [optional] 
**ApiKey** | Pointer to **string** | The API key of the subaccount. | [optional] 
**AccessSmpp** | Pointer to **int32** | Flag indicating if the subaccount has access to SMPP. | [optional] 
**AccessUsers** | Pointer to **int32** | Flag indicating if the subaccount has access to users. | [optional] 
**AccessBilling** | Pointer to **int32** | Flag indicating if the subaccount has access to billing. | [optional] 
**AccessReporting** | Pointer to **int32** | Flag indicating if the subaccount has access to reporting. | [optional] 
**AccessContacts** | Pointer to **int32** | Flag indicating if the subaccount has access to contacts. | [optional] 
**AccessSettings** | Pointer to **int32** | Flag indicating if the subaccount has access to settings. | [optional] 
**AccessSms** | Pointer to **int32** | Flag indicating if the subaccount has access to SMS. | [optional] 
**AccessEmail** | Pointer to **int32** | Flag indicating if the subaccount has access to email. | [optional] 
**AccessVoice** | Pointer to **int32** | Flag indicating if the subaccount has access to voice services. | [optional] 
**AccessFax** | Pointer to **int32** | Flag indicating if the subaccount has access to fax services. | [optional] 
**AccessPost** | Pointer to **int32** | Flag indicating if the subaccount has access to post services. | [optional] 
**AccessReseller** | Pointer to **int32** | Flag indicating if the subaccount has access to reseller services. | [optional] 
**AccessGlobalSending** | Pointer to **int32** | Flag indicating if the subaccount has access to global sending. | [optional] 
**AccessMms** | Pointer to **int32** | Flag indicating if the subaccount has access to MMS services. | [optional] 
**HidePricing** | Pointer to **int32** | Flag indicating if pricing is hidden for the subaccount. | [optional] 
**ShareCampaigns** | Pointer to **int32** | Flag indicating if the subaccount can share campaigns. | [optional] 
**Notes** | Pointer to **NullableString** | Additional notes for the subaccount. | [optional] 
**IsMain** | Pointer to **int32** | Flag indicating if this is the main account rather than a subaccount. | [optional] 
**SignUpType** | Pointer to **NullableString** | The sign-up type used to create the subaccount, if applicable. | [optional] 

## Methods

### NewSubaccount

`func NewSubaccount() *Subaccount`

NewSubaccount instantiates a new Subaccount object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewSubaccountWithDefaults

`func NewSubaccountWithDefaults() *Subaccount`

NewSubaccountWithDefaults instantiates a new Subaccount object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetSubaccountId

`func (o *Subaccount) GetSubaccountId() int32`

GetSubaccountId returns the SubaccountId field if non-nil, zero value otherwise.

### GetSubaccountIdOk

`func (o *Subaccount) GetSubaccountIdOk() (*int32, bool)`

GetSubaccountIdOk returns a tuple with the SubaccountId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSubaccountId

`func (o *Subaccount) SetSubaccountId(v int32)`

SetSubaccountId sets SubaccountId field to given value.

### HasSubaccountId

`func (o *Subaccount) HasSubaccountId() bool`

HasSubaccountId returns a boolean if a field has been set.

### GetApiUsername

`func (o *Subaccount) GetApiUsername() string`

GetApiUsername returns the ApiUsername field if non-nil, zero value otherwise.

### GetApiUsernameOk

`func (o *Subaccount) GetApiUsernameOk() (*string, bool)`

GetApiUsernameOk returns a tuple with the ApiUsername field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetApiUsername

`func (o *Subaccount) SetApiUsername(v string)`

SetApiUsername sets ApiUsername field to given value.

### HasApiUsername

`func (o *Subaccount) HasApiUsername() bool`

HasApiUsername returns a boolean if a field has been set.

### GetEmail

`func (o *Subaccount) GetEmail() string`

GetEmail returns the Email field if non-nil, zero value otherwise.

### GetEmailOk

`func (o *Subaccount) GetEmailOk() (*string, bool)`

GetEmailOk returns a tuple with the Email field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetEmail

`func (o *Subaccount) SetEmail(v string)`

SetEmail sets Email field to given value.

### HasEmail

`func (o *Subaccount) HasEmail() bool`

HasEmail returns a boolean if a field has been set.

### GetPhoneNumber

`func (o *Subaccount) GetPhoneNumber() string`

GetPhoneNumber returns the PhoneNumber field if non-nil, zero value otherwise.

### GetPhoneNumberOk

`func (o *Subaccount) GetPhoneNumberOk() (*string, bool)`

GetPhoneNumberOk returns a tuple with the PhoneNumber field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetPhoneNumber

`func (o *Subaccount) SetPhoneNumber(v string)`

SetPhoneNumber sets PhoneNumber field to given value.

### HasPhoneNumber

`func (o *Subaccount) HasPhoneNumber() bool`

HasPhoneNumber returns a boolean if a field has been set.

### GetFirstName

`func (o *Subaccount) GetFirstName() string`

GetFirstName returns the FirstName field if non-nil, zero value otherwise.

### GetFirstNameOk

`func (o *Subaccount) GetFirstNameOk() (*string, bool)`

GetFirstNameOk returns a tuple with the FirstName field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetFirstName

`func (o *Subaccount) SetFirstName(v string)`

SetFirstName sets FirstName field to given value.

### HasFirstName

`func (o *Subaccount) HasFirstName() bool`

HasFirstName returns a boolean if a field has been set.

### GetLastName

`func (o *Subaccount) GetLastName() string`

GetLastName returns the LastName field if non-nil, zero value otherwise.

### GetLastNameOk

`func (o *Subaccount) GetLastNameOk() (*string, bool)`

GetLastNameOk returns a tuple with the LastName field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetLastName

`func (o *Subaccount) SetLastName(v string)`

SetLastName sets LastName field to given value.

### HasLastName

`func (o *Subaccount) HasLastName() bool`

HasLastName returns a boolean if a field has been set.

### GetApiKey

`func (o *Subaccount) GetApiKey() string`

GetApiKey returns the ApiKey field if non-nil, zero value otherwise.

### GetApiKeyOk

`func (o *Subaccount) GetApiKeyOk() (*string, bool)`

GetApiKeyOk returns a tuple with the ApiKey field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetApiKey

`func (o *Subaccount) SetApiKey(v string)`

SetApiKey sets ApiKey field to given value.

### HasApiKey

`func (o *Subaccount) HasApiKey() bool`

HasApiKey returns a boolean if a field has been set.

### GetAccessSmpp

`func (o *Subaccount) GetAccessSmpp() int32`

GetAccessSmpp returns the AccessSmpp field if non-nil, zero value otherwise.

### GetAccessSmppOk

`func (o *Subaccount) GetAccessSmppOk() (*int32, bool)`

GetAccessSmppOk returns a tuple with the AccessSmpp field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAccessSmpp

`func (o *Subaccount) SetAccessSmpp(v int32)`

SetAccessSmpp sets AccessSmpp field to given value.

### HasAccessSmpp

`func (o *Subaccount) HasAccessSmpp() bool`

HasAccessSmpp returns a boolean if a field has been set.

### GetAccessUsers

`func (o *Subaccount) GetAccessUsers() int32`

GetAccessUsers returns the AccessUsers field if non-nil, zero value otherwise.

### GetAccessUsersOk

`func (o *Subaccount) GetAccessUsersOk() (*int32, bool)`

GetAccessUsersOk returns a tuple with the AccessUsers field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAccessUsers

`func (o *Subaccount) SetAccessUsers(v int32)`

SetAccessUsers sets AccessUsers field to given value.

### HasAccessUsers

`func (o *Subaccount) HasAccessUsers() bool`

HasAccessUsers returns a boolean if a field has been set.

### GetAccessBilling

`func (o *Subaccount) GetAccessBilling() int32`

GetAccessBilling returns the AccessBilling field if non-nil, zero value otherwise.

### GetAccessBillingOk

`func (o *Subaccount) GetAccessBillingOk() (*int32, bool)`

GetAccessBillingOk returns a tuple with the AccessBilling field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAccessBilling

`func (o *Subaccount) SetAccessBilling(v int32)`

SetAccessBilling sets AccessBilling field to given value.

### HasAccessBilling

`func (o *Subaccount) HasAccessBilling() bool`

HasAccessBilling returns a boolean if a field has been set.

### GetAccessReporting

`func (o *Subaccount) GetAccessReporting() int32`

GetAccessReporting returns the AccessReporting field if non-nil, zero value otherwise.

### GetAccessReportingOk

`func (o *Subaccount) GetAccessReportingOk() (*int32, bool)`

GetAccessReportingOk returns a tuple with the AccessReporting field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAccessReporting

`func (o *Subaccount) SetAccessReporting(v int32)`

SetAccessReporting sets AccessReporting field to given value.

### HasAccessReporting

`func (o *Subaccount) HasAccessReporting() bool`

HasAccessReporting returns a boolean if a field has been set.

### GetAccessContacts

`func (o *Subaccount) GetAccessContacts() int32`

GetAccessContacts returns the AccessContacts field if non-nil, zero value otherwise.

### GetAccessContactsOk

`func (o *Subaccount) GetAccessContactsOk() (*int32, bool)`

GetAccessContactsOk returns a tuple with the AccessContacts field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAccessContacts

`func (o *Subaccount) SetAccessContacts(v int32)`

SetAccessContacts sets AccessContacts field to given value.

### HasAccessContacts

`func (o *Subaccount) HasAccessContacts() bool`

HasAccessContacts returns a boolean if a field has been set.

### GetAccessSettings

`func (o *Subaccount) GetAccessSettings() int32`

GetAccessSettings returns the AccessSettings field if non-nil, zero value otherwise.

### GetAccessSettingsOk

`func (o *Subaccount) GetAccessSettingsOk() (*int32, bool)`

GetAccessSettingsOk returns a tuple with the AccessSettings field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAccessSettings

`func (o *Subaccount) SetAccessSettings(v int32)`

SetAccessSettings sets AccessSettings field to given value.

### HasAccessSettings

`func (o *Subaccount) HasAccessSettings() bool`

HasAccessSettings returns a boolean if a field has been set.

### GetAccessSms

`func (o *Subaccount) GetAccessSms() int32`

GetAccessSms returns the AccessSms field if non-nil, zero value otherwise.

### GetAccessSmsOk

`func (o *Subaccount) GetAccessSmsOk() (*int32, bool)`

GetAccessSmsOk returns a tuple with the AccessSms field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAccessSms

`func (o *Subaccount) SetAccessSms(v int32)`

SetAccessSms sets AccessSms field to given value.

### HasAccessSms

`func (o *Subaccount) HasAccessSms() bool`

HasAccessSms returns a boolean if a field has been set.

### GetAccessEmail

`func (o *Subaccount) GetAccessEmail() int32`

GetAccessEmail returns the AccessEmail field if non-nil, zero value otherwise.

### GetAccessEmailOk

`func (o *Subaccount) GetAccessEmailOk() (*int32, bool)`

GetAccessEmailOk returns a tuple with the AccessEmail field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAccessEmail

`func (o *Subaccount) SetAccessEmail(v int32)`

SetAccessEmail sets AccessEmail field to given value.

### HasAccessEmail

`func (o *Subaccount) HasAccessEmail() bool`

HasAccessEmail returns a boolean if a field has been set.

### GetAccessVoice

`func (o *Subaccount) GetAccessVoice() int32`

GetAccessVoice returns the AccessVoice field if non-nil, zero value otherwise.

### GetAccessVoiceOk

`func (o *Subaccount) GetAccessVoiceOk() (*int32, bool)`

GetAccessVoiceOk returns a tuple with the AccessVoice field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAccessVoice

`func (o *Subaccount) SetAccessVoice(v int32)`

SetAccessVoice sets AccessVoice field to given value.

### HasAccessVoice

`func (o *Subaccount) HasAccessVoice() bool`

HasAccessVoice returns a boolean if a field has been set.

### GetAccessFax

`func (o *Subaccount) GetAccessFax() int32`

GetAccessFax returns the AccessFax field if non-nil, zero value otherwise.

### GetAccessFaxOk

`func (o *Subaccount) GetAccessFaxOk() (*int32, bool)`

GetAccessFaxOk returns a tuple with the AccessFax field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAccessFax

`func (o *Subaccount) SetAccessFax(v int32)`

SetAccessFax sets AccessFax field to given value.

### HasAccessFax

`func (o *Subaccount) HasAccessFax() bool`

HasAccessFax returns a boolean if a field has been set.

### GetAccessPost

`func (o *Subaccount) GetAccessPost() int32`

GetAccessPost returns the AccessPost field if non-nil, zero value otherwise.

### GetAccessPostOk

`func (o *Subaccount) GetAccessPostOk() (*int32, bool)`

GetAccessPostOk returns a tuple with the AccessPost field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAccessPost

`func (o *Subaccount) SetAccessPost(v int32)`

SetAccessPost sets AccessPost field to given value.

### HasAccessPost

`func (o *Subaccount) HasAccessPost() bool`

HasAccessPost returns a boolean if a field has been set.

### GetAccessReseller

`func (o *Subaccount) GetAccessReseller() int32`

GetAccessReseller returns the AccessReseller field if non-nil, zero value otherwise.

### GetAccessResellerOk

`func (o *Subaccount) GetAccessResellerOk() (*int32, bool)`

GetAccessResellerOk returns a tuple with the AccessReseller field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAccessReseller

`func (o *Subaccount) SetAccessReseller(v int32)`

SetAccessReseller sets AccessReseller field to given value.

### HasAccessReseller

`func (o *Subaccount) HasAccessReseller() bool`

HasAccessReseller returns a boolean if a field has been set.

### GetAccessGlobalSending

`func (o *Subaccount) GetAccessGlobalSending() int32`

GetAccessGlobalSending returns the AccessGlobalSending field if non-nil, zero value otherwise.

### GetAccessGlobalSendingOk

`func (o *Subaccount) GetAccessGlobalSendingOk() (*int32, bool)`

GetAccessGlobalSendingOk returns a tuple with the AccessGlobalSending field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAccessGlobalSending

`func (o *Subaccount) SetAccessGlobalSending(v int32)`

SetAccessGlobalSending sets AccessGlobalSending field to given value.

### HasAccessGlobalSending

`func (o *Subaccount) HasAccessGlobalSending() bool`

HasAccessGlobalSending returns a boolean if a field has been set.

### GetAccessMms

`func (o *Subaccount) GetAccessMms() int32`

GetAccessMms returns the AccessMms field if non-nil, zero value otherwise.

### GetAccessMmsOk

`func (o *Subaccount) GetAccessMmsOk() (*int32, bool)`

GetAccessMmsOk returns a tuple with the AccessMms field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAccessMms

`func (o *Subaccount) SetAccessMms(v int32)`

SetAccessMms sets AccessMms field to given value.

### HasAccessMms

`func (o *Subaccount) HasAccessMms() bool`

HasAccessMms returns a boolean if a field has been set.

### GetHidePricing

`func (o *Subaccount) GetHidePricing() int32`

GetHidePricing returns the HidePricing field if non-nil, zero value otherwise.

### GetHidePricingOk

`func (o *Subaccount) GetHidePricingOk() (*int32, bool)`

GetHidePricingOk returns a tuple with the HidePricing field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetHidePricing

`func (o *Subaccount) SetHidePricing(v int32)`

SetHidePricing sets HidePricing field to given value.

### HasHidePricing

`func (o *Subaccount) HasHidePricing() bool`

HasHidePricing returns a boolean if a field has been set.

### GetShareCampaigns

`func (o *Subaccount) GetShareCampaigns() int32`

GetShareCampaigns returns the ShareCampaigns field if non-nil, zero value otherwise.

### GetShareCampaignsOk

`func (o *Subaccount) GetShareCampaignsOk() (*int32, bool)`

GetShareCampaignsOk returns a tuple with the ShareCampaigns field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetShareCampaigns

`func (o *Subaccount) SetShareCampaigns(v int32)`

SetShareCampaigns sets ShareCampaigns field to given value.

### HasShareCampaigns

`func (o *Subaccount) HasShareCampaigns() bool`

HasShareCampaigns returns a boolean if a field has been set.

### GetNotes

`func (o *Subaccount) GetNotes() string`

GetNotes returns the Notes field if non-nil, zero value otherwise.

### GetNotesOk

`func (o *Subaccount) GetNotesOk() (*string, bool)`

GetNotesOk returns a tuple with the Notes field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetNotes

`func (o *Subaccount) SetNotes(v string)`

SetNotes sets Notes field to given value.

### HasNotes

`func (o *Subaccount) HasNotes() bool`

HasNotes returns a boolean if a field has been set.

### SetNotesNil

`func (o *Subaccount) SetNotesNil(b bool)`

 SetNotesNil sets the value for Notes to be an explicit nil

### UnsetNotes
`func (o *Subaccount) UnsetNotes()`

UnsetNotes ensures that no value is present for Notes, not even an explicit nil
### GetIsMain

`func (o *Subaccount) GetIsMain() int32`

GetIsMain returns the IsMain field if non-nil, zero value otherwise.

### GetIsMainOk

`func (o *Subaccount) GetIsMainOk() (*int32, bool)`

GetIsMainOk returns a tuple with the IsMain field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetIsMain

`func (o *Subaccount) SetIsMain(v int32)`

SetIsMain sets IsMain field to given value.

### HasIsMain

`func (o *Subaccount) HasIsMain() bool`

HasIsMain returns a boolean if a field has been set.

### GetSignUpType

`func (o *Subaccount) GetSignUpType() string`

GetSignUpType returns the SignUpType field if non-nil, zero value otherwise.

### GetSignUpTypeOk

`func (o *Subaccount) GetSignUpTypeOk() (*string, bool)`

GetSignUpTypeOk returns a tuple with the SignUpType field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSignUpType

`func (o *Subaccount) SetSignUpType(v string)`

SetSignUpType sets SignUpType field to given value.

### HasSignUpType

`func (o *Subaccount) HasSignUpType() bool`

HasSignUpType returns a boolean if a field has been set.

### SetSignUpTypeNil

`func (o *Subaccount) SetSignUpTypeNil(b bool)`

 SetSignUpTypeNil sets the value for SignUpType to be an explicit nil

### UnsetSignUpType
`func (o *Subaccount) UnsetSignUpType()`

UnsetSignUpType ensures that no value is present for SignUpType, not even an explicit nil

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


