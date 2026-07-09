# Account

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**UserId** | Pointer to **int32** | The unique identifier for the user. | [optional] 
**Username** | Pointer to **string** | The username of the user. | [optional] 
**UserEmail** | Pointer to **string** | The email address of the user. | [optional] 
**Active** | Pointer to **int32** | Flag indicating if the user account is active. | [optional] 
**Banned** | Pointer to **int32** | Flag indicating if the user account is banned. | [optional] 
**Balance** | Pointer to **string** | The balance of the user&#39;s account. | [optional] 
**UserPhone** | Pointer to **string** | The phone number of the user. | [optional] 
**ReplyTo** | Pointer to **string** | The email address to reply to. | [optional] 
**DeliveryTo** | Pointer to **NullableString** | The delivery email address. | [optional] 
**UserFirstName** | Pointer to **string** | The first name of the user. | [optional] 
**UserLastName** | Pointer to **string** | The last name of the user. | [optional] 
**Account** | Pointer to **int32** | The account number. | [optional] 
**AccountName** | Pointer to **string** | The name of the account. | [optional] 
**AccountBillingEmail** | Pointer to **string** | The billing email address of the account. | [optional] 
**AccountBillingMobile** | Pointer to **string** | The billing mobile number of the account. | [optional] 
**Country** | Pointer to **string** | The country of the user. | [optional] 
**DefaultCountrySms** | Pointer to **string** | The default country for SMS. | [optional] 
**AutoRecharge** | Pointer to **int32** | Flag indicating if auto-recharge is enabled. | [optional] 
**AutoRechargeAmount** | Pointer to **string** | The auto-recharge amount. | [optional] 
**LowCreditAmount** | Pointer to **string** | The low credit amount. | [optional] 
**SettingUnicodeSms** | Pointer to **int32** | Flag indicating if unicode SMS is enabled. | [optional] 
**SettingEmailSmsSubject** | Pointer to **int32** | Flag indicating if email SMS subject is enabled. | [optional] 
**SettingFixSenderId** | Pointer to **int32** | Flag indicating if fixing sender ID is enabled. | [optional] 
**SettingSmsMessageCharLimit** | Pointer to **int32** | The SMS message character limit. | [optional] 
**OldDashboard** | Pointer to **int32** | Flag indicating if old dashboard is enabled. | [optional] 
**BalanceCommission** | Pointer to **string** | The balance commission. | [optional] 
**Timezone** | Pointer to **string** | The timezone of the user. | [optional] 
**PriceRate** | Pointer to **int32** | The pricing tier used to determine the cost per message. | [optional] 
**Currency** | Pointer to [**Currency**](Currency.md) |  | [optional] 
**Subaccount** | Pointer to [**Subaccount**](Subaccount.md) |  | [optional] 

## Methods

### NewAccount

`func NewAccount() *Account`

NewAccount instantiates a new Account object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewAccountWithDefaults

`func NewAccountWithDefaults() *Account`

NewAccountWithDefaults instantiates a new Account object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetUserId

`func (o *Account) GetUserId() int32`

GetUserId returns the UserId field if non-nil, zero value otherwise.

### GetUserIdOk

`func (o *Account) GetUserIdOk() (*int32, bool)`

GetUserIdOk returns a tuple with the UserId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetUserId

`func (o *Account) SetUserId(v int32)`

SetUserId sets UserId field to given value.

### HasUserId

`func (o *Account) HasUserId() bool`

HasUserId returns a boolean if a field has been set.

### GetUsername

`func (o *Account) GetUsername() string`

GetUsername returns the Username field if non-nil, zero value otherwise.

### GetUsernameOk

`func (o *Account) GetUsernameOk() (*string, bool)`

GetUsernameOk returns a tuple with the Username field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetUsername

`func (o *Account) SetUsername(v string)`

SetUsername sets Username field to given value.

### HasUsername

`func (o *Account) HasUsername() bool`

HasUsername returns a boolean if a field has been set.

### GetUserEmail

`func (o *Account) GetUserEmail() string`

GetUserEmail returns the UserEmail field if non-nil, zero value otherwise.

### GetUserEmailOk

`func (o *Account) GetUserEmailOk() (*string, bool)`

GetUserEmailOk returns a tuple with the UserEmail field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetUserEmail

`func (o *Account) SetUserEmail(v string)`

SetUserEmail sets UserEmail field to given value.

### HasUserEmail

`func (o *Account) HasUserEmail() bool`

HasUserEmail returns a boolean if a field has been set.

### GetActive

`func (o *Account) GetActive() int32`

GetActive returns the Active field if non-nil, zero value otherwise.

### GetActiveOk

`func (o *Account) GetActiveOk() (*int32, bool)`

GetActiveOk returns a tuple with the Active field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetActive

`func (o *Account) SetActive(v int32)`

SetActive sets Active field to given value.

### HasActive

`func (o *Account) HasActive() bool`

HasActive returns a boolean if a field has been set.

### GetBanned

`func (o *Account) GetBanned() int32`

GetBanned returns the Banned field if non-nil, zero value otherwise.

### GetBannedOk

`func (o *Account) GetBannedOk() (*int32, bool)`

GetBannedOk returns a tuple with the Banned field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetBanned

`func (o *Account) SetBanned(v int32)`

SetBanned sets Banned field to given value.

### HasBanned

`func (o *Account) HasBanned() bool`

HasBanned returns a boolean if a field has been set.

### GetBalance

`func (o *Account) GetBalance() string`

GetBalance returns the Balance field if non-nil, zero value otherwise.

### GetBalanceOk

`func (o *Account) GetBalanceOk() (*string, bool)`

GetBalanceOk returns a tuple with the Balance field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetBalance

`func (o *Account) SetBalance(v string)`

SetBalance sets Balance field to given value.

### HasBalance

`func (o *Account) HasBalance() bool`

HasBalance returns a boolean if a field has been set.

### GetUserPhone

`func (o *Account) GetUserPhone() string`

GetUserPhone returns the UserPhone field if non-nil, zero value otherwise.

### GetUserPhoneOk

`func (o *Account) GetUserPhoneOk() (*string, bool)`

GetUserPhoneOk returns a tuple with the UserPhone field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetUserPhone

`func (o *Account) SetUserPhone(v string)`

SetUserPhone sets UserPhone field to given value.

### HasUserPhone

`func (o *Account) HasUserPhone() bool`

HasUserPhone returns a boolean if a field has been set.

### GetReplyTo

`func (o *Account) GetReplyTo() string`

GetReplyTo returns the ReplyTo field if non-nil, zero value otherwise.

### GetReplyToOk

`func (o *Account) GetReplyToOk() (*string, bool)`

GetReplyToOk returns a tuple with the ReplyTo field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetReplyTo

`func (o *Account) SetReplyTo(v string)`

SetReplyTo sets ReplyTo field to given value.

### HasReplyTo

`func (o *Account) HasReplyTo() bool`

HasReplyTo returns a boolean if a field has been set.

### GetDeliveryTo

`func (o *Account) GetDeliveryTo() string`

GetDeliveryTo returns the DeliveryTo field if non-nil, zero value otherwise.

### GetDeliveryToOk

`func (o *Account) GetDeliveryToOk() (*string, bool)`

GetDeliveryToOk returns a tuple with the DeliveryTo field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDeliveryTo

`func (o *Account) SetDeliveryTo(v string)`

SetDeliveryTo sets DeliveryTo field to given value.

### HasDeliveryTo

`func (o *Account) HasDeliveryTo() bool`

HasDeliveryTo returns a boolean if a field has been set.

### SetDeliveryToNil

`func (o *Account) SetDeliveryToNil(b bool)`

 SetDeliveryToNil sets the value for DeliveryTo to be an explicit nil

### UnsetDeliveryTo
`func (o *Account) UnsetDeliveryTo()`

UnsetDeliveryTo ensures that no value is present for DeliveryTo, not even an explicit nil
### GetUserFirstName

`func (o *Account) GetUserFirstName() string`

GetUserFirstName returns the UserFirstName field if non-nil, zero value otherwise.

### GetUserFirstNameOk

`func (o *Account) GetUserFirstNameOk() (*string, bool)`

GetUserFirstNameOk returns a tuple with the UserFirstName field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetUserFirstName

`func (o *Account) SetUserFirstName(v string)`

SetUserFirstName sets UserFirstName field to given value.

### HasUserFirstName

`func (o *Account) HasUserFirstName() bool`

HasUserFirstName returns a boolean if a field has been set.

### GetUserLastName

`func (o *Account) GetUserLastName() string`

GetUserLastName returns the UserLastName field if non-nil, zero value otherwise.

### GetUserLastNameOk

`func (o *Account) GetUserLastNameOk() (*string, bool)`

GetUserLastNameOk returns a tuple with the UserLastName field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetUserLastName

`func (o *Account) SetUserLastName(v string)`

SetUserLastName sets UserLastName field to given value.

### HasUserLastName

`func (o *Account) HasUserLastName() bool`

HasUserLastName returns a boolean if a field has been set.

### GetAccount

`func (o *Account) GetAccount() int32`

GetAccount returns the Account field if non-nil, zero value otherwise.

### GetAccountOk

`func (o *Account) GetAccountOk() (*int32, bool)`

GetAccountOk returns a tuple with the Account field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAccount

`func (o *Account) SetAccount(v int32)`

SetAccount sets Account field to given value.

### HasAccount

`func (o *Account) HasAccount() bool`

HasAccount returns a boolean if a field has been set.

### GetAccountName

`func (o *Account) GetAccountName() string`

GetAccountName returns the AccountName field if non-nil, zero value otherwise.

### GetAccountNameOk

`func (o *Account) GetAccountNameOk() (*string, bool)`

GetAccountNameOk returns a tuple with the AccountName field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAccountName

`func (o *Account) SetAccountName(v string)`

SetAccountName sets AccountName field to given value.

### HasAccountName

`func (o *Account) HasAccountName() bool`

HasAccountName returns a boolean if a field has been set.

### GetAccountBillingEmail

`func (o *Account) GetAccountBillingEmail() string`

GetAccountBillingEmail returns the AccountBillingEmail field if non-nil, zero value otherwise.

### GetAccountBillingEmailOk

`func (o *Account) GetAccountBillingEmailOk() (*string, bool)`

GetAccountBillingEmailOk returns a tuple with the AccountBillingEmail field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAccountBillingEmail

`func (o *Account) SetAccountBillingEmail(v string)`

SetAccountBillingEmail sets AccountBillingEmail field to given value.

### HasAccountBillingEmail

`func (o *Account) HasAccountBillingEmail() bool`

HasAccountBillingEmail returns a boolean if a field has been set.

### GetAccountBillingMobile

`func (o *Account) GetAccountBillingMobile() string`

GetAccountBillingMobile returns the AccountBillingMobile field if non-nil, zero value otherwise.

### GetAccountBillingMobileOk

`func (o *Account) GetAccountBillingMobileOk() (*string, bool)`

GetAccountBillingMobileOk returns a tuple with the AccountBillingMobile field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAccountBillingMobile

`func (o *Account) SetAccountBillingMobile(v string)`

SetAccountBillingMobile sets AccountBillingMobile field to given value.

### HasAccountBillingMobile

`func (o *Account) HasAccountBillingMobile() bool`

HasAccountBillingMobile returns a boolean if a field has been set.

### GetCountry

`func (o *Account) GetCountry() string`

GetCountry returns the Country field if non-nil, zero value otherwise.

### GetCountryOk

`func (o *Account) GetCountryOk() (*string, bool)`

GetCountryOk returns a tuple with the Country field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCountry

`func (o *Account) SetCountry(v string)`

SetCountry sets Country field to given value.

### HasCountry

`func (o *Account) HasCountry() bool`

HasCountry returns a boolean if a field has been set.

### GetDefaultCountrySms

`func (o *Account) GetDefaultCountrySms() string`

GetDefaultCountrySms returns the DefaultCountrySms field if non-nil, zero value otherwise.

### GetDefaultCountrySmsOk

`func (o *Account) GetDefaultCountrySmsOk() (*string, bool)`

GetDefaultCountrySmsOk returns a tuple with the DefaultCountrySms field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDefaultCountrySms

`func (o *Account) SetDefaultCountrySms(v string)`

SetDefaultCountrySms sets DefaultCountrySms field to given value.

### HasDefaultCountrySms

`func (o *Account) HasDefaultCountrySms() bool`

HasDefaultCountrySms returns a boolean if a field has been set.

### GetAutoRecharge

`func (o *Account) GetAutoRecharge() int32`

GetAutoRecharge returns the AutoRecharge field if non-nil, zero value otherwise.

### GetAutoRechargeOk

`func (o *Account) GetAutoRechargeOk() (*int32, bool)`

GetAutoRechargeOk returns a tuple with the AutoRecharge field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAutoRecharge

`func (o *Account) SetAutoRecharge(v int32)`

SetAutoRecharge sets AutoRecharge field to given value.

### HasAutoRecharge

`func (o *Account) HasAutoRecharge() bool`

HasAutoRecharge returns a boolean if a field has been set.

### GetAutoRechargeAmount

`func (o *Account) GetAutoRechargeAmount() string`

GetAutoRechargeAmount returns the AutoRechargeAmount field if non-nil, zero value otherwise.

### GetAutoRechargeAmountOk

`func (o *Account) GetAutoRechargeAmountOk() (*string, bool)`

GetAutoRechargeAmountOk returns a tuple with the AutoRechargeAmount field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAutoRechargeAmount

`func (o *Account) SetAutoRechargeAmount(v string)`

SetAutoRechargeAmount sets AutoRechargeAmount field to given value.

### HasAutoRechargeAmount

`func (o *Account) HasAutoRechargeAmount() bool`

HasAutoRechargeAmount returns a boolean if a field has been set.

### GetLowCreditAmount

`func (o *Account) GetLowCreditAmount() string`

GetLowCreditAmount returns the LowCreditAmount field if non-nil, zero value otherwise.

### GetLowCreditAmountOk

`func (o *Account) GetLowCreditAmountOk() (*string, bool)`

GetLowCreditAmountOk returns a tuple with the LowCreditAmount field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetLowCreditAmount

`func (o *Account) SetLowCreditAmount(v string)`

SetLowCreditAmount sets LowCreditAmount field to given value.

### HasLowCreditAmount

`func (o *Account) HasLowCreditAmount() bool`

HasLowCreditAmount returns a boolean if a field has been set.

### GetSettingUnicodeSms

`func (o *Account) GetSettingUnicodeSms() int32`

GetSettingUnicodeSms returns the SettingUnicodeSms field if non-nil, zero value otherwise.

### GetSettingUnicodeSmsOk

`func (o *Account) GetSettingUnicodeSmsOk() (*int32, bool)`

GetSettingUnicodeSmsOk returns a tuple with the SettingUnicodeSms field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSettingUnicodeSms

`func (o *Account) SetSettingUnicodeSms(v int32)`

SetSettingUnicodeSms sets SettingUnicodeSms field to given value.

### HasSettingUnicodeSms

`func (o *Account) HasSettingUnicodeSms() bool`

HasSettingUnicodeSms returns a boolean if a field has been set.

### GetSettingEmailSmsSubject

`func (o *Account) GetSettingEmailSmsSubject() int32`

GetSettingEmailSmsSubject returns the SettingEmailSmsSubject field if non-nil, zero value otherwise.

### GetSettingEmailSmsSubjectOk

`func (o *Account) GetSettingEmailSmsSubjectOk() (*int32, bool)`

GetSettingEmailSmsSubjectOk returns a tuple with the SettingEmailSmsSubject field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSettingEmailSmsSubject

`func (o *Account) SetSettingEmailSmsSubject(v int32)`

SetSettingEmailSmsSubject sets SettingEmailSmsSubject field to given value.

### HasSettingEmailSmsSubject

`func (o *Account) HasSettingEmailSmsSubject() bool`

HasSettingEmailSmsSubject returns a boolean if a field has been set.

### GetSettingFixSenderId

`func (o *Account) GetSettingFixSenderId() int32`

GetSettingFixSenderId returns the SettingFixSenderId field if non-nil, zero value otherwise.

### GetSettingFixSenderIdOk

`func (o *Account) GetSettingFixSenderIdOk() (*int32, bool)`

GetSettingFixSenderIdOk returns a tuple with the SettingFixSenderId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSettingFixSenderId

`func (o *Account) SetSettingFixSenderId(v int32)`

SetSettingFixSenderId sets SettingFixSenderId field to given value.

### HasSettingFixSenderId

`func (o *Account) HasSettingFixSenderId() bool`

HasSettingFixSenderId returns a boolean if a field has been set.

### GetSettingSmsMessageCharLimit

`func (o *Account) GetSettingSmsMessageCharLimit() int32`

GetSettingSmsMessageCharLimit returns the SettingSmsMessageCharLimit field if non-nil, zero value otherwise.

### GetSettingSmsMessageCharLimitOk

`func (o *Account) GetSettingSmsMessageCharLimitOk() (*int32, bool)`

GetSettingSmsMessageCharLimitOk returns a tuple with the SettingSmsMessageCharLimit field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSettingSmsMessageCharLimit

`func (o *Account) SetSettingSmsMessageCharLimit(v int32)`

SetSettingSmsMessageCharLimit sets SettingSmsMessageCharLimit field to given value.

### HasSettingSmsMessageCharLimit

`func (o *Account) HasSettingSmsMessageCharLimit() bool`

HasSettingSmsMessageCharLimit returns a boolean if a field has been set.

### GetOldDashboard

`func (o *Account) GetOldDashboard() int32`

GetOldDashboard returns the OldDashboard field if non-nil, zero value otherwise.

### GetOldDashboardOk

`func (o *Account) GetOldDashboardOk() (*int32, bool)`

GetOldDashboardOk returns a tuple with the OldDashboard field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetOldDashboard

`func (o *Account) SetOldDashboard(v int32)`

SetOldDashboard sets OldDashboard field to given value.

### HasOldDashboard

`func (o *Account) HasOldDashboard() bool`

HasOldDashboard returns a boolean if a field has been set.

### GetBalanceCommission

`func (o *Account) GetBalanceCommission() string`

GetBalanceCommission returns the BalanceCommission field if non-nil, zero value otherwise.

### GetBalanceCommissionOk

`func (o *Account) GetBalanceCommissionOk() (*string, bool)`

GetBalanceCommissionOk returns a tuple with the BalanceCommission field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetBalanceCommission

`func (o *Account) SetBalanceCommission(v string)`

SetBalanceCommission sets BalanceCommission field to given value.

### HasBalanceCommission

`func (o *Account) HasBalanceCommission() bool`

HasBalanceCommission returns a boolean if a field has been set.

### GetTimezone

`func (o *Account) GetTimezone() string`

GetTimezone returns the Timezone field if non-nil, zero value otherwise.

### GetTimezoneOk

`func (o *Account) GetTimezoneOk() (*string, bool)`

GetTimezoneOk returns a tuple with the Timezone field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTimezone

`func (o *Account) SetTimezone(v string)`

SetTimezone sets Timezone field to given value.

### HasTimezone

`func (o *Account) HasTimezone() bool`

HasTimezone returns a boolean if a field has been set.

### GetPriceRate

`func (o *Account) GetPriceRate() int32`

GetPriceRate returns the PriceRate field if non-nil, zero value otherwise.

### GetPriceRateOk

`func (o *Account) GetPriceRateOk() (*int32, bool)`

GetPriceRateOk returns a tuple with the PriceRate field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetPriceRate

`func (o *Account) SetPriceRate(v int32)`

SetPriceRate sets PriceRate field to given value.

### HasPriceRate

`func (o *Account) HasPriceRate() bool`

HasPriceRate returns a boolean if a field has been set.

### GetCurrency

`func (o *Account) GetCurrency() Currency`

GetCurrency returns the Currency field if non-nil, zero value otherwise.

### GetCurrencyOk

`func (o *Account) GetCurrencyOk() (*Currency, bool)`

GetCurrencyOk returns a tuple with the Currency field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCurrency

`func (o *Account) SetCurrency(v Currency)`

SetCurrency sets Currency field to given value.

### HasCurrency

`func (o *Account) HasCurrency() bool`

HasCurrency returns a boolean if a field has been set.

### GetSubaccount

`func (o *Account) GetSubaccount() Subaccount`

GetSubaccount returns the Subaccount field if non-nil, zero value otherwise.

### GetSubaccountOk

`func (o *Account) GetSubaccountOk() (*Subaccount, bool)`

GetSubaccountOk returns a tuple with the Subaccount field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSubaccount

`func (o *Account) SetSubaccount(v Subaccount)`

SetSubaccount sets Subaccount field to given value.

### HasSubaccount

`func (o *Account) HasSubaccount() bool`

HasSubaccount returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


