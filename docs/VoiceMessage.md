# VoiceMessage

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Date** | Pointer to **float32** | The date. | [optional] 
**To** | Pointer to **string** | The recipient&#39;s phone number. | [optional] 
**ToType** | Pointer to **string** | The type of recipient. | [optional] 
**Body** | Pointer to **string** | The body of the message. | [optional] 
**From** | Pointer to **NullableString** | The sender&#39;s phone number. | [optional] 
**Lang** | Pointer to **string** | The language of the message. | [optional] 
**Voice** | Pointer to **string** | The voice of the message. | [optional] 
**Schedule** | Pointer to **float32** | The timestamp when the message should be sent. | [optional] 
**MessageId** | Pointer to **string** | The ID of the message. | [optional] 
**MessageParts** | Pointer to **float32** | The number of parts in the message. | [optional] 
**MessagePrice** | Pointer to **float32** | The price of the message. | [optional] 
**CustomString** | Pointer to **string** | The custom string of the message. | [optional] 
**UserId** | Pointer to **float32** | The ID of the user. | [optional] 
**SubaccountId** | Pointer to **float32** | The ID of the subaccount. | [optional] 
**Country** | Pointer to **string** | The country code of the message. | [optional] 
**RequireInput** | Pointer to **float32** | The require input of the message. | [optional] 
**MachineDetection** | Pointer to **float32** | The machine detection of the message. | [optional] 
**Status** | Pointer to **string** | The status of the message. | [optional] 

## Methods

### NewVoiceMessage

`func NewVoiceMessage() *VoiceMessage`

NewVoiceMessage instantiates a new VoiceMessage object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewVoiceMessageWithDefaults

`func NewVoiceMessageWithDefaults() *VoiceMessage`

NewVoiceMessageWithDefaults instantiates a new VoiceMessage object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetDate

`func (o *VoiceMessage) GetDate() float32`

GetDate returns the Date field if non-nil, zero value otherwise.

### GetDateOk

`func (o *VoiceMessage) GetDateOk() (*float32, bool)`

GetDateOk returns a tuple with the Date field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDate

`func (o *VoiceMessage) SetDate(v float32)`

SetDate sets Date field to given value.

### HasDate

`func (o *VoiceMessage) HasDate() bool`

HasDate returns a boolean if a field has been set.

### GetTo

`func (o *VoiceMessage) GetTo() string`

GetTo returns the To field if non-nil, zero value otherwise.

### GetToOk

`func (o *VoiceMessage) GetToOk() (*string, bool)`

GetToOk returns a tuple with the To field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTo

`func (o *VoiceMessage) SetTo(v string)`

SetTo sets To field to given value.

### HasTo

`func (o *VoiceMessage) HasTo() bool`

HasTo returns a boolean if a field has been set.

### GetToType

`func (o *VoiceMessage) GetToType() string`

GetToType returns the ToType field if non-nil, zero value otherwise.

### GetToTypeOk

`func (o *VoiceMessage) GetToTypeOk() (*string, bool)`

GetToTypeOk returns a tuple with the ToType field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetToType

`func (o *VoiceMessage) SetToType(v string)`

SetToType sets ToType field to given value.

### HasToType

`func (o *VoiceMessage) HasToType() bool`

HasToType returns a boolean if a field has been set.

### GetBody

`func (o *VoiceMessage) GetBody() string`

GetBody returns the Body field if non-nil, zero value otherwise.

### GetBodyOk

`func (o *VoiceMessage) GetBodyOk() (*string, bool)`

GetBodyOk returns a tuple with the Body field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetBody

`func (o *VoiceMessage) SetBody(v string)`

SetBody sets Body field to given value.

### HasBody

`func (o *VoiceMessage) HasBody() bool`

HasBody returns a boolean if a field has been set.

### GetFrom

`func (o *VoiceMessage) GetFrom() string`

GetFrom returns the From field if non-nil, zero value otherwise.

### GetFromOk

`func (o *VoiceMessage) GetFromOk() (*string, bool)`

GetFromOk returns a tuple with the From field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetFrom

`func (o *VoiceMessage) SetFrom(v string)`

SetFrom sets From field to given value.

### HasFrom

`func (o *VoiceMessage) HasFrom() bool`

HasFrom returns a boolean if a field has been set.

### SetFromNil

`func (o *VoiceMessage) SetFromNil(b bool)`

 SetFromNil sets the value for From to be an explicit nil

### UnsetFrom
`func (o *VoiceMessage) UnsetFrom()`

UnsetFrom ensures that no value is present for From, not even an explicit nil
### GetLang

`func (o *VoiceMessage) GetLang() string`

GetLang returns the Lang field if non-nil, zero value otherwise.

### GetLangOk

`func (o *VoiceMessage) GetLangOk() (*string, bool)`

GetLangOk returns a tuple with the Lang field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetLang

`func (o *VoiceMessage) SetLang(v string)`

SetLang sets Lang field to given value.

### HasLang

`func (o *VoiceMessage) HasLang() bool`

HasLang returns a boolean if a field has been set.

### GetVoice

`func (o *VoiceMessage) GetVoice() string`

GetVoice returns the Voice field if non-nil, zero value otherwise.

### GetVoiceOk

`func (o *VoiceMessage) GetVoiceOk() (*string, bool)`

GetVoiceOk returns a tuple with the Voice field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetVoice

`func (o *VoiceMessage) SetVoice(v string)`

SetVoice sets Voice field to given value.

### HasVoice

`func (o *VoiceMessage) HasVoice() bool`

HasVoice returns a boolean if a field has been set.

### GetSchedule

`func (o *VoiceMessage) GetSchedule() float32`

GetSchedule returns the Schedule field if non-nil, zero value otherwise.

### GetScheduleOk

`func (o *VoiceMessage) GetScheduleOk() (*float32, bool)`

GetScheduleOk returns a tuple with the Schedule field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSchedule

`func (o *VoiceMessage) SetSchedule(v float32)`

SetSchedule sets Schedule field to given value.

### HasSchedule

`func (o *VoiceMessage) HasSchedule() bool`

HasSchedule returns a boolean if a field has been set.

### GetMessageId

`func (o *VoiceMessage) GetMessageId() string`

GetMessageId returns the MessageId field if non-nil, zero value otherwise.

### GetMessageIdOk

`func (o *VoiceMessage) GetMessageIdOk() (*string, bool)`

GetMessageIdOk returns a tuple with the MessageId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetMessageId

`func (o *VoiceMessage) SetMessageId(v string)`

SetMessageId sets MessageId field to given value.

### HasMessageId

`func (o *VoiceMessage) HasMessageId() bool`

HasMessageId returns a boolean if a field has been set.

### GetMessageParts

`func (o *VoiceMessage) GetMessageParts() float32`

GetMessageParts returns the MessageParts field if non-nil, zero value otherwise.

### GetMessagePartsOk

`func (o *VoiceMessage) GetMessagePartsOk() (*float32, bool)`

GetMessagePartsOk returns a tuple with the MessageParts field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetMessageParts

`func (o *VoiceMessage) SetMessageParts(v float32)`

SetMessageParts sets MessageParts field to given value.

### HasMessageParts

`func (o *VoiceMessage) HasMessageParts() bool`

HasMessageParts returns a boolean if a field has been set.

### GetMessagePrice

`func (o *VoiceMessage) GetMessagePrice() float32`

GetMessagePrice returns the MessagePrice field if non-nil, zero value otherwise.

### GetMessagePriceOk

`func (o *VoiceMessage) GetMessagePriceOk() (*float32, bool)`

GetMessagePriceOk returns a tuple with the MessagePrice field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetMessagePrice

`func (o *VoiceMessage) SetMessagePrice(v float32)`

SetMessagePrice sets MessagePrice field to given value.

### HasMessagePrice

`func (o *VoiceMessage) HasMessagePrice() bool`

HasMessagePrice returns a boolean if a field has been set.

### GetCustomString

`func (o *VoiceMessage) GetCustomString() string`

GetCustomString returns the CustomString field if non-nil, zero value otherwise.

### GetCustomStringOk

`func (o *VoiceMessage) GetCustomStringOk() (*string, bool)`

GetCustomStringOk returns a tuple with the CustomString field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCustomString

`func (o *VoiceMessage) SetCustomString(v string)`

SetCustomString sets CustomString field to given value.

### HasCustomString

`func (o *VoiceMessage) HasCustomString() bool`

HasCustomString returns a boolean if a field has been set.

### GetUserId

`func (o *VoiceMessage) GetUserId() float32`

GetUserId returns the UserId field if non-nil, zero value otherwise.

### GetUserIdOk

`func (o *VoiceMessage) GetUserIdOk() (*float32, bool)`

GetUserIdOk returns a tuple with the UserId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetUserId

`func (o *VoiceMessage) SetUserId(v float32)`

SetUserId sets UserId field to given value.

### HasUserId

`func (o *VoiceMessage) HasUserId() bool`

HasUserId returns a boolean if a field has been set.

### GetSubaccountId

`func (o *VoiceMessage) GetSubaccountId() float32`

GetSubaccountId returns the SubaccountId field if non-nil, zero value otherwise.

### GetSubaccountIdOk

`func (o *VoiceMessage) GetSubaccountIdOk() (*float32, bool)`

GetSubaccountIdOk returns a tuple with the SubaccountId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSubaccountId

`func (o *VoiceMessage) SetSubaccountId(v float32)`

SetSubaccountId sets SubaccountId field to given value.

### HasSubaccountId

`func (o *VoiceMessage) HasSubaccountId() bool`

HasSubaccountId returns a boolean if a field has been set.

### GetCountry

`func (o *VoiceMessage) GetCountry() string`

GetCountry returns the Country field if non-nil, zero value otherwise.

### GetCountryOk

`func (o *VoiceMessage) GetCountryOk() (*string, bool)`

GetCountryOk returns a tuple with the Country field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCountry

`func (o *VoiceMessage) SetCountry(v string)`

SetCountry sets Country field to given value.

### HasCountry

`func (o *VoiceMessage) HasCountry() bool`

HasCountry returns a boolean if a field has been set.

### GetRequireInput

`func (o *VoiceMessage) GetRequireInput() float32`

GetRequireInput returns the RequireInput field if non-nil, zero value otherwise.

### GetRequireInputOk

`func (o *VoiceMessage) GetRequireInputOk() (*float32, bool)`

GetRequireInputOk returns a tuple with the RequireInput field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetRequireInput

`func (o *VoiceMessage) SetRequireInput(v float32)`

SetRequireInput sets RequireInput field to given value.

### HasRequireInput

`func (o *VoiceMessage) HasRequireInput() bool`

HasRequireInput returns a boolean if a field has been set.

### GetMachineDetection

`func (o *VoiceMessage) GetMachineDetection() float32`

GetMachineDetection returns the MachineDetection field if non-nil, zero value otherwise.

### GetMachineDetectionOk

`func (o *VoiceMessage) GetMachineDetectionOk() (*float32, bool)`

GetMachineDetectionOk returns a tuple with the MachineDetection field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetMachineDetection

`func (o *VoiceMessage) SetMachineDetection(v float32)`

SetMachineDetection sets MachineDetection field to given value.

### HasMachineDetection

`func (o *VoiceMessage) HasMachineDetection() bool`

HasMachineDetection returns a boolean if a field has been set.

### GetStatus

`func (o *VoiceMessage) GetStatus() string`

GetStatus returns the Status field if non-nil, zero value otherwise.

### GetStatusOk

`func (o *VoiceMessage) GetStatusOk() (*string, bool)`

GetStatusOk returns a tuple with the Status field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetStatus

`func (o *VoiceMessage) SetStatus(v string)`

SetStatus sets Status field to given value.

### HasStatus

`func (o *VoiceMessage) HasStatus() bool`

HasStatus returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


