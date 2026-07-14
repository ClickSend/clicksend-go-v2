# ViewAllowedEmailsDataAllOfDataInner

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**EmailAddressId** | Pointer to **float32** | The ID of the email address. | [optional] 
**EmailAddress** | Pointer to **string** | The email address. | [optional] 
**From** | Pointer to **string** | The sender. | [optional] 
**SubaccountId** | Pointer to **int32** | The ID of the subaccount that owns this email address. | [optional] 
**FromFax** | Pointer to **NullableString** | The fax number used as the sender, if applicable. | [optional] 
**Voice** | Pointer to **string** | The voice used when this email address triggers a voice message. | [optional] 
**Lang** | Pointer to **string** | The language used when this email address triggers a voice message. | [optional] 
**SubaccountName** | Pointer to **string** | The name of the subaccount that owns this email address. | [optional] 

## Methods

### NewViewAllowedEmailsDataAllOfDataInner

`func NewViewAllowedEmailsDataAllOfDataInner() *ViewAllowedEmailsDataAllOfDataInner`

NewViewAllowedEmailsDataAllOfDataInner instantiates a new ViewAllowedEmailsDataAllOfDataInner object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewViewAllowedEmailsDataAllOfDataInnerWithDefaults

`func NewViewAllowedEmailsDataAllOfDataInnerWithDefaults() *ViewAllowedEmailsDataAllOfDataInner`

NewViewAllowedEmailsDataAllOfDataInnerWithDefaults instantiates a new ViewAllowedEmailsDataAllOfDataInner object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetEmailAddressId

`func (o *ViewAllowedEmailsDataAllOfDataInner) GetEmailAddressId() float32`

GetEmailAddressId returns the EmailAddressId field if non-nil, zero value otherwise.

### GetEmailAddressIdOk

`func (o *ViewAllowedEmailsDataAllOfDataInner) GetEmailAddressIdOk() (*float32, bool)`

GetEmailAddressIdOk returns a tuple with the EmailAddressId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetEmailAddressId

`func (o *ViewAllowedEmailsDataAllOfDataInner) SetEmailAddressId(v float32)`

SetEmailAddressId sets EmailAddressId field to given value.

### HasEmailAddressId

`func (o *ViewAllowedEmailsDataAllOfDataInner) HasEmailAddressId() bool`

HasEmailAddressId returns a boolean if a field has been set.

### GetEmailAddress

`func (o *ViewAllowedEmailsDataAllOfDataInner) GetEmailAddress() string`

GetEmailAddress returns the EmailAddress field if non-nil, zero value otherwise.

### GetEmailAddressOk

`func (o *ViewAllowedEmailsDataAllOfDataInner) GetEmailAddressOk() (*string, bool)`

GetEmailAddressOk returns a tuple with the EmailAddress field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetEmailAddress

`func (o *ViewAllowedEmailsDataAllOfDataInner) SetEmailAddress(v string)`

SetEmailAddress sets EmailAddress field to given value.

### HasEmailAddress

`func (o *ViewAllowedEmailsDataAllOfDataInner) HasEmailAddress() bool`

HasEmailAddress returns a boolean if a field has been set.

### GetFrom

`func (o *ViewAllowedEmailsDataAllOfDataInner) GetFrom() string`

GetFrom returns the From field if non-nil, zero value otherwise.

### GetFromOk

`func (o *ViewAllowedEmailsDataAllOfDataInner) GetFromOk() (*string, bool)`

GetFromOk returns a tuple with the From field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetFrom

`func (o *ViewAllowedEmailsDataAllOfDataInner) SetFrom(v string)`

SetFrom sets From field to given value.

### HasFrom

`func (o *ViewAllowedEmailsDataAllOfDataInner) HasFrom() bool`

HasFrom returns a boolean if a field has been set.

### GetSubaccountId

`func (o *ViewAllowedEmailsDataAllOfDataInner) GetSubaccountId() int32`

GetSubaccountId returns the SubaccountId field if non-nil, zero value otherwise.

### GetSubaccountIdOk

`func (o *ViewAllowedEmailsDataAllOfDataInner) GetSubaccountIdOk() (*int32, bool)`

GetSubaccountIdOk returns a tuple with the SubaccountId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSubaccountId

`func (o *ViewAllowedEmailsDataAllOfDataInner) SetSubaccountId(v int32)`

SetSubaccountId sets SubaccountId field to given value.

### HasSubaccountId

`func (o *ViewAllowedEmailsDataAllOfDataInner) HasSubaccountId() bool`

HasSubaccountId returns a boolean if a field has been set.

### GetFromFax

`func (o *ViewAllowedEmailsDataAllOfDataInner) GetFromFax() string`

GetFromFax returns the FromFax field if non-nil, zero value otherwise.

### GetFromFaxOk

`func (o *ViewAllowedEmailsDataAllOfDataInner) GetFromFaxOk() (*string, bool)`

GetFromFaxOk returns a tuple with the FromFax field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetFromFax

`func (o *ViewAllowedEmailsDataAllOfDataInner) SetFromFax(v string)`

SetFromFax sets FromFax field to given value.

### HasFromFax

`func (o *ViewAllowedEmailsDataAllOfDataInner) HasFromFax() bool`

HasFromFax returns a boolean if a field has been set.

### SetFromFaxNil

`func (o *ViewAllowedEmailsDataAllOfDataInner) SetFromFaxNil(b bool)`

 SetFromFaxNil sets the value for FromFax to be an explicit nil

### UnsetFromFax
`func (o *ViewAllowedEmailsDataAllOfDataInner) UnsetFromFax()`

UnsetFromFax ensures that no value is present for FromFax, not even an explicit nil
### GetVoice

`func (o *ViewAllowedEmailsDataAllOfDataInner) GetVoice() string`

GetVoice returns the Voice field if non-nil, zero value otherwise.

### GetVoiceOk

`func (o *ViewAllowedEmailsDataAllOfDataInner) GetVoiceOk() (*string, bool)`

GetVoiceOk returns a tuple with the Voice field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetVoice

`func (o *ViewAllowedEmailsDataAllOfDataInner) SetVoice(v string)`

SetVoice sets Voice field to given value.

### HasVoice

`func (o *ViewAllowedEmailsDataAllOfDataInner) HasVoice() bool`

HasVoice returns a boolean if a field has been set.

### GetLang

`func (o *ViewAllowedEmailsDataAllOfDataInner) GetLang() string`

GetLang returns the Lang field if non-nil, zero value otherwise.

### GetLangOk

`func (o *ViewAllowedEmailsDataAllOfDataInner) GetLangOk() (*string, bool)`

GetLangOk returns a tuple with the Lang field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetLang

`func (o *ViewAllowedEmailsDataAllOfDataInner) SetLang(v string)`

SetLang sets Lang field to given value.

### HasLang

`func (o *ViewAllowedEmailsDataAllOfDataInner) HasLang() bool`

HasLang returns a boolean if a field has been set.

### GetSubaccountName

`func (o *ViewAllowedEmailsDataAllOfDataInner) GetSubaccountName() string`

GetSubaccountName returns the SubaccountName field if non-nil, zero value otherwise.

### GetSubaccountNameOk

`func (o *ViewAllowedEmailsDataAllOfDataInner) GetSubaccountNameOk() (*string, bool)`

GetSubaccountNameOk returns a tuple with the SubaccountName field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSubaccountName

`func (o *ViewAllowedEmailsDataAllOfDataInner) SetSubaccountName(v string)`

SetSubaccountName sets SubaccountName field to given value.

### HasSubaccountName

`func (o *ViewAllowedEmailsDataAllOfDataInner) HasSubaccountName() bool`

HasSubaccountName returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


