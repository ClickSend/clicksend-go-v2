# ViewMmsHistoryDataAllOfDataInner

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Direction** | Pointer to **string** | The direction of the message (in or out). | [optional] 
**Date** | Pointer to **string** | The date of the message. | [optional] 
**To** | Pointer to **string** | The recipient of the message. | [optional] 
**Body** | Pointer to **string** | The body of the message. | [optional] 
**Subject** | Pointer to **NullableString** | The subject of the message. | [optional] 
**Priority** | Pointer to **int32** | The priority of the message. | [optional] 
**MediaFileUrl** | Pointer to **NullableString** | A temporary, signed URL to download the message&#39;s media attachment. | [optional] 
**Status** | Pointer to **string** | The status of the message. | [optional] 
**From** | Pointer to **string** | The sender of the message. | [optional] 
**Schedule** | Pointer to **string** | The schedule time of the message. | [optional] 
**DateAdded** | Pointer to **int32** | The Unix timestamp when the message was added. | [optional] 
**StatusCode** | Pointer to **NullableString** | The status code (if applicable). | [optional] 
**StatusText** | Pointer to **NullableString** | The status text (if applicable). | [optional] 
**ErrorCode** | Pointer to **NullableString** | The error code (if applicable). | [optional] 
**ErrorText** | Pointer to **string** | The error text (if applicable). | [optional] 
**MessageId** | Pointer to **string** | The ID of the message. | [optional] 
**MessageParts** | Pointer to **string** | The number of parts the message was split into. | [optional] 
**MessagePrice** | Pointer to **string** | The price of the message. | [optional] 
**FromEmail** | Pointer to **NullableString** | The email of the sender (if applicable). | [optional] 
**ListId** | Pointer to **NullableString** | The ID of the list (if applicable). | [optional] 
**CustomString** | Pointer to **string** | Custom string associated with the message. | [optional] 
**ContactId** | Pointer to **int32** | The ID of the contact. | [optional] 
**UserId** | Pointer to **int32** | The ID of the user. | [optional] 
**SubaccountId** | Pointer to **int32** | The ID of the subaccount. | [optional] 
**Country** | Pointer to **string** | The country code. | [optional] 
**Carrier** | Pointer to **string** | The carrier information. | [optional] 
**FirstName** | Pointer to **string** | The first name of the sender. | [optional] 
**LastName** | Pointer to **string** | The last name of the sender. | [optional] 
**ApiUsername** | Pointer to **string** | The API username associated with the message. | [optional] 

## Methods

### NewViewMmsHistoryDataAllOfDataInner

`func NewViewMmsHistoryDataAllOfDataInner() *ViewMmsHistoryDataAllOfDataInner`

NewViewMmsHistoryDataAllOfDataInner instantiates a new ViewMmsHistoryDataAllOfDataInner object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewViewMmsHistoryDataAllOfDataInnerWithDefaults

`func NewViewMmsHistoryDataAllOfDataInnerWithDefaults() *ViewMmsHistoryDataAllOfDataInner`

NewViewMmsHistoryDataAllOfDataInnerWithDefaults instantiates a new ViewMmsHistoryDataAllOfDataInner object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetDirection

`func (o *ViewMmsHistoryDataAllOfDataInner) GetDirection() string`

GetDirection returns the Direction field if non-nil, zero value otherwise.

### GetDirectionOk

`func (o *ViewMmsHistoryDataAllOfDataInner) GetDirectionOk() (*string, bool)`

GetDirectionOk returns a tuple with the Direction field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDirection

`func (o *ViewMmsHistoryDataAllOfDataInner) SetDirection(v string)`

SetDirection sets Direction field to given value.

### HasDirection

`func (o *ViewMmsHistoryDataAllOfDataInner) HasDirection() bool`

HasDirection returns a boolean if a field has been set.

### GetDate

`func (o *ViewMmsHistoryDataAllOfDataInner) GetDate() string`

GetDate returns the Date field if non-nil, zero value otherwise.

### GetDateOk

`func (o *ViewMmsHistoryDataAllOfDataInner) GetDateOk() (*string, bool)`

GetDateOk returns a tuple with the Date field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDate

`func (o *ViewMmsHistoryDataAllOfDataInner) SetDate(v string)`

SetDate sets Date field to given value.

### HasDate

`func (o *ViewMmsHistoryDataAllOfDataInner) HasDate() bool`

HasDate returns a boolean if a field has been set.

### GetTo

`func (o *ViewMmsHistoryDataAllOfDataInner) GetTo() string`

GetTo returns the To field if non-nil, zero value otherwise.

### GetToOk

`func (o *ViewMmsHistoryDataAllOfDataInner) GetToOk() (*string, bool)`

GetToOk returns a tuple with the To field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTo

`func (o *ViewMmsHistoryDataAllOfDataInner) SetTo(v string)`

SetTo sets To field to given value.

### HasTo

`func (o *ViewMmsHistoryDataAllOfDataInner) HasTo() bool`

HasTo returns a boolean if a field has been set.

### GetBody

`func (o *ViewMmsHistoryDataAllOfDataInner) GetBody() string`

GetBody returns the Body field if non-nil, zero value otherwise.

### GetBodyOk

`func (o *ViewMmsHistoryDataAllOfDataInner) GetBodyOk() (*string, bool)`

GetBodyOk returns a tuple with the Body field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetBody

`func (o *ViewMmsHistoryDataAllOfDataInner) SetBody(v string)`

SetBody sets Body field to given value.

### HasBody

`func (o *ViewMmsHistoryDataAllOfDataInner) HasBody() bool`

HasBody returns a boolean if a field has been set.

### GetSubject

`func (o *ViewMmsHistoryDataAllOfDataInner) GetSubject() string`

GetSubject returns the Subject field if non-nil, zero value otherwise.

### GetSubjectOk

`func (o *ViewMmsHistoryDataAllOfDataInner) GetSubjectOk() (*string, bool)`

GetSubjectOk returns a tuple with the Subject field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSubject

`func (o *ViewMmsHistoryDataAllOfDataInner) SetSubject(v string)`

SetSubject sets Subject field to given value.

### HasSubject

`func (o *ViewMmsHistoryDataAllOfDataInner) HasSubject() bool`

HasSubject returns a boolean if a field has been set.

### SetSubjectNil

`func (o *ViewMmsHistoryDataAllOfDataInner) SetSubjectNil(b bool)`

 SetSubjectNil sets the value for Subject to be an explicit nil

### UnsetSubject
`func (o *ViewMmsHistoryDataAllOfDataInner) UnsetSubject()`

UnsetSubject ensures that no value is present for Subject, not even an explicit nil
### GetPriority

`func (o *ViewMmsHistoryDataAllOfDataInner) GetPriority() int32`

GetPriority returns the Priority field if non-nil, zero value otherwise.

### GetPriorityOk

`func (o *ViewMmsHistoryDataAllOfDataInner) GetPriorityOk() (*int32, bool)`

GetPriorityOk returns a tuple with the Priority field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetPriority

`func (o *ViewMmsHistoryDataAllOfDataInner) SetPriority(v int32)`

SetPriority sets Priority field to given value.

### HasPriority

`func (o *ViewMmsHistoryDataAllOfDataInner) HasPriority() bool`

HasPriority returns a boolean if a field has been set.

### GetMediaFileUrl

`func (o *ViewMmsHistoryDataAllOfDataInner) GetMediaFileUrl() string`

GetMediaFileUrl returns the MediaFileUrl field if non-nil, zero value otherwise.

### GetMediaFileUrlOk

`func (o *ViewMmsHistoryDataAllOfDataInner) GetMediaFileUrlOk() (*string, bool)`

GetMediaFileUrlOk returns a tuple with the MediaFileUrl field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetMediaFileUrl

`func (o *ViewMmsHistoryDataAllOfDataInner) SetMediaFileUrl(v string)`

SetMediaFileUrl sets MediaFileUrl field to given value.

### HasMediaFileUrl

`func (o *ViewMmsHistoryDataAllOfDataInner) HasMediaFileUrl() bool`

HasMediaFileUrl returns a boolean if a field has been set.

### SetMediaFileUrlNil

`func (o *ViewMmsHistoryDataAllOfDataInner) SetMediaFileUrlNil(b bool)`

 SetMediaFileUrlNil sets the value for MediaFileUrl to be an explicit nil

### UnsetMediaFileUrl
`func (o *ViewMmsHistoryDataAllOfDataInner) UnsetMediaFileUrl()`

UnsetMediaFileUrl ensures that no value is present for MediaFileUrl, not even an explicit nil
### GetStatus

`func (o *ViewMmsHistoryDataAllOfDataInner) GetStatus() string`

GetStatus returns the Status field if non-nil, zero value otherwise.

### GetStatusOk

`func (o *ViewMmsHistoryDataAllOfDataInner) GetStatusOk() (*string, bool)`

GetStatusOk returns a tuple with the Status field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetStatus

`func (o *ViewMmsHistoryDataAllOfDataInner) SetStatus(v string)`

SetStatus sets Status field to given value.

### HasStatus

`func (o *ViewMmsHistoryDataAllOfDataInner) HasStatus() bool`

HasStatus returns a boolean if a field has been set.

### GetFrom

`func (o *ViewMmsHistoryDataAllOfDataInner) GetFrom() string`

GetFrom returns the From field if non-nil, zero value otherwise.

### GetFromOk

`func (o *ViewMmsHistoryDataAllOfDataInner) GetFromOk() (*string, bool)`

GetFromOk returns a tuple with the From field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetFrom

`func (o *ViewMmsHistoryDataAllOfDataInner) SetFrom(v string)`

SetFrom sets From field to given value.

### HasFrom

`func (o *ViewMmsHistoryDataAllOfDataInner) HasFrom() bool`

HasFrom returns a boolean if a field has been set.

### GetSchedule

`func (o *ViewMmsHistoryDataAllOfDataInner) GetSchedule() string`

GetSchedule returns the Schedule field if non-nil, zero value otherwise.

### GetScheduleOk

`func (o *ViewMmsHistoryDataAllOfDataInner) GetScheduleOk() (*string, bool)`

GetScheduleOk returns a tuple with the Schedule field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSchedule

`func (o *ViewMmsHistoryDataAllOfDataInner) SetSchedule(v string)`

SetSchedule sets Schedule field to given value.

### HasSchedule

`func (o *ViewMmsHistoryDataAllOfDataInner) HasSchedule() bool`

HasSchedule returns a boolean if a field has been set.

### GetDateAdded

`func (o *ViewMmsHistoryDataAllOfDataInner) GetDateAdded() int32`

GetDateAdded returns the DateAdded field if non-nil, zero value otherwise.

### GetDateAddedOk

`func (o *ViewMmsHistoryDataAllOfDataInner) GetDateAddedOk() (*int32, bool)`

GetDateAddedOk returns a tuple with the DateAdded field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDateAdded

`func (o *ViewMmsHistoryDataAllOfDataInner) SetDateAdded(v int32)`

SetDateAdded sets DateAdded field to given value.

### HasDateAdded

`func (o *ViewMmsHistoryDataAllOfDataInner) HasDateAdded() bool`

HasDateAdded returns a boolean if a field has been set.

### GetStatusCode

`func (o *ViewMmsHistoryDataAllOfDataInner) GetStatusCode() string`

GetStatusCode returns the StatusCode field if non-nil, zero value otherwise.

### GetStatusCodeOk

`func (o *ViewMmsHistoryDataAllOfDataInner) GetStatusCodeOk() (*string, bool)`

GetStatusCodeOk returns a tuple with the StatusCode field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetStatusCode

`func (o *ViewMmsHistoryDataAllOfDataInner) SetStatusCode(v string)`

SetStatusCode sets StatusCode field to given value.

### HasStatusCode

`func (o *ViewMmsHistoryDataAllOfDataInner) HasStatusCode() bool`

HasStatusCode returns a boolean if a field has been set.

### SetStatusCodeNil

`func (o *ViewMmsHistoryDataAllOfDataInner) SetStatusCodeNil(b bool)`

 SetStatusCodeNil sets the value for StatusCode to be an explicit nil

### UnsetStatusCode
`func (o *ViewMmsHistoryDataAllOfDataInner) UnsetStatusCode()`

UnsetStatusCode ensures that no value is present for StatusCode, not even an explicit nil
### GetStatusText

`func (o *ViewMmsHistoryDataAllOfDataInner) GetStatusText() string`

GetStatusText returns the StatusText field if non-nil, zero value otherwise.

### GetStatusTextOk

`func (o *ViewMmsHistoryDataAllOfDataInner) GetStatusTextOk() (*string, bool)`

GetStatusTextOk returns a tuple with the StatusText field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetStatusText

`func (o *ViewMmsHistoryDataAllOfDataInner) SetStatusText(v string)`

SetStatusText sets StatusText field to given value.

### HasStatusText

`func (o *ViewMmsHistoryDataAllOfDataInner) HasStatusText() bool`

HasStatusText returns a boolean if a field has been set.

### SetStatusTextNil

`func (o *ViewMmsHistoryDataAllOfDataInner) SetStatusTextNil(b bool)`

 SetStatusTextNil sets the value for StatusText to be an explicit nil

### UnsetStatusText
`func (o *ViewMmsHistoryDataAllOfDataInner) UnsetStatusText()`

UnsetStatusText ensures that no value is present for StatusText, not even an explicit nil
### GetErrorCode

`func (o *ViewMmsHistoryDataAllOfDataInner) GetErrorCode() string`

GetErrorCode returns the ErrorCode field if non-nil, zero value otherwise.

### GetErrorCodeOk

`func (o *ViewMmsHistoryDataAllOfDataInner) GetErrorCodeOk() (*string, bool)`

GetErrorCodeOk returns a tuple with the ErrorCode field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetErrorCode

`func (o *ViewMmsHistoryDataAllOfDataInner) SetErrorCode(v string)`

SetErrorCode sets ErrorCode field to given value.

### HasErrorCode

`func (o *ViewMmsHistoryDataAllOfDataInner) HasErrorCode() bool`

HasErrorCode returns a boolean if a field has been set.

### SetErrorCodeNil

`func (o *ViewMmsHistoryDataAllOfDataInner) SetErrorCodeNil(b bool)`

 SetErrorCodeNil sets the value for ErrorCode to be an explicit nil

### UnsetErrorCode
`func (o *ViewMmsHistoryDataAllOfDataInner) UnsetErrorCode()`

UnsetErrorCode ensures that no value is present for ErrorCode, not even an explicit nil
### GetErrorText

`func (o *ViewMmsHistoryDataAllOfDataInner) GetErrorText() string`

GetErrorText returns the ErrorText field if non-nil, zero value otherwise.

### GetErrorTextOk

`func (o *ViewMmsHistoryDataAllOfDataInner) GetErrorTextOk() (*string, bool)`

GetErrorTextOk returns a tuple with the ErrorText field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetErrorText

`func (o *ViewMmsHistoryDataAllOfDataInner) SetErrorText(v string)`

SetErrorText sets ErrorText field to given value.

### HasErrorText

`func (o *ViewMmsHistoryDataAllOfDataInner) HasErrorText() bool`

HasErrorText returns a boolean if a field has been set.

### GetMessageId

`func (o *ViewMmsHistoryDataAllOfDataInner) GetMessageId() string`

GetMessageId returns the MessageId field if non-nil, zero value otherwise.

### GetMessageIdOk

`func (o *ViewMmsHistoryDataAllOfDataInner) GetMessageIdOk() (*string, bool)`

GetMessageIdOk returns a tuple with the MessageId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetMessageId

`func (o *ViewMmsHistoryDataAllOfDataInner) SetMessageId(v string)`

SetMessageId sets MessageId field to given value.

### HasMessageId

`func (o *ViewMmsHistoryDataAllOfDataInner) HasMessageId() bool`

HasMessageId returns a boolean if a field has been set.

### GetMessageParts

`func (o *ViewMmsHistoryDataAllOfDataInner) GetMessageParts() string`

GetMessageParts returns the MessageParts field if non-nil, zero value otherwise.

### GetMessagePartsOk

`func (o *ViewMmsHistoryDataAllOfDataInner) GetMessagePartsOk() (*string, bool)`

GetMessagePartsOk returns a tuple with the MessageParts field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetMessageParts

`func (o *ViewMmsHistoryDataAllOfDataInner) SetMessageParts(v string)`

SetMessageParts sets MessageParts field to given value.

### HasMessageParts

`func (o *ViewMmsHistoryDataAllOfDataInner) HasMessageParts() bool`

HasMessageParts returns a boolean if a field has been set.

### GetMessagePrice

`func (o *ViewMmsHistoryDataAllOfDataInner) GetMessagePrice() string`

GetMessagePrice returns the MessagePrice field if non-nil, zero value otherwise.

### GetMessagePriceOk

`func (o *ViewMmsHistoryDataAllOfDataInner) GetMessagePriceOk() (*string, bool)`

GetMessagePriceOk returns a tuple with the MessagePrice field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetMessagePrice

`func (o *ViewMmsHistoryDataAllOfDataInner) SetMessagePrice(v string)`

SetMessagePrice sets MessagePrice field to given value.

### HasMessagePrice

`func (o *ViewMmsHistoryDataAllOfDataInner) HasMessagePrice() bool`

HasMessagePrice returns a boolean if a field has been set.

### GetFromEmail

`func (o *ViewMmsHistoryDataAllOfDataInner) GetFromEmail() string`

GetFromEmail returns the FromEmail field if non-nil, zero value otherwise.

### GetFromEmailOk

`func (o *ViewMmsHistoryDataAllOfDataInner) GetFromEmailOk() (*string, bool)`

GetFromEmailOk returns a tuple with the FromEmail field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetFromEmail

`func (o *ViewMmsHistoryDataAllOfDataInner) SetFromEmail(v string)`

SetFromEmail sets FromEmail field to given value.

### HasFromEmail

`func (o *ViewMmsHistoryDataAllOfDataInner) HasFromEmail() bool`

HasFromEmail returns a boolean if a field has been set.

### SetFromEmailNil

`func (o *ViewMmsHistoryDataAllOfDataInner) SetFromEmailNil(b bool)`

 SetFromEmailNil sets the value for FromEmail to be an explicit nil

### UnsetFromEmail
`func (o *ViewMmsHistoryDataAllOfDataInner) UnsetFromEmail()`

UnsetFromEmail ensures that no value is present for FromEmail, not even an explicit nil
### GetListId

`func (o *ViewMmsHistoryDataAllOfDataInner) GetListId() string`

GetListId returns the ListId field if non-nil, zero value otherwise.

### GetListIdOk

`func (o *ViewMmsHistoryDataAllOfDataInner) GetListIdOk() (*string, bool)`

GetListIdOk returns a tuple with the ListId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetListId

`func (o *ViewMmsHistoryDataAllOfDataInner) SetListId(v string)`

SetListId sets ListId field to given value.

### HasListId

`func (o *ViewMmsHistoryDataAllOfDataInner) HasListId() bool`

HasListId returns a boolean if a field has been set.

### SetListIdNil

`func (o *ViewMmsHistoryDataAllOfDataInner) SetListIdNil(b bool)`

 SetListIdNil sets the value for ListId to be an explicit nil

### UnsetListId
`func (o *ViewMmsHistoryDataAllOfDataInner) UnsetListId()`

UnsetListId ensures that no value is present for ListId, not even an explicit nil
### GetCustomString

`func (o *ViewMmsHistoryDataAllOfDataInner) GetCustomString() string`

GetCustomString returns the CustomString field if non-nil, zero value otherwise.

### GetCustomStringOk

`func (o *ViewMmsHistoryDataAllOfDataInner) GetCustomStringOk() (*string, bool)`

GetCustomStringOk returns a tuple with the CustomString field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCustomString

`func (o *ViewMmsHistoryDataAllOfDataInner) SetCustomString(v string)`

SetCustomString sets CustomString field to given value.

### HasCustomString

`func (o *ViewMmsHistoryDataAllOfDataInner) HasCustomString() bool`

HasCustomString returns a boolean if a field has been set.

### GetContactId

`func (o *ViewMmsHistoryDataAllOfDataInner) GetContactId() int32`

GetContactId returns the ContactId field if non-nil, zero value otherwise.

### GetContactIdOk

`func (o *ViewMmsHistoryDataAllOfDataInner) GetContactIdOk() (*int32, bool)`

GetContactIdOk returns a tuple with the ContactId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetContactId

`func (o *ViewMmsHistoryDataAllOfDataInner) SetContactId(v int32)`

SetContactId sets ContactId field to given value.

### HasContactId

`func (o *ViewMmsHistoryDataAllOfDataInner) HasContactId() bool`

HasContactId returns a boolean if a field has been set.

### GetUserId

`func (o *ViewMmsHistoryDataAllOfDataInner) GetUserId() int32`

GetUserId returns the UserId field if non-nil, zero value otherwise.

### GetUserIdOk

`func (o *ViewMmsHistoryDataAllOfDataInner) GetUserIdOk() (*int32, bool)`

GetUserIdOk returns a tuple with the UserId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetUserId

`func (o *ViewMmsHistoryDataAllOfDataInner) SetUserId(v int32)`

SetUserId sets UserId field to given value.

### HasUserId

`func (o *ViewMmsHistoryDataAllOfDataInner) HasUserId() bool`

HasUserId returns a boolean if a field has been set.

### GetSubaccountId

`func (o *ViewMmsHistoryDataAllOfDataInner) GetSubaccountId() int32`

GetSubaccountId returns the SubaccountId field if non-nil, zero value otherwise.

### GetSubaccountIdOk

`func (o *ViewMmsHistoryDataAllOfDataInner) GetSubaccountIdOk() (*int32, bool)`

GetSubaccountIdOk returns a tuple with the SubaccountId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSubaccountId

`func (o *ViewMmsHistoryDataAllOfDataInner) SetSubaccountId(v int32)`

SetSubaccountId sets SubaccountId field to given value.

### HasSubaccountId

`func (o *ViewMmsHistoryDataAllOfDataInner) HasSubaccountId() bool`

HasSubaccountId returns a boolean if a field has been set.

### GetCountry

`func (o *ViewMmsHistoryDataAllOfDataInner) GetCountry() string`

GetCountry returns the Country field if non-nil, zero value otherwise.

### GetCountryOk

`func (o *ViewMmsHistoryDataAllOfDataInner) GetCountryOk() (*string, bool)`

GetCountryOk returns a tuple with the Country field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCountry

`func (o *ViewMmsHistoryDataAllOfDataInner) SetCountry(v string)`

SetCountry sets Country field to given value.

### HasCountry

`func (o *ViewMmsHistoryDataAllOfDataInner) HasCountry() bool`

HasCountry returns a boolean if a field has been set.

### GetCarrier

`func (o *ViewMmsHistoryDataAllOfDataInner) GetCarrier() string`

GetCarrier returns the Carrier field if non-nil, zero value otherwise.

### GetCarrierOk

`func (o *ViewMmsHistoryDataAllOfDataInner) GetCarrierOk() (*string, bool)`

GetCarrierOk returns a tuple with the Carrier field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCarrier

`func (o *ViewMmsHistoryDataAllOfDataInner) SetCarrier(v string)`

SetCarrier sets Carrier field to given value.

### HasCarrier

`func (o *ViewMmsHistoryDataAllOfDataInner) HasCarrier() bool`

HasCarrier returns a boolean if a field has been set.

### GetFirstName

`func (o *ViewMmsHistoryDataAllOfDataInner) GetFirstName() string`

GetFirstName returns the FirstName field if non-nil, zero value otherwise.

### GetFirstNameOk

`func (o *ViewMmsHistoryDataAllOfDataInner) GetFirstNameOk() (*string, bool)`

GetFirstNameOk returns a tuple with the FirstName field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetFirstName

`func (o *ViewMmsHistoryDataAllOfDataInner) SetFirstName(v string)`

SetFirstName sets FirstName field to given value.

### HasFirstName

`func (o *ViewMmsHistoryDataAllOfDataInner) HasFirstName() bool`

HasFirstName returns a boolean if a field has been set.

### GetLastName

`func (o *ViewMmsHistoryDataAllOfDataInner) GetLastName() string`

GetLastName returns the LastName field if non-nil, zero value otherwise.

### GetLastNameOk

`func (o *ViewMmsHistoryDataAllOfDataInner) GetLastNameOk() (*string, bool)`

GetLastNameOk returns a tuple with the LastName field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetLastName

`func (o *ViewMmsHistoryDataAllOfDataInner) SetLastName(v string)`

SetLastName sets LastName field to given value.

### HasLastName

`func (o *ViewMmsHistoryDataAllOfDataInner) HasLastName() bool`

HasLastName returns a boolean if a field has been set.

### GetApiUsername

`func (o *ViewMmsHistoryDataAllOfDataInner) GetApiUsername() string`

GetApiUsername returns the ApiUsername field if non-nil, zero value otherwise.

### GetApiUsernameOk

`func (o *ViewMmsHistoryDataAllOfDataInner) GetApiUsernameOk() (*string, bool)`

GetApiUsernameOk returns a tuple with the ApiUsername field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetApiUsername

`func (o *ViewMmsHistoryDataAllOfDataInner) SetApiUsername(v string)`

SetApiUsername sets ApiUsername field to given value.

### HasApiUsername

`func (o *ViewMmsHistoryDataAllOfDataInner) HasApiUsername() bool`

HasApiUsername returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


