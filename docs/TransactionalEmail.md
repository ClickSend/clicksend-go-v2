# TransactionalEmail

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**UserId** | Pointer to **int32** | The ID of the user. | [optional] 
**SubaccountId** | Pointer to **int32** | The ID of the subaccount. | [optional] 
**FromEmailAddressId** | Pointer to **int32** | The ID of the from email address. | [optional] 
**FromName** | Pointer to **string** | The name of the sender. | [optional] 
**To** | Pointer to [**[]SendEmailRequestToInner**](SendEmailRequestToInner.md) |  | [optional] 
**Cc** | Pointer to [**[]SendEmailRequestToInner**](SendEmailRequestToInner.md) |  | [optional] 
**Bcc** | Pointer to [**[]SendEmailRequestToInner**](SendEmailRequestToInner.md) |  | [optional] 
**Subject** | Pointer to **string** | The subject of the email. | [optional] 
**Body** | Pointer to **string** | The HTML body of the email. | [optional] 
**BodyPlainText** | Pointer to **string** | The plain text body of the email. | [optional] 
**Schedule** | Pointer to **int32** | The timestamp indicating the scheduled time of the email. | [optional] 
**MessageId** | Pointer to **string** | The ID of the email message. | [optional] 
**Status** | Pointer to **string** | The status of the email. | [optional] 
**StatusText** | Pointer to **string** | The text description of the email status. | [optional] 
**SoftBounceCount** | Pointer to **int32** | The count of soft bounces. | [optional] 
**HardBounceCount** | Pointer to **int32** | The count of hard bounces. | [optional] 
**Price** | Pointer to **string** | The price of the email. | [optional] 
**DateAdded** | Pointer to **int32** | The timestamp indicating when the email was added. | [optional] 
**CustomString** | Pointer to **NullableString** | A custom string. | [optional] 
**Attachments** | Pointer to [**[]Attachment**](Attachment.md) |  | [optional] 
**Currency** | Pointer to [**Currency**](Currency.md) |  | [optional] 

## Methods

### NewTransactionalEmail

`func NewTransactionalEmail() *TransactionalEmail`

NewTransactionalEmail instantiates a new TransactionalEmail object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewTransactionalEmailWithDefaults

`func NewTransactionalEmailWithDefaults() *TransactionalEmail`

NewTransactionalEmailWithDefaults instantiates a new TransactionalEmail object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetUserId

`func (o *TransactionalEmail) GetUserId() int32`

GetUserId returns the UserId field if non-nil, zero value otherwise.

### GetUserIdOk

`func (o *TransactionalEmail) GetUserIdOk() (*int32, bool)`

GetUserIdOk returns a tuple with the UserId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetUserId

`func (o *TransactionalEmail) SetUserId(v int32)`

SetUserId sets UserId field to given value.

### HasUserId

`func (o *TransactionalEmail) HasUserId() bool`

HasUserId returns a boolean if a field has been set.

### GetSubaccountId

`func (o *TransactionalEmail) GetSubaccountId() int32`

GetSubaccountId returns the SubaccountId field if non-nil, zero value otherwise.

### GetSubaccountIdOk

`func (o *TransactionalEmail) GetSubaccountIdOk() (*int32, bool)`

GetSubaccountIdOk returns a tuple with the SubaccountId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSubaccountId

`func (o *TransactionalEmail) SetSubaccountId(v int32)`

SetSubaccountId sets SubaccountId field to given value.

### HasSubaccountId

`func (o *TransactionalEmail) HasSubaccountId() bool`

HasSubaccountId returns a boolean if a field has been set.

### GetFromEmailAddressId

`func (o *TransactionalEmail) GetFromEmailAddressId() int32`

GetFromEmailAddressId returns the FromEmailAddressId field if non-nil, zero value otherwise.

### GetFromEmailAddressIdOk

`func (o *TransactionalEmail) GetFromEmailAddressIdOk() (*int32, bool)`

GetFromEmailAddressIdOk returns a tuple with the FromEmailAddressId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetFromEmailAddressId

`func (o *TransactionalEmail) SetFromEmailAddressId(v int32)`

SetFromEmailAddressId sets FromEmailAddressId field to given value.

### HasFromEmailAddressId

`func (o *TransactionalEmail) HasFromEmailAddressId() bool`

HasFromEmailAddressId returns a boolean if a field has been set.

### GetFromName

`func (o *TransactionalEmail) GetFromName() string`

GetFromName returns the FromName field if non-nil, zero value otherwise.

### GetFromNameOk

`func (o *TransactionalEmail) GetFromNameOk() (*string, bool)`

GetFromNameOk returns a tuple with the FromName field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetFromName

`func (o *TransactionalEmail) SetFromName(v string)`

SetFromName sets FromName field to given value.

### HasFromName

`func (o *TransactionalEmail) HasFromName() bool`

HasFromName returns a boolean if a field has been set.

### GetTo

`func (o *TransactionalEmail) GetTo() []SendEmailRequestToInner`

GetTo returns the To field if non-nil, zero value otherwise.

### GetToOk

`func (o *TransactionalEmail) GetToOk() (*[]SendEmailRequestToInner, bool)`

GetToOk returns a tuple with the To field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTo

`func (o *TransactionalEmail) SetTo(v []SendEmailRequestToInner)`

SetTo sets To field to given value.

### HasTo

`func (o *TransactionalEmail) HasTo() bool`

HasTo returns a boolean if a field has been set.

### GetCc

`func (o *TransactionalEmail) GetCc() []SendEmailRequestToInner`

GetCc returns the Cc field if non-nil, zero value otherwise.

### GetCcOk

`func (o *TransactionalEmail) GetCcOk() (*[]SendEmailRequestToInner, bool)`

GetCcOk returns a tuple with the Cc field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCc

`func (o *TransactionalEmail) SetCc(v []SendEmailRequestToInner)`

SetCc sets Cc field to given value.

### HasCc

`func (o *TransactionalEmail) HasCc() bool`

HasCc returns a boolean if a field has been set.

### GetBcc

`func (o *TransactionalEmail) GetBcc() []SendEmailRequestToInner`

GetBcc returns the Bcc field if non-nil, zero value otherwise.

### GetBccOk

`func (o *TransactionalEmail) GetBccOk() (*[]SendEmailRequestToInner, bool)`

GetBccOk returns a tuple with the Bcc field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetBcc

`func (o *TransactionalEmail) SetBcc(v []SendEmailRequestToInner)`

SetBcc sets Bcc field to given value.

### HasBcc

`func (o *TransactionalEmail) HasBcc() bool`

HasBcc returns a boolean if a field has been set.

### GetSubject

`func (o *TransactionalEmail) GetSubject() string`

GetSubject returns the Subject field if non-nil, zero value otherwise.

### GetSubjectOk

`func (o *TransactionalEmail) GetSubjectOk() (*string, bool)`

GetSubjectOk returns a tuple with the Subject field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSubject

`func (o *TransactionalEmail) SetSubject(v string)`

SetSubject sets Subject field to given value.

### HasSubject

`func (o *TransactionalEmail) HasSubject() bool`

HasSubject returns a boolean if a field has been set.

### GetBody

`func (o *TransactionalEmail) GetBody() string`

GetBody returns the Body field if non-nil, zero value otherwise.

### GetBodyOk

`func (o *TransactionalEmail) GetBodyOk() (*string, bool)`

GetBodyOk returns a tuple with the Body field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetBody

`func (o *TransactionalEmail) SetBody(v string)`

SetBody sets Body field to given value.

### HasBody

`func (o *TransactionalEmail) HasBody() bool`

HasBody returns a boolean if a field has been set.

### GetBodyPlainText

`func (o *TransactionalEmail) GetBodyPlainText() string`

GetBodyPlainText returns the BodyPlainText field if non-nil, zero value otherwise.

### GetBodyPlainTextOk

`func (o *TransactionalEmail) GetBodyPlainTextOk() (*string, bool)`

GetBodyPlainTextOk returns a tuple with the BodyPlainText field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetBodyPlainText

`func (o *TransactionalEmail) SetBodyPlainText(v string)`

SetBodyPlainText sets BodyPlainText field to given value.

### HasBodyPlainText

`func (o *TransactionalEmail) HasBodyPlainText() bool`

HasBodyPlainText returns a boolean if a field has been set.

### GetSchedule

`func (o *TransactionalEmail) GetSchedule() int32`

GetSchedule returns the Schedule field if non-nil, zero value otherwise.

### GetScheduleOk

`func (o *TransactionalEmail) GetScheduleOk() (*int32, bool)`

GetScheduleOk returns a tuple with the Schedule field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSchedule

`func (o *TransactionalEmail) SetSchedule(v int32)`

SetSchedule sets Schedule field to given value.

### HasSchedule

`func (o *TransactionalEmail) HasSchedule() bool`

HasSchedule returns a boolean if a field has been set.

### GetMessageId

`func (o *TransactionalEmail) GetMessageId() string`

GetMessageId returns the MessageId field if non-nil, zero value otherwise.

### GetMessageIdOk

`func (o *TransactionalEmail) GetMessageIdOk() (*string, bool)`

GetMessageIdOk returns a tuple with the MessageId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetMessageId

`func (o *TransactionalEmail) SetMessageId(v string)`

SetMessageId sets MessageId field to given value.

### HasMessageId

`func (o *TransactionalEmail) HasMessageId() bool`

HasMessageId returns a boolean if a field has been set.

### GetStatus

`func (o *TransactionalEmail) GetStatus() string`

GetStatus returns the Status field if non-nil, zero value otherwise.

### GetStatusOk

`func (o *TransactionalEmail) GetStatusOk() (*string, bool)`

GetStatusOk returns a tuple with the Status field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetStatus

`func (o *TransactionalEmail) SetStatus(v string)`

SetStatus sets Status field to given value.

### HasStatus

`func (o *TransactionalEmail) HasStatus() bool`

HasStatus returns a boolean if a field has been set.

### GetStatusText

`func (o *TransactionalEmail) GetStatusText() string`

GetStatusText returns the StatusText field if non-nil, zero value otherwise.

### GetStatusTextOk

`func (o *TransactionalEmail) GetStatusTextOk() (*string, bool)`

GetStatusTextOk returns a tuple with the StatusText field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetStatusText

`func (o *TransactionalEmail) SetStatusText(v string)`

SetStatusText sets StatusText field to given value.

### HasStatusText

`func (o *TransactionalEmail) HasStatusText() bool`

HasStatusText returns a boolean if a field has been set.

### GetSoftBounceCount

`func (o *TransactionalEmail) GetSoftBounceCount() int32`

GetSoftBounceCount returns the SoftBounceCount field if non-nil, zero value otherwise.

### GetSoftBounceCountOk

`func (o *TransactionalEmail) GetSoftBounceCountOk() (*int32, bool)`

GetSoftBounceCountOk returns a tuple with the SoftBounceCount field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSoftBounceCount

`func (o *TransactionalEmail) SetSoftBounceCount(v int32)`

SetSoftBounceCount sets SoftBounceCount field to given value.

### HasSoftBounceCount

`func (o *TransactionalEmail) HasSoftBounceCount() bool`

HasSoftBounceCount returns a boolean if a field has been set.

### GetHardBounceCount

`func (o *TransactionalEmail) GetHardBounceCount() int32`

GetHardBounceCount returns the HardBounceCount field if non-nil, zero value otherwise.

### GetHardBounceCountOk

`func (o *TransactionalEmail) GetHardBounceCountOk() (*int32, bool)`

GetHardBounceCountOk returns a tuple with the HardBounceCount field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetHardBounceCount

`func (o *TransactionalEmail) SetHardBounceCount(v int32)`

SetHardBounceCount sets HardBounceCount field to given value.

### HasHardBounceCount

`func (o *TransactionalEmail) HasHardBounceCount() bool`

HasHardBounceCount returns a boolean if a field has been set.

### GetPrice

`func (o *TransactionalEmail) GetPrice() string`

GetPrice returns the Price field if non-nil, zero value otherwise.

### GetPriceOk

`func (o *TransactionalEmail) GetPriceOk() (*string, bool)`

GetPriceOk returns a tuple with the Price field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetPrice

`func (o *TransactionalEmail) SetPrice(v string)`

SetPrice sets Price field to given value.

### HasPrice

`func (o *TransactionalEmail) HasPrice() bool`

HasPrice returns a boolean if a field has been set.

### GetDateAdded

`func (o *TransactionalEmail) GetDateAdded() int32`

GetDateAdded returns the DateAdded field if non-nil, zero value otherwise.

### GetDateAddedOk

`func (o *TransactionalEmail) GetDateAddedOk() (*int32, bool)`

GetDateAddedOk returns a tuple with the DateAdded field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDateAdded

`func (o *TransactionalEmail) SetDateAdded(v int32)`

SetDateAdded sets DateAdded field to given value.

### HasDateAdded

`func (o *TransactionalEmail) HasDateAdded() bool`

HasDateAdded returns a boolean if a field has been set.

### GetCustomString

`func (o *TransactionalEmail) GetCustomString() string`

GetCustomString returns the CustomString field if non-nil, zero value otherwise.

### GetCustomStringOk

`func (o *TransactionalEmail) GetCustomStringOk() (*string, bool)`

GetCustomStringOk returns a tuple with the CustomString field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCustomString

`func (o *TransactionalEmail) SetCustomString(v string)`

SetCustomString sets CustomString field to given value.

### HasCustomString

`func (o *TransactionalEmail) HasCustomString() bool`

HasCustomString returns a boolean if a field has been set.

### SetCustomStringNil

`func (o *TransactionalEmail) SetCustomStringNil(b bool)`

 SetCustomStringNil sets the value for CustomString to be an explicit nil

### UnsetCustomString
`func (o *TransactionalEmail) UnsetCustomString()`

UnsetCustomString ensures that no value is present for CustomString, not even an explicit nil
### GetAttachments

`func (o *TransactionalEmail) GetAttachments() []Attachment`

GetAttachments returns the Attachments field if non-nil, zero value otherwise.

### GetAttachmentsOk

`func (o *TransactionalEmail) GetAttachmentsOk() (*[]Attachment, bool)`

GetAttachmentsOk returns a tuple with the Attachments field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAttachments

`func (o *TransactionalEmail) SetAttachments(v []Attachment)`

SetAttachments sets Attachments field to given value.

### HasAttachments

`func (o *TransactionalEmail) HasAttachments() bool`

HasAttachments returns a boolean if a field has been set.

### GetCurrency

`func (o *TransactionalEmail) GetCurrency() Currency`

GetCurrency returns the Currency field if non-nil, zero value otherwise.

### GetCurrencyOk

`func (o *TransactionalEmail) GetCurrencyOk() (*Currency, bool)`

GetCurrencyOk returns a tuple with the Currency field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCurrency

`func (o *TransactionalEmail) SetCurrency(v Currency)`

SetCurrency sets Currency field to given value.

### HasCurrency

`func (o *TransactionalEmail) HasCurrency() bool`

HasCurrency returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


