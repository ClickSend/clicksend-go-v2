# ResellerAccount

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**UserId** | Pointer to **int32** | The user&#39;s ID | [optional] 
**Username** | Pointer to **string** | The username | [optional] 
**UserEmail** | Pointer to **string** | The user&#39;s email | [optional] 
**Active** | Pointer to **int32** | Indicates if the user is active | [optional] 
**Banned** | Pointer to **int32** | Indicates if the user is banned | [optional] 
**Balance** | Pointer to **string** | The user&#39;s balance | [optional] 
**UserPhone** | Pointer to **string** | The user&#39;s phone number | [optional] 
**ReplyTo** | Pointer to **string** | The reply-to email address | [optional] 
**DeliveryTo** | Pointer to **NullableString** | The delivery-to email address | [optional] 
**UserFirstName** | Pointer to **string** | The user&#39;s first name | [optional] 
**UserLastName** | Pointer to **string** | The user&#39;s last name | [optional] 
**Account** | Pointer to **int32** | The user&#39;s account number | [optional] 
**AccountName** | Pointer to **string** | The name of the user&#39;s account | [optional] 
**AccountBillingEmail** | Pointer to **string** | The account billing email | [optional] 
**AccountBillingMobile** | Pointer to **string** | The account billing mobile number | [optional] 
**Country** | Pointer to **string** | The user&#39;s country | [optional] 
**DefaultCountrySms** | Pointer to **string** | The default country for SMS | [optional] 
**AutoRecharge** | Pointer to **int32** | Indicates if auto-recharge is enabled | [optional] 
**AutoRechargeAmount** | Pointer to **string** | The auto-recharge amount | [optional] 
**LowCreditAmount** | Pointer to **string** | The low credit amount | [optional] 
**SettingUnicodeSms** | Pointer to **int32** | Setting for Unicode SMS | [optional] 
**SettingEmailSmsSubject** | Pointer to **int32** | Setting for email SMS subject | [optional] 
**SettingFixSenderId** | Pointer to **int32** | Setting for fixed sender ID | [optional] 
**SettingSmsMessageCharLimit** | Pointer to **int32** | Setting for SMS message character limit | [optional] 
**OldDashboard** | Pointer to **int32** | Indicates if the user is using the old dashboard | [optional] 
**BalanceCommission** | Pointer to **string** | The balance commission | [optional] 
**Timezone** | Pointer to **string** | The user&#39;s timezone | [optional] 

## Methods

### NewResellerAccount

`func NewResellerAccount() *ResellerAccount`

NewResellerAccount instantiates a new ResellerAccount object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewResellerAccountWithDefaults

`func NewResellerAccountWithDefaults() *ResellerAccount`

NewResellerAccountWithDefaults instantiates a new ResellerAccount object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetUserId

`func (o *ResellerAccount) GetUserId() int32`

GetUserId returns the UserId field if non-nil, zero value otherwise.

### GetUserIdOk

`func (o *ResellerAccount) GetUserIdOk() (*int32, bool)`

GetUserIdOk returns a tuple with the UserId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetUserId

`func (o *ResellerAccount) SetUserId(v int32)`

SetUserId sets UserId field to given value.

### HasUserId

`func (o *ResellerAccount) HasUserId() bool`

HasUserId returns a boolean if a field has been set.

### GetUsername

`func (o *ResellerAccount) GetUsername() string`

GetUsername returns the Username field if non-nil, zero value otherwise.

### GetUsernameOk

`func (o *ResellerAccount) GetUsernameOk() (*string, bool)`

GetUsernameOk returns a tuple with the Username field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetUsername

`func (o *ResellerAccount) SetUsername(v string)`

SetUsername sets Username field to given value.

### HasUsername

`func (o *ResellerAccount) HasUsername() bool`

HasUsername returns a boolean if a field has been set.

### GetUserEmail

`func (o *ResellerAccount) GetUserEmail() string`

GetUserEmail returns the UserEmail field if non-nil, zero value otherwise.

### GetUserEmailOk

`func (o *ResellerAccount) GetUserEmailOk() (*string, bool)`

GetUserEmailOk returns a tuple with the UserEmail field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetUserEmail

`func (o *ResellerAccount) SetUserEmail(v string)`

SetUserEmail sets UserEmail field to given value.

### HasUserEmail

`func (o *ResellerAccount) HasUserEmail() bool`

HasUserEmail returns a boolean if a field has been set.

### GetActive

`func (o *ResellerAccount) GetActive() int32`

GetActive returns the Active field if non-nil, zero value otherwise.

### GetActiveOk

`func (o *ResellerAccount) GetActiveOk() (*int32, bool)`

GetActiveOk returns a tuple with the Active field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetActive

`func (o *ResellerAccount) SetActive(v int32)`

SetActive sets Active field to given value.

### HasActive

`func (o *ResellerAccount) HasActive() bool`

HasActive returns a boolean if a field has been set.

### GetBanned

`func (o *ResellerAccount) GetBanned() int32`

GetBanned returns the Banned field if non-nil, zero value otherwise.

### GetBannedOk

`func (o *ResellerAccount) GetBannedOk() (*int32, bool)`

GetBannedOk returns a tuple with the Banned field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetBanned

`func (o *ResellerAccount) SetBanned(v int32)`

SetBanned sets Banned field to given value.

### HasBanned

`func (o *ResellerAccount) HasBanned() bool`

HasBanned returns a boolean if a field has been set.

### GetBalance

`func (o *ResellerAccount) GetBalance() string`

GetBalance returns the Balance field if non-nil, zero value otherwise.

### GetBalanceOk

`func (o *ResellerAccount) GetBalanceOk() (*string, bool)`

GetBalanceOk returns a tuple with the Balance field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetBalance

`func (o *ResellerAccount) SetBalance(v string)`

SetBalance sets Balance field to given value.

### HasBalance

`func (o *ResellerAccount) HasBalance() bool`

HasBalance returns a boolean if a field has been set.

### GetUserPhone

`func (o *ResellerAccount) GetUserPhone() string`

GetUserPhone returns the UserPhone field if non-nil, zero value otherwise.

### GetUserPhoneOk

`func (o *ResellerAccount) GetUserPhoneOk() (*string, bool)`

GetUserPhoneOk returns a tuple with the UserPhone field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetUserPhone

`func (o *ResellerAccount) SetUserPhone(v string)`

SetUserPhone sets UserPhone field to given value.

### HasUserPhone

`func (o *ResellerAccount) HasUserPhone() bool`

HasUserPhone returns a boolean if a field has been set.

### GetReplyTo

`func (o *ResellerAccount) GetReplyTo() string`

GetReplyTo returns the ReplyTo field if non-nil, zero value otherwise.

### GetReplyToOk

`func (o *ResellerAccount) GetReplyToOk() (*string, bool)`

GetReplyToOk returns a tuple with the ReplyTo field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetReplyTo

`func (o *ResellerAccount) SetReplyTo(v string)`

SetReplyTo sets ReplyTo field to given value.

### HasReplyTo

`func (o *ResellerAccount) HasReplyTo() bool`

HasReplyTo returns a boolean if a field has been set.

### GetDeliveryTo

`func (o *ResellerAccount) GetDeliveryTo() string`

GetDeliveryTo returns the DeliveryTo field if non-nil, zero value otherwise.

### GetDeliveryToOk

`func (o *ResellerAccount) GetDeliveryToOk() (*string, bool)`

GetDeliveryToOk returns a tuple with the DeliveryTo field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDeliveryTo

`func (o *ResellerAccount) SetDeliveryTo(v string)`

SetDeliveryTo sets DeliveryTo field to given value.

### HasDeliveryTo

`func (o *ResellerAccount) HasDeliveryTo() bool`

HasDeliveryTo returns a boolean if a field has been set.

### SetDeliveryToNil

`func (o *ResellerAccount) SetDeliveryToNil(b bool)`

 SetDeliveryToNil sets the value for DeliveryTo to be an explicit nil

### UnsetDeliveryTo
`func (o *ResellerAccount) UnsetDeliveryTo()`

UnsetDeliveryTo ensures that no value is present for DeliveryTo, not even an explicit nil
### GetUserFirstName

`func (o *ResellerAccount) GetUserFirstName() string`

GetUserFirstName returns the UserFirstName field if non-nil, zero value otherwise.

### GetUserFirstNameOk

`func (o *ResellerAccount) GetUserFirstNameOk() (*string, bool)`

GetUserFirstNameOk returns a tuple with the UserFirstName field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetUserFirstName

`func (o *ResellerAccount) SetUserFirstName(v string)`

SetUserFirstName sets UserFirstName field to given value.

### HasUserFirstName

`func (o *ResellerAccount) HasUserFirstName() bool`

HasUserFirstName returns a boolean if a field has been set.

### GetUserLastName

`func (o *ResellerAccount) GetUserLastName() string`

GetUserLastName returns the UserLastName field if non-nil, zero value otherwise.

### GetUserLastNameOk

`func (o *ResellerAccount) GetUserLastNameOk() (*string, bool)`

GetUserLastNameOk returns a tuple with the UserLastName field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetUserLastName

`func (o *ResellerAccount) SetUserLastName(v string)`

SetUserLastName sets UserLastName field to given value.

### HasUserLastName

`func (o *ResellerAccount) HasUserLastName() bool`

HasUserLastName returns a boolean if a field has been set.

### GetAccount

`func (o *ResellerAccount) GetAccount() int32`

GetAccount returns the Account field if non-nil, zero value otherwise.

### GetAccountOk

`func (o *ResellerAccount) GetAccountOk() (*int32, bool)`

GetAccountOk returns a tuple with the Account field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAccount

`func (o *ResellerAccount) SetAccount(v int32)`

SetAccount sets Account field to given value.

### HasAccount

`func (o *ResellerAccount) HasAccount() bool`

HasAccount returns a boolean if a field has been set.

### GetAccountName

`func (o *ResellerAccount) GetAccountName() string`

GetAccountName returns the AccountName field if non-nil, zero value otherwise.

### GetAccountNameOk

`func (o *ResellerAccount) GetAccountNameOk() (*string, bool)`

GetAccountNameOk returns a tuple with the AccountName field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAccountName

`func (o *ResellerAccount) SetAccountName(v string)`

SetAccountName sets AccountName field to given value.

### HasAccountName

`func (o *ResellerAccount) HasAccountName() bool`

HasAccountName returns a boolean if a field has been set.

### GetAccountBillingEmail

`func (o *ResellerAccount) GetAccountBillingEmail() string`

GetAccountBillingEmail returns the AccountBillingEmail field if non-nil, zero value otherwise.

### GetAccountBillingEmailOk

`func (o *ResellerAccount) GetAccountBillingEmailOk() (*string, bool)`

GetAccountBillingEmailOk returns a tuple with the AccountBillingEmail field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAccountBillingEmail

`func (o *ResellerAccount) SetAccountBillingEmail(v string)`

SetAccountBillingEmail sets AccountBillingEmail field to given value.

### HasAccountBillingEmail

`func (o *ResellerAccount) HasAccountBillingEmail() bool`

HasAccountBillingEmail returns a boolean if a field has been set.

### GetAccountBillingMobile

`func (o *ResellerAccount) GetAccountBillingMobile() string`

GetAccountBillingMobile returns the AccountBillingMobile field if non-nil, zero value otherwise.

### GetAccountBillingMobileOk

`func (o *ResellerAccount) GetAccountBillingMobileOk() (*string, bool)`

GetAccountBillingMobileOk returns a tuple with the AccountBillingMobile field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAccountBillingMobile

`func (o *ResellerAccount) SetAccountBillingMobile(v string)`

SetAccountBillingMobile sets AccountBillingMobile field to given value.

### HasAccountBillingMobile

`func (o *ResellerAccount) HasAccountBillingMobile() bool`

HasAccountBillingMobile returns a boolean if a field has been set.

### GetCountry

`func (o *ResellerAccount) GetCountry() string`

GetCountry returns the Country field if non-nil, zero value otherwise.

### GetCountryOk

`func (o *ResellerAccount) GetCountryOk() (*string, bool)`

GetCountryOk returns a tuple with the Country field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCountry

`func (o *ResellerAccount) SetCountry(v string)`

SetCountry sets Country field to given value.

### HasCountry

`func (o *ResellerAccount) HasCountry() bool`

HasCountry returns a boolean if a field has been set.

### GetDefaultCountrySms

`func (o *ResellerAccount) GetDefaultCountrySms() string`

GetDefaultCountrySms returns the DefaultCountrySms field if non-nil, zero value otherwise.

### GetDefaultCountrySmsOk

`func (o *ResellerAccount) GetDefaultCountrySmsOk() (*string, bool)`

GetDefaultCountrySmsOk returns a tuple with the DefaultCountrySms field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDefaultCountrySms

`func (o *ResellerAccount) SetDefaultCountrySms(v string)`

SetDefaultCountrySms sets DefaultCountrySms field to given value.

### HasDefaultCountrySms

`func (o *ResellerAccount) HasDefaultCountrySms() bool`

HasDefaultCountrySms returns a boolean if a field has been set.

### GetAutoRecharge

`func (o *ResellerAccount) GetAutoRecharge() int32`

GetAutoRecharge returns the AutoRecharge field if non-nil, zero value otherwise.

### GetAutoRechargeOk

`func (o *ResellerAccount) GetAutoRechargeOk() (*int32, bool)`

GetAutoRechargeOk returns a tuple with the AutoRecharge field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAutoRecharge

`func (o *ResellerAccount) SetAutoRecharge(v int32)`

SetAutoRecharge sets AutoRecharge field to given value.

### HasAutoRecharge

`func (o *ResellerAccount) HasAutoRecharge() bool`

HasAutoRecharge returns a boolean if a field has been set.

### GetAutoRechargeAmount

`func (o *ResellerAccount) GetAutoRechargeAmount() string`

GetAutoRechargeAmount returns the AutoRechargeAmount field if non-nil, zero value otherwise.

### GetAutoRechargeAmountOk

`func (o *ResellerAccount) GetAutoRechargeAmountOk() (*string, bool)`

GetAutoRechargeAmountOk returns a tuple with the AutoRechargeAmount field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAutoRechargeAmount

`func (o *ResellerAccount) SetAutoRechargeAmount(v string)`

SetAutoRechargeAmount sets AutoRechargeAmount field to given value.

### HasAutoRechargeAmount

`func (o *ResellerAccount) HasAutoRechargeAmount() bool`

HasAutoRechargeAmount returns a boolean if a field has been set.

### GetLowCreditAmount

`func (o *ResellerAccount) GetLowCreditAmount() string`

GetLowCreditAmount returns the LowCreditAmount field if non-nil, zero value otherwise.

### GetLowCreditAmountOk

`func (o *ResellerAccount) GetLowCreditAmountOk() (*string, bool)`

GetLowCreditAmountOk returns a tuple with the LowCreditAmount field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetLowCreditAmount

`func (o *ResellerAccount) SetLowCreditAmount(v string)`

SetLowCreditAmount sets LowCreditAmount field to given value.

### HasLowCreditAmount

`func (o *ResellerAccount) HasLowCreditAmount() bool`

HasLowCreditAmount returns a boolean if a field has been set.

### GetSettingUnicodeSms

`func (o *ResellerAccount) GetSettingUnicodeSms() int32`

GetSettingUnicodeSms returns the SettingUnicodeSms field if non-nil, zero value otherwise.

### GetSettingUnicodeSmsOk

`func (o *ResellerAccount) GetSettingUnicodeSmsOk() (*int32, bool)`

GetSettingUnicodeSmsOk returns a tuple with the SettingUnicodeSms field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSettingUnicodeSms

`func (o *ResellerAccount) SetSettingUnicodeSms(v int32)`

SetSettingUnicodeSms sets SettingUnicodeSms field to given value.

### HasSettingUnicodeSms

`func (o *ResellerAccount) HasSettingUnicodeSms() bool`

HasSettingUnicodeSms returns a boolean if a field has been set.

### GetSettingEmailSmsSubject

`func (o *ResellerAccount) GetSettingEmailSmsSubject() int32`

GetSettingEmailSmsSubject returns the SettingEmailSmsSubject field if non-nil, zero value otherwise.

### GetSettingEmailSmsSubjectOk

`func (o *ResellerAccount) GetSettingEmailSmsSubjectOk() (*int32, bool)`

GetSettingEmailSmsSubjectOk returns a tuple with the SettingEmailSmsSubject field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSettingEmailSmsSubject

`func (o *ResellerAccount) SetSettingEmailSmsSubject(v int32)`

SetSettingEmailSmsSubject sets SettingEmailSmsSubject field to given value.

### HasSettingEmailSmsSubject

`func (o *ResellerAccount) HasSettingEmailSmsSubject() bool`

HasSettingEmailSmsSubject returns a boolean if a field has been set.

### GetSettingFixSenderId

`func (o *ResellerAccount) GetSettingFixSenderId() int32`

GetSettingFixSenderId returns the SettingFixSenderId field if non-nil, zero value otherwise.

### GetSettingFixSenderIdOk

`func (o *ResellerAccount) GetSettingFixSenderIdOk() (*int32, bool)`

GetSettingFixSenderIdOk returns a tuple with the SettingFixSenderId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSettingFixSenderId

`func (o *ResellerAccount) SetSettingFixSenderId(v int32)`

SetSettingFixSenderId sets SettingFixSenderId field to given value.

### HasSettingFixSenderId

`func (o *ResellerAccount) HasSettingFixSenderId() bool`

HasSettingFixSenderId returns a boolean if a field has been set.

### GetSettingSmsMessageCharLimit

`func (o *ResellerAccount) GetSettingSmsMessageCharLimit() int32`

GetSettingSmsMessageCharLimit returns the SettingSmsMessageCharLimit field if non-nil, zero value otherwise.

### GetSettingSmsMessageCharLimitOk

`func (o *ResellerAccount) GetSettingSmsMessageCharLimitOk() (*int32, bool)`

GetSettingSmsMessageCharLimitOk returns a tuple with the SettingSmsMessageCharLimit field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSettingSmsMessageCharLimit

`func (o *ResellerAccount) SetSettingSmsMessageCharLimit(v int32)`

SetSettingSmsMessageCharLimit sets SettingSmsMessageCharLimit field to given value.

### HasSettingSmsMessageCharLimit

`func (o *ResellerAccount) HasSettingSmsMessageCharLimit() bool`

HasSettingSmsMessageCharLimit returns a boolean if a field has been set.

### GetOldDashboard

`func (o *ResellerAccount) GetOldDashboard() int32`

GetOldDashboard returns the OldDashboard field if non-nil, zero value otherwise.

### GetOldDashboardOk

`func (o *ResellerAccount) GetOldDashboardOk() (*int32, bool)`

GetOldDashboardOk returns a tuple with the OldDashboard field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetOldDashboard

`func (o *ResellerAccount) SetOldDashboard(v int32)`

SetOldDashboard sets OldDashboard field to given value.

### HasOldDashboard

`func (o *ResellerAccount) HasOldDashboard() bool`

HasOldDashboard returns a boolean if a field has been set.

### GetBalanceCommission

`func (o *ResellerAccount) GetBalanceCommission() string`

GetBalanceCommission returns the BalanceCommission field if non-nil, zero value otherwise.

### GetBalanceCommissionOk

`func (o *ResellerAccount) GetBalanceCommissionOk() (*string, bool)`

GetBalanceCommissionOk returns a tuple with the BalanceCommission field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetBalanceCommission

`func (o *ResellerAccount) SetBalanceCommission(v string)`

SetBalanceCommission sets BalanceCommission field to given value.

### HasBalanceCommission

`func (o *ResellerAccount) HasBalanceCommission() bool`

HasBalanceCommission returns a boolean if a field has been set.

### GetTimezone

`func (o *ResellerAccount) GetTimezone() string`

GetTimezone returns the Timezone field if non-nil, zero value otherwise.

### GetTimezoneOk

`func (o *ResellerAccount) GetTimezoneOk() (*string, bool)`

GetTimezoneOk returns a tuple with the Timezone field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTimezone

`func (o *ResellerAccount) SetTimezone(v string)`

SetTimezone sets Timezone field to given value.

### HasTimezone

`func (o *ResellerAccount) HasTimezone() bool`

HasTimezone returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


