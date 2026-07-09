# CreateResellerAccountData

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
**Currency** | Pointer to [**Currency**](Currency.md) |  | [optional] 
**Subaccount** | Pointer to [**Subaccount**](Subaccount.md) |  | [optional] 

## Methods

### NewCreateResellerAccountData

`func NewCreateResellerAccountData() *CreateResellerAccountData`

NewCreateResellerAccountData instantiates a new CreateResellerAccountData object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewCreateResellerAccountDataWithDefaults

`func NewCreateResellerAccountDataWithDefaults() *CreateResellerAccountData`

NewCreateResellerAccountDataWithDefaults instantiates a new CreateResellerAccountData object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetUserId

`func (o *CreateResellerAccountData) GetUserId() int32`

GetUserId returns the UserId field if non-nil, zero value otherwise.

### GetUserIdOk

`func (o *CreateResellerAccountData) GetUserIdOk() (*int32, bool)`

GetUserIdOk returns a tuple with the UserId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetUserId

`func (o *CreateResellerAccountData) SetUserId(v int32)`

SetUserId sets UserId field to given value.

### HasUserId

`func (o *CreateResellerAccountData) HasUserId() bool`

HasUserId returns a boolean if a field has been set.

### GetUsername

`func (o *CreateResellerAccountData) GetUsername() string`

GetUsername returns the Username field if non-nil, zero value otherwise.

### GetUsernameOk

`func (o *CreateResellerAccountData) GetUsernameOk() (*string, bool)`

GetUsernameOk returns a tuple with the Username field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetUsername

`func (o *CreateResellerAccountData) SetUsername(v string)`

SetUsername sets Username field to given value.

### HasUsername

`func (o *CreateResellerAccountData) HasUsername() bool`

HasUsername returns a boolean if a field has been set.

### GetUserEmail

`func (o *CreateResellerAccountData) GetUserEmail() string`

GetUserEmail returns the UserEmail field if non-nil, zero value otherwise.

### GetUserEmailOk

`func (o *CreateResellerAccountData) GetUserEmailOk() (*string, bool)`

GetUserEmailOk returns a tuple with the UserEmail field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetUserEmail

`func (o *CreateResellerAccountData) SetUserEmail(v string)`

SetUserEmail sets UserEmail field to given value.

### HasUserEmail

`func (o *CreateResellerAccountData) HasUserEmail() bool`

HasUserEmail returns a boolean if a field has been set.

### GetActive

`func (o *CreateResellerAccountData) GetActive() int32`

GetActive returns the Active field if non-nil, zero value otherwise.

### GetActiveOk

`func (o *CreateResellerAccountData) GetActiveOk() (*int32, bool)`

GetActiveOk returns a tuple with the Active field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetActive

`func (o *CreateResellerAccountData) SetActive(v int32)`

SetActive sets Active field to given value.

### HasActive

`func (o *CreateResellerAccountData) HasActive() bool`

HasActive returns a boolean if a field has been set.

### GetBanned

`func (o *CreateResellerAccountData) GetBanned() int32`

GetBanned returns the Banned field if non-nil, zero value otherwise.

### GetBannedOk

`func (o *CreateResellerAccountData) GetBannedOk() (*int32, bool)`

GetBannedOk returns a tuple with the Banned field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetBanned

`func (o *CreateResellerAccountData) SetBanned(v int32)`

SetBanned sets Banned field to given value.

### HasBanned

`func (o *CreateResellerAccountData) HasBanned() bool`

HasBanned returns a boolean if a field has been set.

### GetBalance

`func (o *CreateResellerAccountData) GetBalance() string`

GetBalance returns the Balance field if non-nil, zero value otherwise.

### GetBalanceOk

`func (o *CreateResellerAccountData) GetBalanceOk() (*string, bool)`

GetBalanceOk returns a tuple with the Balance field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetBalance

`func (o *CreateResellerAccountData) SetBalance(v string)`

SetBalance sets Balance field to given value.

### HasBalance

`func (o *CreateResellerAccountData) HasBalance() bool`

HasBalance returns a boolean if a field has been set.

### GetUserPhone

`func (o *CreateResellerAccountData) GetUserPhone() string`

GetUserPhone returns the UserPhone field if non-nil, zero value otherwise.

### GetUserPhoneOk

`func (o *CreateResellerAccountData) GetUserPhoneOk() (*string, bool)`

GetUserPhoneOk returns a tuple with the UserPhone field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetUserPhone

`func (o *CreateResellerAccountData) SetUserPhone(v string)`

SetUserPhone sets UserPhone field to given value.

### HasUserPhone

`func (o *CreateResellerAccountData) HasUserPhone() bool`

HasUserPhone returns a boolean if a field has been set.

### GetReplyTo

`func (o *CreateResellerAccountData) GetReplyTo() string`

GetReplyTo returns the ReplyTo field if non-nil, zero value otherwise.

### GetReplyToOk

`func (o *CreateResellerAccountData) GetReplyToOk() (*string, bool)`

GetReplyToOk returns a tuple with the ReplyTo field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetReplyTo

`func (o *CreateResellerAccountData) SetReplyTo(v string)`

SetReplyTo sets ReplyTo field to given value.

### HasReplyTo

`func (o *CreateResellerAccountData) HasReplyTo() bool`

HasReplyTo returns a boolean if a field has been set.

### GetDeliveryTo

`func (o *CreateResellerAccountData) GetDeliveryTo() string`

GetDeliveryTo returns the DeliveryTo field if non-nil, zero value otherwise.

### GetDeliveryToOk

`func (o *CreateResellerAccountData) GetDeliveryToOk() (*string, bool)`

GetDeliveryToOk returns a tuple with the DeliveryTo field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDeliveryTo

`func (o *CreateResellerAccountData) SetDeliveryTo(v string)`

SetDeliveryTo sets DeliveryTo field to given value.

### HasDeliveryTo

`func (o *CreateResellerAccountData) HasDeliveryTo() bool`

HasDeliveryTo returns a boolean if a field has been set.

### SetDeliveryToNil

`func (o *CreateResellerAccountData) SetDeliveryToNil(b bool)`

 SetDeliveryToNil sets the value for DeliveryTo to be an explicit nil

### UnsetDeliveryTo
`func (o *CreateResellerAccountData) UnsetDeliveryTo()`

UnsetDeliveryTo ensures that no value is present for DeliveryTo, not even an explicit nil
### GetUserFirstName

`func (o *CreateResellerAccountData) GetUserFirstName() string`

GetUserFirstName returns the UserFirstName field if non-nil, zero value otherwise.

### GetUserFirstNameOk

`func (o *CreateResellerAccountData) GetUserFirstNameOk() (*string, bool)`

GetUserFirstNameOk returns a tuple with the UserFirstName field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetUserFirstName

`func (o *CreateResellerAccountData) SetUserFirstName(v string)`

SetUserFirstName sets UserFirstName field to given value.

### HasUserFirstName

`func (o *CreateResellerAccountData) HasUserFirstName() bool`

HasUserFirstName returns a boolean if a field has been set.

### GetUserLastName

`func (o *CreateResellerAccountData) GetUserLastName() string`

GetUserLastName returns the UserLastName field if non-nil, zero value otherwise.

### GetUserLastNameOk

`func (o *CreateResellerAccountData) GetUserLastNameOk() (*string, bool)`

GetUserLastNameOk returns a tuple with the UserLastName field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetUserLastName

`func (o *CreateResellerAccountData) SetUserLastName(v string)`

SetUserLastName sets UserLastName field to given value.

### HasUserLastName

`func (o *CreateResellerAccountData) HasUserLastName() bool`

HasUserLastName returns a boolean if a field has been set.

### GetAccount

`func (o *CreateResellerAccountData) GetAccount() int32`

GetAccount returns the Account field if non-nil, zero value otherwise.

### GetAccountOk

`func (o *CreateResellerAccountData) GetAccountOk() (*int32, bool)`

GetAccountOk returns a tuple with the Account field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAccount

`func (o *CreateResellerAccountData) SetAccount(v int32)`

SetAccount sets Account field to given value.

### HasAccount

`func (o *CreateResellerAccountData) HasAccount() bool`

HasAccount returns a boolean if a field has been set.

### GetAccountName

`func (o *CreateResellerAccountData) GetAccountName() string`

GetAccountName returns the AccountName field if non-nil, zero value otherwise.

### GetAccountNameOk

`func (o *CreateResellerAccountData) GetAccountNameOk() (*string, bool)`

GetAccountNameOk returns a tuple with the AccountName field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAccountName

`func (o *CreateResellerAccountData) SetAccountName(v string)`

SetAccountName sets AccountName field to given value.

### HasAccountName

`func (o *CreateResellerAccountData) HasAccountName() bool`

HasAccountName returns a boolean if a field has been set.

### GetAccountBillingEmail

`func (o *CreateResellerAccountData) GetAccountBillingEmail() string`

GetAccountBillingEmail returns the AccountBillingEmail field if non-nil, zero value otherwise.

### GetAccountBillingEmailOk

`func (o *CreateResellerAccountData) GetAccountBillingEmailOk() (*string, bool)`

GetAccountBillingEmailOk returns a tuple with the AccountBillingEmail field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAccountBillingEmail

`func (o *CreateResellerAccountData) SetAccountBillingEmail(v string)`

SetAccountBillingEmail sets AccountBillingEmail field to given value.

### HasAccountBillingEmail

`func (o *CreateResellerAccountData) HasAccountBillingEmail() bool`

HasAccountBillingEmail returns a boolean if a field has been set.

### GetAccountBillingMobile

`func (o *CreateResellerAccountData) GetAccountBillingMobile() string`

GetAccountBillingMobile returns the AccountBillingMobile field if non-nil, zero value otherwise.

### GetAccountBillingMobileOk

`func (o *CreateResellerAccountData) GetAccountBillingMobileOk() (*string, bool)`

GetAccountBillingMobileOk returns a tuple with the AccountBillingMobile field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAccountBillingMobile

`func (o *CreateResellerAccountData) SetAccountBillingMobile(v string)`

SetAccountBillingMobile sets AccountBillingMobile field to given value.

### HasAccountBillingMobile

`func (o *CreateResellerAccountData) HasAccountBillingMobile() bool`

HasAccountBillingMobile returns a boolean if a field has been set.

### GetCountry

`func (o *CreateResellerAccountData) GetCountry() string`

GetCountry returns the Country field if non-nil, zero value otherwise.

### GetCountryOk

`func (o *CreateResellerAccountData) GetCountryOk() (*string, bool)`

GetCountryOk returns a tuple with the Country field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCountry

`func (o *CreateResellerAccountData) SetCountry(v string)`

SetCountry sets Country field to given value.

### HasCountry

`func (o *CreateResellerAccountData) HasCountry() bool`

HasCountry returns a boolean if a field has been set.

### GetDefaultCountrySms

`func (o *CreateResellerAccountData) GetDefaultCountrySms() string`

GetDefaultCountrySms returns the DefaultCountrySms field if non-nil, zero value otherwise.

### GetDefaultCountrySmsOk

`func (o *CreateResellerAccountData) GetDefaultCountrySmsOk() (*string, bool)`

GetDefaultCountrySmsOk returns a tuple with the DefaultCountrySms field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDefaultCountrySms

`func (o *CreateResellerAccountData) SetDefaultCountrySms(v string)`

SetDefaultCountrySms sets DefaultCountrySms field to given value.

### HasDefaultCountrySms

`func (o *CreateResellerAccountData) HasDefaultCountrySms() bool`

HasDefaultCountrySms returns a boolean if a field has been set.

### GetAutoRecharge

`func (o *CreateResellerAccountData) GetAutoRecharge() int32`

GetAutoRecharge returns the AutoRecharge field if non-nil, zero value otherwise.

### GetAutoRechargeOk

`func (o *CreateResellerAccountData) GetAutoRechargeOk() (*int32, bool)`

GetAutoRechargeOk returns a tuple with the AutoRecharge field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAutoRecharge

`func (o *CreateResellerAccountData) SetAutoRecharge(v int32)`

SetAutoRecharge sets AutoRecharge field to given value.

### HasAutoRecharge

`func (o *CreateResellerAccountData) HasAutoRecharge() bool`

HasAutoRecharge returns a boolean if a field has been set.

### GetAutoRechargeAmount

`func (o *CreateResellerAccountData) GetAutoRechargeAmount() string`

GetAutoRechargeAmount returns the AutoRechargeAmount field if non-nil, zero value otherwise.

### GetAutoRechargeAmountOk

`func (o *CreateResellerAccountData) GetAutoRechargeAmountOk() (*string, bool)`

GetAutoRechargeAmountOk returns a tuple with the AutoRechargeAmount field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAutoRechargeAmount

`func (o *CreateResellerAccountData) SetAutoRechargeAmount(v string)`

SetAutoRechargeAmount sets AutoRechargeAmount field to given value.

### HasAutoRechargeAmount

`func (o *CreateResellerAccountData) HasAutoRechargeAmount() bool`

HasAutoRechargeAmount returns a boolean if a field has been set.

### GetLowCreditAmount

`func (o *CreateResellerAccountData) GetLowCreditAmount() string`

GetLowCreditAmount returns the LowCreditAmount field if non-nil, zero value otherwise.

### GetLowCreditAmountOk

`func (o *CreateResellerAccountData) GetLowCreditAmountOk() (*string, bool)`

GetLowCreditAmountOk returns a tuple with the LowCreditAmount field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetLowCreditAmount

`func (o *CreateResellerAccountData) SetLowCreditAmount(v string)`

SetLowCreditAmount sets LowCreditAmount field to given value.

### HasLowCreditAmount

`func (o *CreateResellerAccountData) HasLowCreditAmount() bool`

HasLowCreditAmount returns a boolean if a field has been set.

### GetSettingUnicodeSms

`func (o *CreateResellerAccountData) GetSettingUnicodeSms() int32`

GetSettingUnicodeSms returns the SettingUnicodeSms field if non-nil, zero value otherwise.

### GetSettingUnicodeSmsOk

`func (o *CreateResellerAccountData) GetSettingUnicodeSmsOk() (*int32, bool)`

GetSettingUnicodeSmsOk returns a tuple with the SettingUnicodeSms field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSettingUnicodeSms

`func (o *CreateResellerAccountData) SetSettingUnicodeSms(v int32)`

SetSettingUnicodeSms sets SettingUnicodeSms field to given value.

### HasSettingUnicodeSms

`func (o *CreateResellerAccountData) HasSettingUnicodeSms() bool`

HasSettingUnicodeSms returns a boolean if a field has been set.

### GetSettingEmailSmsSubject

`func (o *CreateResellerAccountData) GetSettingEmailSmsSubject() int32`

GetSettingEmailSmsSubject returns the SettingEmailSmsSubject field if non-nil, zero value otherwise.

### GetSettingEmailSmsSubjectOk

`func (o *CreateResellerAccountData) GetSettingEmailSmsSubjectOk() (*int32, bool)`

GetSettingEmailSmsSubjectOk returns a tuple with the SettingEmailSmsSubject field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSettingEmailSmsSubject

`func (o *CreateResellerAccountData) SetSettingEmailSmsSubject(v int32)`

SetSettingEmailSmsSubject sets SettingEmailSmsSubject field to given value.

### HasSettingEmailSmsSubject

`func (o *CreateResellerAccountData) HasSettingEmailSmsSubject() bool`

HasSettingEmailSmsSubject returns a boolean if a field has been set.

### GetSettingFixSenderId

`func (o *CreateResellerAccountData) GetSettingFixSenderId() int32`

GetSettingFixSenderId returns the SettingFixSenderId field if non-nil, zero value otherwise.

### GetSettingFixSenderIdOk

`func (o *CreateResellerAccountData) GetSettingFixSenderIdOk() (*int32, bool)`

GetSettingFixSenderIdOk returns a tuple with the SettingFixSenderId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSettingFixSenderId

`func (o *CreateResellerAccountData) SetSettingFixSenderId(v int32)`

SetSettingFixSenderId sets SettingFixSenderId field to given value.

### HasSettingFixSenderId

`func (o *CreateResellerAccountData) HasSettingFixSenderId() bool`

HasSettingFixSenderId returns a boolean if a field has been set.

### GetSettingSmsMessageCharLimit

`func (o *CreateResellerAccountData) GetSettingSmsMessageCharLimit() int32`

GetSettingSmsMessageCharLimit returns the SettingSmsMessageCharLimit field if non-nil, zero value otherwise.

### GetSettingSmsMessageCharLimitOk

`func (o *CreateResellerAccountData) GetSettingSmsMessageCharLimitOk() (*int32, bool)`

GetSettingSmsMessageCharLimitOk returns a tuple with the SettingSmsMessageCharLimit field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSettingSmsMessageCharLimit

`func (o *CreateResellerAccountData) SetSettingSmsMessageCharLimit(v int32)`

SetSettingSmsMessageCharLimit sets SettingSmsMessageCharLimit field to given value.

### HasSettingSmsMessageCharLimit

`func (o *CreateResellerAccountData) HasSettingSmsMessageCharLimit() bool`

HasSettingSmsMessageCharLimit returns a boolean if a field has been set.

### GetOldDashboard

`func (o *CreateResellerAccountData) GetOldDashboard() int32`

GetOldDashboard returns the OldDashboard field if non-nil, zero value otherwise.

### GetOldDashboardOk

`func (o *CreateResellerAccountData) GetOldDashboardOk() (*int32, bool)`

GetOldDashboardOk returns a tuple with the OldDashboard field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetOldDashboard

`func (o *CreateResellerAccountData) SetOldDashboard(v int32)`

SetOldDashboard sets OldDashboard field to given value.

### HasOldDashboard

`func (o *CreateResellerAccountData) HasOldDashboard() bool`

HasOldDashboard returns a boolean if a field has been set.

### GetBalanceCommission

`func (o *CreateResellerAccountData) GetBalanceCommission() string`

GetBalanceCommission returns the BalanceCommission field if non-nil, zero value otherwise.

### GetBalanceCommissionOk

`func (o *CreateResellerAccountData) GetBalanceCommissionOk() (*string, bool)`

GetBalanceCommissionOk returns a tuple with the BalanceCommission field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetBalanceCommission

`func (o *CreateResellerAccountData) SetBalanceCommission(v string)`

SetBalanceCommission sets BalanceCommission field to given value.

### HasBalanceCommission

`func (o *CreateResellerAccountData) HasBalanceCommission() bool`

HasBalanceCommission returns a boolean if a field has been set.

### GetTimezone

`func (o *CreateResellerAccountData) GetTimezone() string`

GetTimezone returns the Timezone field if non-nil, zero value otherwise.

### GetTimezoneOk

`func (o *CreateResellerAccountData) GetTimezoneOk() (*string, bool)`

GetTimezoneOk returns a tuple with the Timezone field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTimezone

`func (o *CreateResellerAccountData) SetTimezone(v string)`

SetTimezone sets Timezone field to given value.

### HasTimezone

`func (o *CreateResellerAccountData) HasTimezone() bool`

HasTimezone returns a boolean if a field has been set.

### GetCurrency

`func (o *CreateResellerAccountData) GetCurrency() Currency`

GetCurrency returns the Currency field if non-nil, zero value otherwise.

### GetCurrencyOk

`func (o *CreateResellerAccountData) GetCurrencyOk() (*Currency, bool)`

GetCurrencyOk returns a tuple with the Currency field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCurrency

`func (o *CreateResellerAccountData) SetCurrency(v Currency)`

SetCurrency sets Currency field to given value.

### HasCurrency

`func (o *CreateResellerAccountData) HasCurrency() bool`

HasCurrency returns a boolean if a field has been set.

### GetSubaccount

`func (o *CreateResellerAccountData) GetSubaccount() Subaccount`

GetSubaccount returns the Subaccount field if non-nil, zero value otherwise.

### GetSubaccountOk

`func (o *CreateResellerAccountData) GetSubaccountOk() (*Subaccount, bool)`

GetSubaccountOk returns a tuple with the Subaccount field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSubaccount

`func (o *CreateResellerAccountData) SetSubaccount(v Subaccount)`

SetSubaccount sets Subaccount field to given value.

### HasSubaccount

`func (o *CreateResellerAccountData) HasSubaccount() bool`

HasSubaccount returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


