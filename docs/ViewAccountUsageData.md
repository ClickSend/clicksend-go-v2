# ViewAccountUsageData

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Sms** | Pointer to [**[]ViewAccountUsageDataSmsInner**](ViewAccountUsageDataSmsInner.md) |  | [optional] 
**Voice** | Pointer to [**[]ViewAccountUsageDataSmsInner**](ViewAccountUsageDataSmsInner.md) |  | [optional] 
**Fax** | Pointer to [**[]ViewAccountUsageDataSmsInner**](ViewAccountUsageDataSmsInner.md) |  | [optional] 
**Post** | Pointer to [**[]ViewAccountUsageDataSmsInner**](ViewAccountUsageDataSmsInner.md) |  | [optional] 
**Email** | Pointer to [**[]ViewAccountUsageDataEmailInner**](ViewAccountUsageDataEmailInner.md) |  | [optional] 
**SmsTotal** | Pointer to [**ViewAccountUsageDataSmsTotal**](ViewAccountUsageDataSmsTotal.md) |  | [optional] 
**VoiceTotal** | Pointer to [**ViewAccountUsageDataSmsTotal**](ViewAccountUsageDataSmsTotal.md) |  | [optional] 
**FaxTotal** | Pointer to [**ViewAccountUsageDataSmsTotal**](ViewAccountUsageDataSmsTotal.md) |  | [optional] 
**PostTotal** | Pointer to [**ViewAccountUsageDataSmsTotal**](ViewAccountUsageDataSmsTotal.md) |  | [optional] 
**EmailTotal** | Pointer to [**ViewVoiceStatisticsDataTotalOutbound**](ViewVoiceStatisticsDataTotalOutbound.md) |  | [optional] 

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

### GetVoice

`func (o *ViewAccountUsageData) GetVoice() []ViewAccountUsageDataSmsInner`

GetVoice returns the Voice field if non-nil, zero value otherwise.

### GetVoiceOk

`func (o *ViewAccountUsageData) GetVoiceOk() (*[]ViewAccountUsageDataSmsInner, bool)`

GetVoiceOk returns a tuple with the Voice field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetVoice

`func (o *ViewAccountUsageData) SetVoice(v []ViewAccountUsageDataSmsInner)`

SetVoice sets Voice field to given value.

### HasVoice

`func (o *ViewAccountUsageData) HasVoice() bool`

HasVoice returns a boolean if a field has been set.

### GetFax

`func (o *ViewAccountUsageData) GetFax() []ViewAccountUsageDataSmsInner`

GetFax returns the Fax field if non-nil, zero value otherwise.

### GetFaxOk

`func (o *ViewAccountUsageData) GetFaxOk() (*[]ViewAccountUsageDataSmsInner, bool)`

GetFaxOk returns a tuple with the Fax field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetFax

`func (o *ViewAccountUsageData) SetFax(v []ViewAccountUsageDataSmsInner)`

SetFax sets Fax field to given value.

### HasFax

`func (o *ViewAccountUsageData) HasFax() bool`

HasFax returns a boolean if a field has been set.

### GetPost

`func (o *ViewAccountUsageData) GetPost() []ViewAccountUsageDataSmsInner`

GetPost returns the Post field if non-nil, zero value otherwise.

### GetPostOk

`func (o *ViewAccountUsageData) GetPostOk() (*[]ViewAccountUsageDataSmsInner, bool)`

GetPostOk returns a tuple with the Post field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetPost

`func (o *ViewAccountUsageData) SetPost(v []ViewAccountUsageDataSmsInner)`

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

`func (o *ViewAccountUsageData) GetEmailTotal() ViewVoiceStatisticsDataTotalOutbound`

GetEmailTotal returns the EmailTotal field if non-nil, zero value otherwise.

### GetEmailTotalOk

`func (o *ViewAccountUsageData) GetEmailTotalOk() (*ViewVoiceStatisticsDataTotalOutbound, bool)`

GetEmailTotalOk returns a tuple with the EmailTotal field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetEmailTotal

`func (o *ViewAccountUsageData) SetEmailTotal(v ViewVoiceStatisticsDataTotalOutbound)`

SetEmailTotal sets EmailTotal field to given value.

### HasEmailTotal

`func (o *ViewAccountUsageData) HasEmailTotal() bool`

HasEmailTotal returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


