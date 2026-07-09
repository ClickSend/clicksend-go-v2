# Mms

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**ListId** | Pointer to **NullableString** | The ID of the list (if applicable). | [optional] 
**ContactId** | Pointer to **int32** | The ID of the contact. | [optional] 
**MessageId** | Pointer to **string** | The ID of the message. | [optional] 
**To** | Pointer to **string** | The recipient of the message. | [optional] 
**Subject** | Pointer to **string** | The subject of the message. | [optional] 
**From** | Pointer to **string** | The sender of the message. | [optional] 
**Body** | Pointer to **string** | The body of the message. | [optional] 
**Country** | Pointer to **string** | The country code. | [optional] 
**CustomString** | Pointer to **string** | Custom string associated with the message. | [optional] 
**Schedule** | Pointer to **string** | The schedule time of the message. | [optional] 
**MessageParts** | Pointer to **int32** | The number of parts the message was split into. | [optional] 
**MessagePrice** | Pointer to **string** | The price of the message. | [optional] 
**MediaFileUrl** | Pointer to **string** | The URL of the media file attached to the message. | [optional] 
**Status** | Pointer to **string** | The status of the message. | [optional] 

## Methods

### NewMms

`func NewMms() *Mms`

NewMms instantiates a new Mms object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewMmsWithDefaults

`func NewMmsWithDefaults() *Mms`

NewMmsWithDefaults instantiates a new Mms object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetListId

`func (o *Mms) GetListId() string`

GetListId returns the ListId field if non-nil, zero value otherwise.

### GetListIdOk

`func (o *Mms) GetListIdOk() (*string, bool)`

GetListIdOk returns a tuple with the ListId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetListId

`func (o *Mms) SetListId(v string)`

SetListId sets ListId field to given value.

### HasListId

`func (o *Mms) HasListId() bool`

HasListId returns a boolean if a field has been set.

### SetListIdNil

`func (o *Mms) SetListIdNil(b bool)`

 SetListIdNil sets the value for ListId to be an explicit nil

### UnsetListId
`func (o *Mms) UnsetListId()`

UnsetListId ensures that no value is present for ListId, not even an explicit nil
### GetContactId

`func (o *Mms) GetContactId() int32`

GetContactId returns the ContactId field if non-nil, zero value otherwise.

### GetContactIdOk

`func (o *Mms) GetContactIdOk() (*int32, bool)`

GetContactIdOk returns a tuple with the ContactId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetContactId

`func (o *Mms) SetContactId(v int32)`

SetContactId sets ContactId field to given value.

### HasContactId

`func (o *Mms) HasContactId() bool`

HasContactId returns a boolean if a field has been set.

### GetMessageId

`func (o *Mms) GetMessageId() string`

GetMessageId returns the MessageId field if non-nil, zero value otherwise.

### GetMessageIdOk

`func (o *Mms) GetMessageIdOk() (*string, bool)`

GetMessageIdOk returns a tuple with the MessageId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetMessageId

`func (o *Mms) SetMessageId(v string)`

SetMessageId sets MessageId field to given value.

### HasMessageId

`func (o *Mms) HasMessageId() bool`

HasMessageId returns a boolean if a field has been set.

### GetTo

`func (o *Mms) GetTo() string`

GetTo returns the To field if non-nil, zero value otherwise.

### GetToOk

`func (o *Mms) GetToOk() (*string, bool)`

GetToOk returns a tuple with the To field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTo

`func (o *Mms) SetTo(v string)`

SetTo sets To field to given value.

### HasTo

`func (o *Mms) HasTo() bool`

HasTo returns a boolean if a field has been set.

### GetSubject

`func (o *Mms) GetSubject() string`

GetSubject returns the Subject field if non-nil, zero value otherwise.

### GetSubjectOk

`func (o *Mms) GetSubjectOk() (*string, bool)`

GetSubjectOk returns a tuple with the Subject field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSubject

`func (o *Mms) SetSubject(v string)`

SetSubject sets Subject field to given value.

### HasSubject

`func (o *Mms) HasSubject() bool`

HasSubject returns a boolean if a field has been set.

### GetFrom

`func (o *Mms) GetFrom() string`

GetFrom returns the From field if non-nil, zero value otherwise.

### GetFromOk

`func (o *Mms) GetFromOk() (*string, bool)`

GetFromOk returns a tuple with the From field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetFrom

`func (o *Mms) SetFrom(v string)`

SetFrom sets From field to given value.

### HasFrom

`func (o *Mms) HasFrom() bool`

HasFrom returns a boolean if a field has been set.

### GetBody

`func (o *Mms) GetBody() string`

GetBody returns the Body field if non-nil, zero value otherwise.

### GetBodyOk

`func (o *Mms) GetBodyOk() (*string, bool)`

GetBodyOk returns a tuple with the Body field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetBody

`func (o *Mms) SetBody(v string)`

SetBody sets Body field to given value.

### HasBody

`func (o *Mms) HasBody() bool`

HasBody returns a boolean if a field has been set.

### GetCountry

`func (o *Mms) GetCountry() string`

GetCountry returns the Country field if non-nil, zero value otherwise.

### GetCountryOk

`func (o *Mms) GetCountryOk() (*string, bool)`

GetCountryOk returns a tuple with the Country field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCountry

`func (o *Mms) SetCountry(v string)`

SetCountry sets Country field to given value.

### HasCountry

`func (o *Mms) HasCountry() bool`

HasCountry returns a boolean if a field has been set.

### GetCustomString

`func (o *Mms) GetCustomString() string`

GetCustomString returns the CustomString field if non-nil, zero value otherwise.

### GetCustomStringOk

`func (o *Mms) GetCustomStringOk() (*string, bool)`

GetCustomStringOk returns a tuple with the CustomString field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCustomString

`func (o *Mms) SetCustomString(v string)`

SetCustomString sets CustomString field to given value.

### HasCustomString

`func (o *Mms) HasCustomString() bool`

HasCustomString returns a boolean if a field has been set.

### GetSchedule

`func (o *Mms) GetSchedule() string`

GetSchedule returns the Schedule field if non-nil, zero value otherwise.

### GetScheduleOk

`func (o *Mms) GetScheduleOk() (*string, bool)`

GetScheduleOk returns a tuple with the Schedule field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSchedule

`func (o *Mms) SetSchedule(v string)`

SetSchedule sets Schedule field to given value.

### HasSchedule

`func (o *Mms) HasSchedule() bool`

HasSchedule returns a boolean if a field has been set.

### GetMessageParts

`func (o *Mms) GetMessageParts() int32`

GetMessageParts returns the MessageParts field if non-nil, zero value otherwise.

### GetMessagePartsOk

`func (o *Mms) GetMessagePartsOk() (*int32, bool)`

GetMessagePartsOk returns a tuple with the MessageParts field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetMessageParts

`func (o *Mms) SetMessageParts(v int32)`

SetMessageParts sets MessageParts field to given value.

### HasMessageParts

`func (o *Mms) HasMessageParts() bool`

HasMessageParts returns a boolean if a field has been set.

### GetMessagePrice

`func (o *Mms) GetMessagePrice() string`

GetMessagePrice returns the MessagePrice field if non-nil, zero value otherwise.

### GetMessagePriceOk

`func (o *Mms) GetMessagePriceOk() (*string, bool)`

GetMessagePriceOk returns a tuple with the MessagePrice field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetMessagePrice

`func (o *Mms) SetMessagePrice(v string)`

SetMessagePrice sets MessagePrice field to given value.

### HasMessagePrice

`func (o *Mms) HasMessagePrice() bool`

HasMessagePrice returns a boolean if a field has been set.

### GetMediaFileUrl

`func (o *Mms) GetMediaFileUrl() string`

GetMediaFileUrl returns the MediaFileUrl field if non-nil, zero value otherwise.

### GetMediaFileUrlOk

`func (o *Mms) GetMediaFileUrlOk() (*string, bool)`

GetMediaFileUrlOk returns a tuple with the MediaFileUrl field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetMediaFileUrl

`func (o *Mms) SetMediaFileUrl(v string)`

SetMediaFileUrl sets MediaFileUrl field to given value.

### HasMediaFileUrl

`func (o *Mms) HasMediaFileUrl() bool`

HasMediaFileUrl returns a boolean if a field has been set.

### GetStatus

`func (o *Mms) GetStatus() string`

GetStatus returns the Status field if non-nil, zero value otherwise.

### GetStatusOk

`func (o *Mms) GetStatusOk() (*string, bool)`

GetStatusOk returns a tuple with the Status field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetStatus

`func (o *Mms) SetStatus(v string)`

SetStatus sets Status field to given value.

### HasStatus

`func (o *Mms) HasStatus() bool`

HasStatus returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


