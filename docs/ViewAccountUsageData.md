# ViewAccountUsageData

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Sms** | Pointer to [**[]ViewAccountUsageDataSmsInner**](ViewAccountUsageDataSmsInner.md) |  | [optional] 
**Mms** | Pointer to [**[]ViewAccountUsageDataMmsInner**](ViewAccountUsageDataMmsInner.md) |  | [optional] 
**Voice** | Pointer to [**[]ViewAccountUsageDataMmsInner**](ViewAccountUsageDataMmsInner.md) |  | [optional] 
**Fax** | Pointer to [**[]ViewAccountUsageDataMmsInner**](ViewAccountUsageDataMmsInner.md) |  | [optional] 
**Post** | Pointer to [**[]ViewAccountUsageDataMmsInner**](ViewAccountUsageDataMmsInner.md) |  | [optional] 
**Email** | Pointer to [**[]ViewAccountUsageDataEmailInner**](ViewAccountUsageDataEmailInner.md) |  | [optional] 
**EmailTransactional** | Pointer to [**[]ViewAccountUsageDataEmailInner**](ViewAccountUsageDataEmailInner.md) |  | [optional] 
**Postcards** | Pointer to [**[]ViewAccountUsageDataMmsInner**](ViewAccountUsageDataMmsInner.md) |  | [optional] 
**SmsTotal** | Pointer to [**ViewAccountUsageDataSmsTotal**](ViewAccountUsageDataSmsTotal.md) |  | [optional] 
**VoiceTotal** | Pointer to [**ViewAccountUsageDataSmsTotal**](ViewAccountUsageDataSmsTotal.md) |  | [optional] 
**FaxTotal** | Pointer to [**ViewAccountUsageDataSmsTotal**](ViewAccountUsageDataSmsTotal.md) |  | [optional] 
**PostTotal** | Pointer to [**ViewAccountUsageDataSmsTotal**](ViewAccountUsageDataSmsTotal.md) |  | [optional] 
**EmailTotal** | Pointer to [**ViewAccountUsageDataEmailTotal**](ViewAccountUsageDataEmailTotal.md) |  | [optional] 
**MmsTotal** | Pointer to [**ViewVoiceStatisticsDataTotalOutbound**](ViewVoiceStatisticsDataTotalOutbound.md) |  | [optional] 
**EmailTransactionalTotal** | Pointer to [**ViewVoiceStatisticsDataTotalOutbound**](ViewVoiceStatisticsDataTotalOutbound.md) |  | [optional] 
**PostcardsTotal** | Pointer to [**ViewVoiceStatisticsDataTotalOutbound**](ViewVoiceStatisticsDataTotalOutbound.md) |  | [optional] 
**Currency** | Pointer to [**Currency**](Currency.md) |  | [optional] 

## Methods

### NewViewAccountUsageData

`func NewViewAccountUsageData() *ViewAccountUsageData`

NewViewAccountUsageData instantiates a new ViewAccountUsageData object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewViewAccountUsageDataWithDefaults

`func NewViewAccountUsageDataWithDefaults() *ViewAccountUsageData`

NewViewAccountUsageDataWithDefaults instantiates a new ViewAccountUsageData object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetSms

`func (o *ViewAccountUsageData) GetSms() []ViewAccountUsageDataSmsInner`

GetSms returns the Sms field if non-nil, zero value otherwise.

### GetSmsOk

`func (o *ViewAccountUsageData) GetSmsOk() (*[]ViewAccountUsageDataSmsInner, bool)`

GetSmsOk returns a tuple with the Sms field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSms

`func (o *ViewAccountUsageData) SetSms(v []ViewAccountUsageDataSmsInner)`

SetSms sets Sms field to given value.

### HasSms

`func (o *ViewAccountUsageData) HasSms() bool`

HasSms returns a boolean if a field has been set.

### GetMms

`func (o *ViewAccountUsageData) GetMms() []ViewAccountUsageDataMmsInner`

GetMms returns the Mms field if non-nil, zero value otherwise.

### GetMmsOk

`func (o *ViewAccountUsageData) GetMmsOk() (*[]ViewAccountUsageDataMmsInner, bool)`

GetMmsOk returns a tuple with the Mms field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetMms

`func (o *ViewAccountUsageData) SetMms(v []ViewAccountUsageDataMmsInner)`

SetMms sets Mms field to given value.

### HasMms

`func (o *ViewAccountUsageData) HasMms() bool`

HasMms returns a boolean if a field has been set.

### GetVoice

`func (o *ViewAccountUsageData) GetVoice() []ViewAccountUsageDataMmsInner`

GetVoice returns the Voice field if non-nil, zero value otherwise.

### GetVoiceOk

`func (o *ViewAccountUsageData) GetVoiceOk() (*[]ViewAccountUsageDataMmsInner, bool)`

GetVoiceOk returns a tuple with the Voice field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetVoice

`func (o *ViewAccountUsageData) SetVoice(v []ViewAccountUsageDataMmsInner)`

SetVoice sets Voice field to given value.

### HasVoice

`func (o *ViewAccountUsageData) HasVoice() bool`

HasVoice returns a boolean if a field has been set.

### GetFax

`func (o *ViewAccountUsageData) GetFax() []ViewAccountUsageDataMmsInner`

GetFax returns the Fax field if non-nil, zero value otherwise.

### GetFaxOk

`func (o *ViewAccountUsageData) GetFaxOk() (*[]ViewAccountUsageDataMmsInner, bool)`

GetFaxOk returns a tuple with the Fax field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetFax

`func (o *ViewAccountUsageData) SetFax(v []ViewAccountUsageDataMmsInner)`

SetFax sets Fax field to given value.

### HasFax

`func (o *ViewAccountUsageData) HasFax() bool`

HasFax returns a boolean if a field has been set.

### GetPost

`func (o *ViewAccountUsageData) GetPost() []ViewAccountUsageDataMmsInner`

GetPost returns the Post field if non-nil, zero value otherwise.

### GetPostOk

`func (o *ViewAccountUsageData) GetPostOk() (*[]ViewAccountUsageDataMmsInner, bool)`

GetPostOk returns a tuple with the Post field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetPost

`func (o *ViewAccountUsageData) SetPost(v []ViewAccountUsageDataMmsInner)`

SetPost sets Post field to given value.

### HasPost

`func (o *ViewAccountUsageData) HasPost() bool`

HasPost returns a boolean if a field has been set.

### GetEmail

`func (o *ViewAccountUsageData) GetEmail() []ViewAccountUsageDataEmailInner`

GetEmail returns the Email field if non-nil, zero value otherwise.

### GetEmailOk

`func (o *ViewAccountUsageData) GetEmailOk() (*[]ViewAccountUsageDataEmailInner, bool)`

GetEmailOk returns a tuple with the Email field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetEmail

`func (o *ViewAccountUsageData) SetEmail(v []ViewAccountUsageDataEmailInner)`

SetEmail sets Email field to given value.

### HasEmail

`func (o *ViewAccountUsageData) HasEmail() bool`

HasEmail returns a boolean if a field has been set.

### GetEmailTransactional

`func (o *ViewAccountUsageData) GetEmailTransactional() []ViewAccountUsageDataEmailInner`

GetEmailTransactional returns the EmailTransactional field if non-nil, zero value otherwise.

### GetEmailTransactionalOk

`func (o *ViewAccountUsageData) GetEmailTransactionalOk() (*[]ViewAccountUsageDataEmailInner, bool)`

GetEmailTransactionalOk returns a tuple with the EmailTransactional field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetEmailTransactional

`func (o *ViewAccountUsageData) SetEmailTransactional(v []ViewAccountUsageDataEmailInner)`

SetEmailTransactional sets EmailTransactional field to given value.

### HasEmailTransactional

`func (o *ViewAccountUsageData) HasEmailTransactional() bool`

HasEmailTransactional returns a boolean if a field has been set.

### GetPostcards

`func (o *ViewAccountUsageData) GetPostcards() []ViewAccountUsageDataMmsInner`

GetPostcards returns the Postcards field if non-nil, zero value otherwise.

### GetPostcardsOk

`func (o *ViewAccountUsageData) GetPostcardsOk() (*[]ViewAccountUsageDataMmsInner, bool)`

GetPostcardsOk returns a tuple with the Postcards field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetPostcards

`func (o *ViewAccountUsageData) SetPostcards(v []ViewAccountUsageDataMmsInner)`

SetPostcards sets Postcards field to given value.

### HasPostcards

`func (o *ViewAccountUsageData) HasPostcards() bool`

HasPostcards returns a boolean if a field has been set.

### GetSmsTotal

`func (o *ViewAccountUsageData) GetSmsTotal() ViewAccountUsageDataSmsTotal`

GetSmsTotal returns the SmsTotal field if non-nil, zero value otherwise.

### GetSmsTotalOk

`func (o *ViewAccountUsageData) GetSmsTotalOk() (*ViewAccountUsageDataSmsTotal, bool)`

GetSmsTotalOk returns a tuple with the SmsTotal field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSmsTotal

`func (o *ViewAccountUsageData) SetSmsTotal(v ViewAccountUsageDataSmsTotal)`

SetSmsTotal sets SmsTotal field to given value.

### HasSmsTotal

`func (o *ViewAccountUsageData) HasSmsTotal() bool`

HasSmsTotal returns a boolean if a field has been set.

### GetVoiceTotal

`func (o *ViewAccountUsageData) GetVoiceTotal() ViewAccountUsageDataSmsTotal`

GetVoiceTotal returns the VoiceTotal field if non-nil, zero value otherwise.

### GetVoiceTotalOk

`func (o *ViewAccountUsageData) GetVoiceTotalOk() (*ViewAccountUsageDataSmsTotal, bool)`

GetVoiceTotalOk returns a tuple with the VoiceTotal field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetVoiceTotal

`func (o *ViewAccountUsageData) SetVoiceTotal(v ViewAccountUsageDataSmsTotal)`

SetVoiceTotal sets VoiceTotal field to given value.

### HasVoiceTotal

`func (o *ViewAccountUsageData) HasVoiceTotal() bool`

HasVoiceTotal returns a boolean if a field has been set.

### GetFaxTotal

`func (o *ViewAccountUsageData) GetFaxTotal() ViewAccountUsageDataSmsTotal`

GetFaxTotal returns the FaxTotal field if non-nil, zero value otherwise.

### GetFaxTotalOk

`func (o *ViewAccountUsageData) GetFaxTotalOk() (*ViewAccountUsageDataSmsTotal, bool)`

GetFaxTotalOk returns a tuple with the FaxTotal field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetFaxTotal

`func (o *ViewAccountUsageData) SetFaxTotal(v ViewAccountUsageDataSmsTotal)`

SetFaxTotal sets FaxTotal field to given value.

### HasFaxTotal

`func (o *ViewAccountUsageData) HasFaxTotal() bool`

HasFaxTotal returns a boolean if a field has been set.

### GetPostTotal

`func (o *ViewAccountUsageData) GetPostTotal() ViewAccountUsageDataSmsTotal`

GetPostTotal returns the PostTotal field if non-nil, zero value otherwise.

### GetPostTotalOk

`func (o *ViewAccountUsageData) GetPostTotalOk() (*ViewAccountUsageDataSmsTotal, bool)`

GetPostTotalOk returns a tuple with the PostTotal field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetPostTotal

`func (o *ViewAccountUsageData) SetPostTotal(v ViewAccountUsageDataSmsTotal)`

SetPostTotal sets PostTotal field to given value.

### HasPostTotal

`func (o *ViewAccountUsageData) HasPostTotal() bool`

HasPostTotal returns a boolean if a field has been set.

### GetEmailTotal

`func (o *ViewAccountUsageData) GetEmailTotal() ViewAccountUsageDataEmailTotal`

GetEmailTotal returns the EmailTotal field if non-nil, zero value otherwise.

### GetEmailTotalOk

`func (o *ViewAccountUsageData) GetEmailTotalOk() (*ViewAccountUsageDataEmailTotal, bool)`

GetEmailTotalOk returns a tuple with the EmailTotal field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetEmailTotal

`func (o *ViewAccountUsageData) SetEmailTotal(v ViewAccountUsageDataEmailTotal)`

SetEmailTotal sets EmailTotal field to given value.

### HasEmailTotal

`func (o *ViewAccountUsageData) HasEmailTotal() bool`

HasEmailTotal returns a boolean if a field has been set.

### GetMmsTotal

`func (o *ViewAccountUsageData) GetMmsTotal() ViewVoiceStatisticsDataTotalOutbound`

GetMmsTotal returns the MmsTotal field if non-nil, zero value otherwise.

### GetMmsTotalOk

`func (o *ViewAccountUsageData) GetMmsTotalOk() (*ViewVoiceStatisticsDataTotalOutbound, bool)`

GetMmsTotalOk returns a tuple with the MmsTotal field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetMmsTotal

`func (o *ViewAccountUsageData) SetMmsTotal(v ViewVoiceStatisticsDataTotalOutbound)`

SetMmsTotal sets MmsTotal field to given value.

### HasMmsTotal

`func (o *ViewAccountUsageData) HasMmsTotal() bool`

HasMmsTotal returns a boolean if a field has been set.

### GetEmailTransactionalTotal

`func (o *ViewAccountUsageData) GetEmailTransactionalTotal() ViewVoiceStatisticsDataTotalOutbound`

GetEmailTransactionalTotal returns the EmailTransactionalTotal field if non-nil, zero value otherwise.

### GetEmailTransactionalTotalOk

`func (o *ViewAccountUsageData) GetEmailTransactionalTotalOk() (*ViewVoiceStatisticsDataTotalOutbound, bool)`

GetEmailTransactionalTotalOk returns a tuple with the EmailTransactionalTotal field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetEmailTransactionalTotal

`func (o *ViewAccountUsageData) SetEmailTransactionalTotal(v ViewVoiceStatisticsDataTotalOutbound)`

SetEmailTransactionalTotal sets EmailTransactionalTotal field to given value.

### HasEmailTransactionalTotal

`func (o *ViewAccountUsageData) HasEmailTransactionalTotal() bool`

HasEmailTransactionalTotal returns a boolean if a field has been set.

### GetPostcardsTotal

`func (o *ViewAccountUsageData) GetPostcardsTotal() ViewVoiceStatisticsDataTotalOutbound`

GetPostcardsTotal returns the PostcardsTotal field if non-nil, zero value otherwise.

### GetPostcardsTotalOk

`func (o *ViewAccountUsageData) GetPostcardsTotalOk() (*ViewVoiceStatisticsDataTotalOutbound, bool)`

GetPostcardsTotalOk returns a tuple with the PostcardsTotal field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetPostcardsTotal

`func (o *ViewAccountUsageData) SetPostcardsTotal(v ViewVoiceStatisticsDataTotalOutbound)`

SetPostcardsTotal sets PostcardsTotal field to given value.

### HasPostcardsTotal

`func (o *ViewAccountUsageData) HasPostcardsTotal() bool`

HasPostcardsTotal returns a boolean if a field has been set.

### GetCurrency

`func (o *ViewAccountUsageData) GetCurrency() Currency`

GetCurrency returns the Currency field if non-nil, zero value otherwise.

### GetCurrencyOk

`func (o *ViewAccountUsageData) GetCurrencyOk() (*Currency, bool)`

GetCurrencyOk returns a tuple with the Currency field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCurrency

`func (o *ViewAccountUsageData) SetCurrency(v Currency)`

SetCurrency sets Currency field to given value.

### HasCurrency

`func (o *ViewAccountUsageData) HasCurrency() bool`

HasCurrency returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


