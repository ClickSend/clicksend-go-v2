# VoiceMessage

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Date** | Pointer to **NullableString** | The date, if applicable. May be null; see also &#x60;date_added&#x60;. | [optional] 
**DateAdded** | Pointer to **int32** | The Unix timestamp when the message was added. | [optional] 
**ListId** | Pointer to **NullableString** | The ID of the list associated with the message, if applicable. | [optional] 
**To** | Pointer to **string** | The recipient&#39;s phone number. | [optional] 
**ToType** | Pointer to **string** | The type of recipient. | [optional] 
**Body** | Pointer to **string** | The body of the message. | [optional] 
**From** | Pointer to **NullableString** | The sender&#39;s phone number. | [optional] 
**Lang** | Pointer to **string** | The language of the message. | [optional] 
**Voice** | Pointer to **string** | The voice of the message. | [optional] 
**Schedule** | Pointer to [**VoiceMessageSchedule**](VoiceMessageSchedule.md) |  | [optional] 
**MessageId** | Pointer to **string** | The ID of the message. | [optional] 
**MessageParts** | Pointer to **int32** | The number of parts in the message. | [optional] 
**MessagePrice** | Pointer to **string** | The price of the message. | [optional] 
**CustomString** | Pointer to **string** | The custom string of the message. | [optional] 
**UserId** | Pointer to **float32** | The ID of the user. | [optional] 
**SubaccountId** | Pointer to **float32** | The ID of the subaccount. | [optional] 
**Country** | Pointer to **string** | The country code of the message. | [optional] 
**RequireInput** | Pointer to **float32** | The require input of the message. | [optional] 
**MachineDetection** | Pointer to **float32** | The machine detection of the message. | [optional] 
**MachineDetected** | Pointer to **NullableFloat32** | Flag indicating if an answering machine was detected. | [optional] 
**Digits** | Pointer to **NullableString** | The digits entered by the recipient, if any input was collected. | [optional] 
**Carrier** | Pointer to **NullableString** | The carrier of the recipient&#39;s phone number. | [optional] 
**StatusCode** | Pointer to **NullableString** | The status code of the message. | [optional] 
**StatusText** | Pointer to **NullableString** | A human-readable description of the status. | [optional] 
**Status** | Pointer to **string** | The status of the message. | [optional] 
**ApiUsername** | Pointer to **string** | The API username associated with the message. | [optional] 

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

`func (o *VoiceMessage) GetDate() string`

GetDate returns the Date field if non-nil, zero value otherwise.

### GetDateOk

`func (o *VoiceMessage) GetDateOk() (*string, bool)`

GetDateOk returns a tuple with the Date field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDate

`func (o *VoiceMessage) SetDate(v string)`

SetDate sets Date field to given value.

### HasDate

`func (o *VoiceMessage) HasDate() bool`

HasDate returns a boolean if a field has been set.

### SetDateNil

`func (o *VoiceMessage) SetDateNil(b bool)`

 SetDateNil sets the value for Date to be an explicit nil

### UnsetDate
`func (o *VoiceMessage) UnsetDate()`

UnsetDate ensures that no value is present for Date, not even an explicit nil
### GetDateAdded

`func (o *VoiceMessage) GetDateAdded() int32`

GetDateAdded returns the DateAdded field if non-nil, zero value otherwise.

### GetDateAddedOk

`func (o *VoiceMessage) GetDateAddedOk() (*int32, bool)`

GetDateAddedOk returns a tuple with the DateAdded field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDateAdded

`func (o *VoiceMessage) SetDateAdded(v int32)`

SetDateAdded sets DateAdded field to given value.

### HasDateAdded

`func (o *VoiceMessage) HasDateAdded() bool`

HasDateAdded returns a boolean if a field has been set.

### GetListId

`func (o *VoiceMessage) GetListId() string`

GetListId returns the ListId field if non-nil, zero value otherwise.

### GetListIdOk

`func (o *VoiceMessage) GetListIdOk() (*string, bool)`

GetListIdOk returns a tuple with the ListId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetListId

`func (o *VoiceMessage) SetListId(v string)`

SetListId sets ListId field to given value.

### HasListId

`func (o *VoiceMessage) HasListId() bool`

HasListId returns a boolean if a field has been set.

### SetListIdNil

`func (o *VoiceMessage) SetListIdNil(b bool)`

 SetListIdNil sets the value for ListId to be an explicit nil

### UnsetListId
`func (o *VoiceMessage) UnsetListId()`

UnsetListId ensures that no value is present for ListId, not even an explicit nil
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

`func (o *VoiceMessage) GetSchedule() VoiceMessageSchedule`

GetSchedule returns the Schedule field if non-nil, zero value otherwise.

### GetScheduleOk

`func (o *VoiceMessage) GetScheduleOk() (*VoiceMessageSchedule, bool)`

GetScheduleOk returns a tuple with the Schedule field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSchedule

`func (o *VoiceMessage) SetSchedule(v VoiceMessageSchedule)`

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

`func (o *VoiceMessage) GetMessageParts() int32`

GetMessageParts returns the MessageParts field if non-nil, zero value otherwise.

### GetMessagePartsOk

`func (o *VoiceMessage) GetMessagePartsOk() (*int32, bool)`

GetMessagePartsOk returns a tuple with the MessageParts field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetMessageParts

`func (o *VoiceMessage) SetMessageParts(v int32)`

SetMessageParts sets MessageParts field to given value.

### HasMessageParts

`func (o *VoiceMessage) HasMessageParts() bool`

HasMessageParts returns a boolean if a field has been set.

### GetMessagePrice

`func (o *VoiceMessage) GetMessagePrice() string`

GetMessagePrice returns the MessagePrice field if non-nil, zero value otherwise.

### GetMessagePriceOk

`func (o *VoiceMessage) GetMessagePriceOk() (*string, bool)`

GetMessagePriceOk returns a tuple with the MessagePrice field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetMessagePrice

`func (o *VoiceMessage) SetMessagePrice(v string)`

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

### GetMachineDetected

`func (o *VoiceMessage) GetMachineDetected() float32`

GetMachineDetected returns the MachineDetected field if non-nil, zero value otherwise.

### GetMachineDetectedOk

`func (o *VoiceMessage) GetMachineDetectedOk() (*float32, bool)`

GetMachineDetectedOk returns a tuple with the MachineDetected field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetMachineDetected

`func (o *VoiceMessage) SetMachineDetected(v float32)`

SetMachineDetected sets MachineDetected field to given value.

### HasMachineDetected

`func (o *VoiceMessage) HasMachineDetected() bool`

HasMachineDetected returns a boolean if a field has been set.

### SetMachineDetectedNil

`func (o *VoiceMessage) SetMachineDetectedNil(b bool)`

 SetMachineDetectedNil sets the value for MachineDetected to be an explicit nil

### UnsetMachineDetected
`func (o *VoiceMessage) UnsetMachineDetected()`

UnsetMachineDetected ensures that no value is present for MachineDetected, not even an explicit nil
### GetDigits

`func (o *VoiceMessage) GetDigits() string`

GetDigits returns the Digits field if non-nil, zero value otherwise.

### GetDigitsOk

`func (o *VoiceMessage) GetDigitsOk() (*string, bool)`

GetDigitsOk returns a tuple with the Digits field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDigits

`func (o *VoiceMessage) SetDigits(v string)`

SetDigits sets Digits field to given value.

### HasDigits

`func (o *VoiceMessage) HasDigits() bool`

HasDigits returns a boolean if a field has been set.

### SetDigitsNil

`func (o *VoiceMessage) SetDigitsNil(b bool)`

 SetDigitsNil sets the value for Digits to be an explicit nil

### UnsetDigits
`func (o *VoiceMessage) UnsetDigits()`

UnsetDigits ensures that no value is present for Digits, not even an explicit nil
### GetCarrier

`func (o *VoiceMessage) GetCarrier() string`

GetCarrier returns the Carrier field if non-nil, zero value otherwise.

### GetCarrierOk

`func (o *VoiceMessage) GetCarrierOk() (*string, bool)`

GetCarrierOk returns a tuple with the Carrier field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCarrier

`func (o *VoiceMessage) SetCarrier(v string)`

SetCarrier sets Carrier field to given value.

### HasCarrier

`func (o *VoiceMessage) HasCarrier() bool`

HasCarrier returns a boolean if a field has been set.

### SetCarrierNil

`func (o *VoiceMessage) SetCarrierNil(b bool)`

 SetCarrierNil sets the value for Carrier to be an explicit nil

### UnsetCarrier
`func (o *VoiceMessage) UnsetCarrier()`

UnsetCarrier ensures that no value is present for Carrier, not even an explicit nil
### GetStatusCode

`func (o *VoiceMessage) GetStatusCode() string`

GetStatusCode returns the StatusCode field if non-nil, zero value otherwise.

### GetStatusCodeOk

`func (o *VoiceMessage) GetStatusCodeOk() (*string, bool)`

GetStatusCodeOk returns a tuple with the StatusCode field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetStatusCode

`func (o *VoiceMessage) SetStatusCode(v string)`

SetStatusCode sets StatusCode field to given value.

### HasStatusCode

`func (o *VoiceMessage) HasStatusCode() bool`

HasStatusCode returns a boolean if a field has been set.

### SetStatusCodeNil

`func (o *VoiceMessage) SetStatusCodeNil(b bool)`

 SetStatusCodeNil sets the value for StatusCode to be an explicit nil

### UnsetStatusCode
`func (o *VoiceMessage) UnsetStatusCode()`

UnsetStatusCode ensures that no value is present for StatusCode, not even an explicit nil
### GetStatusText

`func (o *VoiceMessage) GetStatusText() string`

GetStatusText returns the StatusText field if non-nil, zero value otherwise.

### GetStatusTextOk

`func (o *VoiceMessage) GetStatusTextOk() (*string, bool)`

GetStatusTextOk returns a tuple with the StatusText field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetStatusText

`func (o *VoiceMessage) SetStatusText(v string)`

SetStatusText sets StatusText field to given value.

### HasStatusText

`func (o *VoiceMessage) HasStatusText() bool`

HasStatusText returns a boolean if a field has been set.

### SetStatusTextNil

`func (o *VoiceMessage) SetStatusTextNil(b bool)`

 SetStatusTextNil sets the value for StatusText to be an explicit nil

### UnsetStatusText
`func (o *VoiceMessage) UnsetStatusText()`

UnsetStatusText ensures that no value is present for StatusText, not even an explicit nil
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

### GetApiUsername

`func (o *VoiceMessage) GetApiUsername() string`

GetApiUsername returns the ApiUsername field if non-nil, zero value otherwise.

### GetApiUsernameOk

`func (o *VoiceMessage) GetApiUsernameOk() (*string, bool)`

GetApiUsernameOk returns a tuple with the ApiUsername field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetApiUsername

`func (o *VoiceMessage) SetApiUsername(v string)`

SetApiUsername sets ApiUsername field to given value.

### HasApiUsername

`func (o *VoiceMessage) HasApiUsername() bool`

HasApiUsername returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


