# Fax

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**UserId** | Pointer to **int32** | The ID of the user. | [optional] 
**SubaccountId** | Pointer to **int32** | The ID of the subaccount. | [optional] 
**ListId** | Pointer to **NullableInt32** | The ID of the list. | [optional] 
**MessageId** | Pointer to **string** | The ID of the message. | [optional] 
**To** | Pointer to **string** | The recipient&#39;s phone number. | [optional] 
**From** | Pointer to **string** | The sender&#39;s phone number. | [optional] 
**Carrier** | Pointer to **string** | The carrier associated with the message. | [optional] 
**Country** | Pointer to **string** | The country code. | [optional] 
**CustomString** | Pointer to **string** | A custom string associated with the message. | [optional] 
**Schedule** | Pointer to **string** | The scheduled time for sending the message. | [optional] 
**MessagePages** | Pointer to **int32** | The number of pages in the message. | [optional] 
**MessagePrice** | Pointer to **string** | The price of the message. | [optional] 
**StatusCode** | Pointer to **NullableString** | The status code of the message. | [optional] 
**StatusText** | Pointer to **NullableString** | The status text of the message. | [optional] 
**DateAdded** | Pointer to **int32** | The date when the message was added. | [optional] 
**FromEmail** | Pointer to **string** | The sender&#39;s email address. | [optional] 
**FileUrl** | Pointer to **string** | The URL of the file associated with the message. | [optional] 
**Status** | Pointer to **string** | The status of the message. | [optional] 

## Methods

### NewFax

`func NewFax() *Fax`

NewFax instantiates a new Fax object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewFaxWithDefaults

`func NewFaxWithDefaults() *Fax`

NewFaxWithDefaults instantiates a new Fax object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetUserId

`func (o *Fax) GetUserId() int32`

GetUserId returns the UserId field if non-nil, zero value otherwise.

### GetUserIdOk

`func (o *Fax) GetUserIdOk() (*int32, bool)`

GetUserIdOk returns a tuple with the UserId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetUserId

`func (o *Fax) SetUserId(v int32)`

SetUserId sets UserId field to given value.

### HasUserId

`func (o *Fax) HasUserId() bool`

HasUserId returns a boolean if a field has been set.

### GetSubaccountId

`func (o *Fax) GetSubaccountId() int32`

GetSubaccountId returns the SubaccountId field if non-nil, zero value otherwise.

### GetSubaccountIdOk

`func (o *Fax) GetSubaccountIdOk() (*int32, bool)`

GetSubaccountIdOk returns a tuple with the SubaccountId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSubaccountId

`func (o *Fax) SetSubaccountId(v int32)`

SetSubaccountId sets SubaccountId field to given value.

### HasSubaccountId

`func (o *Fax) HasSubaccountId() bool`

HasSubaccountId returns a boolean if a field has been set.

### GetListId

`func (o *Fax) GetListId() int32`

GetListId returns the ListId field if non-nil, zero value otherwise.

### GetListIdOk

`func (o *Fax) GetListIdOk() (*int32, bool)`

GetListIdOk returns a tuple with the ListId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetListId

`func (o *Fax) SetListId(v int32)`

SetListId sets ListId field to given value.

### HasListId

`func (o *Fax) HasListId() bool`

HasListId returns a boolean if a field has been set.

### SetListIdNil

`func (o *Fax) SetListIdNil(b bool)`

 SetListIdNil sets the value for ListId to be an explicit nil

### UnsetListId
`func (o *Fax) UnsetListId()`

UnsetListId ensures that no value is present for ListId, not even an explicit nil
### GetMessageId

`func (o *Fax) GetMessageId() string`

GetMessageId returns the MessageId field if non-nil, zero value otherwise.

### GetMessageIdOk

`func (o *Fax) GetMessageIdOk() (*string, bool)`

GetMessageIdOk returns a tuple with the MessageId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetMessageId

`func (o *Fax) SetMessageId(v string)`

SetMessageId sets MessageId field to given value.

### HasMessageId

`func (o *Fax) HasMessageId() bool`

HasMessageId returns a boolean if a field has been set.

### GetTo

`func (o *Fax) GetTo() string`

GetTo returns the To field if non-nil, zero value otherwise.

### GetToOk

`func (o *Fax) GetToOk() (*string, bool)`

GetToOk returns a tuple with the To field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTo

`func (o *Fax) SetTo(v string)`

SetTo sets To field to given value.

### HasTo

`func (o *Fax) HasTo() bool`

HasTo returns a boolean if a field has been set.

### GetFrom

`func (o *Fax) GetFrom() string`

GetFrom returns the From field if non-nil, zero value otherwise.

### GetFromOk

`func (o *Fax) GetFromOk() (*string, bool)`

GetFromOk returns a tuple with the From field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetFrom

`func (o *Fax) SetFrom(v string)`

SetFrom sets From field to given value.

### HasFrom

`func (o *Fax) HasFrom() bool`

HasFrom returns a boolean if a field has been set.

### GetCarrier

`func (o *Fax) GetCarrier() string`

GetCarrier returns the Carrier field if non-nil, zero value otherwise.

### GetCarrierOk

`func (o *Fax) GetCarrierOk() (*string, bool)`

GetCarrierOk returns a tuple with the Carrier field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCarrier

`func (o *Fax) SetCarrier(v string)`

SetCarrier sets Carrier field to given value.

### HasCarrier

`func (o *Fax) HasCarrier() bool`

HasCarrier returns a boolean if a field has been set.

### GetCountry

`func (o *Fax) GetCountry() string`

GetCountry returns the Country field if non-nil, zero value otherwise.

### GetCountryOk

`func (o *Fax) GetCountryOk() (*string, bool)`

GetCountryOk returns a tuple with the Country field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCountry

`func (o *Fax) SetCountry(v string)`

SetCountry sets Country field to given value.

### HasCountry

`func (o *Fax) HasCountry() bool`

HasCountry returns a boolean if a field has been set.

### GetCustomString

`func (o *Fax) GetCustomString() string`

GetCustomString returns the CustomString field if non-nil, zero value otherwise.

### GetCustomStringOk

`func (o *Fax) GetCustomStringOk() (*string, bool)`

GetCustomStringOk returns a tuple with the CustomString field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCustomString

`func (o *Fax) SetCustomString(v string)`

SetCustomString sets CustomString field to given value.

### HasCustomString

`func (o *Fax) HasCustomString() bool`

HasCustomString returns a boolean if a field has been set.

### GetSchedule

`func (o *Fax) GetSchedule() string`

GetSchedule returns the Schedule field if non-nil, zero value otherwise.

### GetScheduleOk

`func (o *Fax) GetScheduleOk() (*string, bool)`

GetScheduleOk returns a tuple with the Schedule field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSchedule

`func (o *Fax) SetSchedule(v string)`

SetSchedule sets Schedule field to given value.

### HasSchedule

`func (o *Fax) HasSchedule() bool`

HasSchedule returns a boolean if a field has been set.

### GetMessagePages

`func (o *Fax) GetMessagePages() int32`

GetMessagePages returns the MessagePages field if non-nil, zero value otherwise.

### GetMessagePagesOk

`func (o *Fax) GetMessagePagesOk() (*int32, bool)`

GetMessagePagesOk returns a tuple with the MessagePages field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetMessagePages

`func (o *Fax) SetMessagePages(v int32)`

SetMessagePages sets MessagePages field to given value.

### HasMessagePages

`func (o *Fax) HasMessagePages() bool`

HasMessagePages returns a boolean if a field has been set.

### GetMessagePrice

`func (o *Fax) GetMessagePrice() string`

GetMessagePrice returns the MessagePrice field if non-nil, zero value otherwise.

### GetMessagePriceOk

`func (o *Fax) GetMessagePriceOk() (*string, bool)`

GetMessagePriceOk returns a tuple with the MessagePrice field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetMessagePrice

`func (o *Fax) SetMessagePrice(v string)`

SetMessagePrice sets MessagePrice field to given value.

### HasMessagePrice

`func (o *Fax) HasMessagePrice() bool`

HasMessagePrice returns a boolean if a field has been set.

### GetStatusCode

`func (o *Fax) GetStatusCode() string`

GetStatusCode returns the StatusCode field if non-nil, zero value otherwise.

### GetStatusCodeOk

`func (o *Fax) GetStatusCodeOk() (*string, bool)`

GetStatusCodeOk returns a tuple with the StatusCode field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetStatusCode

`func (o *Fax) SetStatusCode(v string)`

SetStatusCode sets StatusCode field to given value.

### HasStatusCode

`func (o *Fax) HasStatusCode() bool`

HasStatusCode returns a boolean if a field has been set.

### SetStatusCodeNil

`func (o *Fax) SetStatusCodeNil(b bool)`

 SetStatusCodeNil sets the value for StatusCode to be an explicit nil

### UnsetStatusCode
`func (o *Fax) UnsetStatusCode()`

UnsetStatusCode ensures that no value is present for StatusCode, not even an explicit nil
### GetStatusText

`func (o *Fax) GetStatusText() string`

GetStatusText returns the StatusText field if non-nil, zero value otherwise.

### GetStatusTextOk

`func (o *Fax) GetStatusTextOk() (*string, bool)`

GetStatusTextOk returns a tuple with the StatusText field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetStatusText

`func (o *Fax) SetStatusText(v string)`

SetStatusText sets StatusText field to given value.

### HasStatusText

`func (o *Fax) HasStatusText() bool`

HasStatusText returns a boolean if a field has been set.

### SetStatusTextNil

`func (o *Fax) SetStatusTextNil(b bool)`

 SetStatusTextNil sets the value for StatusText to be an explicit nil

### UnsetStatusText
`func (o *Fax) UnsetStatusText()`

UnsetStatusText ensures that no value is present for StatusText, not even an explicit nil
### GetDateAdded

`func (o *Fax) GetDateAdded() int32`

GetDateAdded returns the DateAdded field if non-nil, zero value otherwise.

### GetDateAddedOk

`func (o *Fax) GetDateAddedOk() (*int32, bool)`

GetDateAddedOk returns a tuple with the DateAdded field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDateAdded

`func (o *Fax) SetDateAdded(v int32)`

SetDateAdded sets DateAdded field to given value.

### HasDateAdded

`func (o *Fax) HasDateAdded() bool`

HasDateAdded returns a boolean if a field has been set.

### GetFromEmail

`func (o *Fax) GetFromEmail() string`

GetFromEmail returns the FromEmail field if non-nil, zero value otherwise.

### GetFromEmailOk

`func (o *Fax) GetFromEmailOk() (*string, bool)`

GetFromEmailOk returns a tuple with the FromEmail field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetFromEmail

`func (o *Fax) SetFromEmail(v string)`

SetFromEmail sets FromEmail field to given value.

### HasFromEmail

`func (o *Fax) HasFromEmail() bool`

HasFromEmail returns a boolean if a field has been set.

### GetFileUrl

`func (o *Fax) GetFileUrl() string`

GetFileUrl returns the FileUrl field if non-nil, zero value otherwise.

### GetFileUrlOk

`func (o *Fax) GetFileUrlOk() (*string, bool)`

GetFileUrlOk returns a tuple with the FileUrl field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetFileUrl

`func (o *Fax) SetFileUrl(v string)`

SetFileUrl sets FileUrl field to given value.

### HasFileUrl

`func (o *Fax) HasFileUrl() bool`

HasFileUrl returns a boolean if a field has been set.

### GetStatus

`func (o *Fax) GetStatus() string`

GetStatus returns the Status field if non-nil, zero value otherwise.

### GetStatusOk

`func (o *Fax) GetStatusOk() (*string, bool)`

GetStatusOk returns a tuple with the Status field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetStatus

`func (o *Fax) SetStatus(v string)`

SetStatus sets Status field to given value.

### HasStatus

`func (o *Fax) HasStatus() bool`

HasStatus returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


