# PostcardRecipient

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**UserId** | Pointer to **int32** | The ID of the user. | [optional] 
**SubaccountId** | Pointer to **int32** | The ID of the subaccount. | [optional] 
**MessageId** | Pointer to **string** | The ID of the message. | [optional] 
**AddressName** | Pointer to **string** | The name associated with the address. | [optional] 
**AddressLine1** | Pointer to **string** | The first line of the address. | [optional] 
**AddressLine2** | Pointer to **string** | The second line of the address. | [optional] 
**AddressCity** | Pointer to **string** | The city of the address. | [optional] 
**AddressState** | Pointer to **string** | The state of the address. | [optional] 
**AddressPostalCode** | Pointer to **string** | The postal code of the address. | [optional] 
**AddressCountry** | Pointer to **string** | The country code of the address. | [optional] 
**ReturnAddressId** | Pointer to **int32** | The ID of the return address. | [optional] 
**LetterFileName** | Pointer to **string** | The filename of the letter file. | [optional] 
**Schedule** | Pointer to **int32** | The schedule timestamp of the message. | [optional] 
**IpAddress** | Pointer to **string** | The IP address associated with the message. | [optional] 
**Source** | Pointer to **string** | The source of the message. | [optional] 
**PostPrice** | Pointer to **int32** | The price of posting the message. | [optional] 
**Priority** | Pointer to **int32** | The priority of the message. | [optional] 
**Status** | Pointer to **string** | The status of the message. | [optional] 
**DateAdded** | Pointer to **int32** | The timestamp when the message was added. | [optional] 
**FileUrl** | Pointer to **string** | The URL of the file associated with the message. | [optional] 
**ReturnAddress** | Pointer to [**PostcardRecipientReturnAddress**](PostcardRecipientReturnAddress.md) |  | [optional] 
**ApiUsername** | Pointer to **string** | The API username associated with the message. | [optional] 

## Methods

### NewPostcardRecipient

`func NewPostcardRecipient() *PostcardRecipient`

NewPostcardRecipient instantiates a new PostcardRecipient object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewPostcardRecipientWithDefaults

`func NewPostcardRecipientWithDefaults() *PostcardRecipient`

NewPostcardRecipientWithDefaults instantiates a new PostcardRecipient object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetUserId

`func (o *PostcardRecipient) GetUserId() int32`

GetUserId returns the UserId field if non-nil, zero value otherwise.

### GetUserIdOk

`func (o *PostcardRecipient) GetUserIdOk() (*int32, bool)`

GetUserIdOk returns a tuple with the UserId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetUserId

`func (o *PostcardRecipient) SetUserId(v int32)`

SetUserId sets UserId field to given value.

### HasUserId

`func (o *PostcardRecipient) HasUserId() bool`

HasUserId returns a boolean if a field has been set.

### GetSubaccountId

`func (o *PostcardRecipient) GetSubaccountId() int32`

GetSubaccountId returns the SubaccountId field if non-nil, zero value otherwise.

### GetSubaccountIdOk

`func (o *PostcardRecipient) GetSubaccountIdOk() (*int32, bool)`

GetSubaccountIdOk returns a tuple with the SubaccountId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSubaccountId

`func (o *PostcardRecipient) SetSubaccountId(v int32)`

SetSubaccountId sets SubaccountId field to given value.

### HasSubaccountId

`func (o *PostcardRecipient) HasSubaccountId() bool`

HasSubaccountId returns a boolean if a field has been set.

### GetMessageId

`func (o *PostcardRecipient) GetMessageId() string`

GetMessageId returns the MessageId field if non-nil, zero value otherwise.

### GetMessageIdOk

`func (o *PostcardRecipient) GetMessageIdOk() (*string, bool)`

GetMessageIdOk returns a tuple with the MessageId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetMessageId

`func (o *PostcardRecipient) SetMessageId(v string)`

SetMessageId sets MessageId field to given value.

### HasMessageId

`func (o *PostcardRecipient) HasMessageId() bool`

HasMessageId returns a boolean if a field has been set.

### GetAddressName

`func (o *PostcardRecipient) GetAddressName() string`

GetAddressName returns the AddressName field if non-nil, zero value otherwise.

### GetAddressNameOk

`func (o *PostcardRecipient) GetAddressNameOk() (*string, bool)`

GetAddressNameOk returns a tuple with the AddressName field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAddressName

`func (o *PostcardRecipient) SetAddressName(v string)`

SetAddressName sets AddressName field to given value.

### HasAddressName

`func (o *PostcardRecipient) HasAddressName() bool`

HasAddressName returns a boolean if a field has been set.

### GetAddressLine1

`func (o *PostcardRecipient) GetAddressLine1() string`

GetAddressLine1 returns the AddressLine1 field if non-nil, zero value otherwise.

### GetAddressLine1Ok

`func (o *PostcardRecipient) GetAddressLine1Ok() (*string, bool)`

GetAddressLine1Ok returns a tuple with the AddressLine1 field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAddressLine1

`func (o *PostcardRecipient) SetAddressLine1(v string)`

SetAddressLine1 sets AddressLine1 field to given value.

### HasAddressLine1

`func (o *PostcardRecipient) HasAddressLine1() bool`

HasAddressLine1 returns a boolean if a field has been set.

### GetAddressLine2

`func (o *PostcardRecipient) GetAddressLine2() string`

GetAddressLine2 returns the AddressLine2 field if non-nil, zero value otherwise.

### GetAddressLine2Ok

`func (o *PostcardRecipient) GetAddressLine2Ok() (*string, bool)`

GetAddressLine2Ok returns a tuple with the AddressLine2 field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAddressLine2

`func (o *PostcardRecipient) SetAddressLine2(v string)`

SetAddressLine2 sets AddressLine2 field to given value.

### HasAddressLine2

`func (o *PostcardRecipient) HasAddressLine2() bool`

HasAddressLine2 returns a boolean if a field has been set.

### GetAddressCity

`func (o *PostcardRecipient) GetAddressCity() string`

GetAddressCity returns the AddressCity field if non-nil, zero value otherwise.

### GetAddressCityOk

`func (o *PostcardRecipient) GetAddressCityOk() (*string, bool)`

GetAddressCityOk returns a tuple with the AddressCity field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAddressCity

`func (o *PostcardRecipient) SetAddressCity(v string)`

SetAddressCity sets AddressCity field to given value.

### HasAddressCity

`func (o *PostcardRecipient) HasAddressCity() bool`

HasAddressCity returns a boolean if a field has been set.

### GetAddressState

`func (o *PostcardRecipient) GetAddressState() string`

GetAddressState returns the AddressState field if non-nil, zero value otherwise.

### GetAddressStateOk

`func (o *PostcardRecipient) GetAddressStateOk() (*string, bool)`

GetAddressStateOk returns a tuple with the AddressState field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAddressState

`func (o *PostcardRecipient) SetAddressState(v string)`

SetAddressState sets AddressState field to given value.

### HasAddressState

`func (o *PostcardRecipient) HasAddressState() bool`

HasAddressState returns a boolean if a field has been set.

### GetAddressPostalCode

`func (o *PostcardRecipient) GetAddressPostalCode() string`

GetAddressPostalCode returns the AddressPostalCode field if non-nil, zero value otherwise.

### GetAddressPostalCodeOk

`func (o *PostcardRecipient) GetAddressPostalCodeOk() (*string, bool)`

GetAddressPostalCodeOk returns a tuple with the AddressPostalCode field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAddressPostalCode

`func (o *PostcardRecipient) SetAddressPostalCode(v string)`

SetAddressPostalCode sets AddressPostalCode field to given value.

### HasAddressPostalCode

`func (o *PostcardRecipient) HasAddressPostalCode() bool`

HasAddressPostalCode returns a boolean if a field has been set.

### GetAddressCountry

`func (o *PostcardRecipient) GetAddressCountry() string`

GetAddressCountry returns the AddressCountry field if non-nil, zero value otherwise.

### GetAddressCountryOk

`func (o *PostcardRecipient) GetAddressCountryOk() (*string, bool)`

GetAddressCountryOk returns a tuple with the AddressCountry field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAddressCountry

`func (o *PostcardRecipient) SetAddressCountry(v string)`

SetAddressCountry sets AddressCountry field to given value.

### HasAddressCountry

`func (o *PostcardRecipient) HasAddressCountry() bool`

HasAddressCountry returns a boolean if a field has been set.

### GetReturnAddressId

`func (o *PostcardRecipient) GetReturnAddressId() int32`

GetReturnAddressId returns the ReturnAddressId field if non-nil, zero value otherwise.

### GetReturnAddressIdOk

`func (o *PostcardRecipient) GetReturnAddressIdOk() (*int32, bool)`

GetReturnAddressIdOk returns a tuple with the ReturnAddressId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetReturnAddressId

`func (o *PostcardRecipient) SetReturnAddressId(v int32)`

SetReturnAddressId sets ReturnAddressId field to given value.

### HasReturnAddressId

`func (o *PostcardRecipient) HasReturnAddressId() bool`

HasReturnAddressId returns a boolean if a field has been set.

### GetLetterFileName

`func (o *PostcardRecipient) GetLetterFileName() string`

GetLetterFileName returns the LetterFileName field if non-nil, zero value otherwise.

### GetLetterFileNameOk

`func (o *PostcardRecipient) GetLetterFileNameOk() (*string, bool)`

GetLetterFileNameOk returns a tuple with the LetterFileName field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetLetterFileName

`func (o *PostcardRecipient) SetLetterFileName(v string)`

SetLetterFileName sets LetterFileName field to given value.

### HasLetterFileName

`func (o *PostcardRecipient) HasLetterFileName() bool`

HasLetterFileName returns a boolean if a field has been set.

### GetSchedule

`func (o *PostcardRecipient) GetSchedule() int32`

GetSchedule returns the Schedule field if non-nil, zero value otherwise.

### GetScheduleOk

`func (o *PostcardRecipient) GetScheduleOk() (*int32, bool)`

GetScheduleOk returns a tuple with the Schedule field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSchedule

`func (o *PostcardRecipient) SetSchedule(v int32)`

SetSchedule sets Schedule field to given value.

### HasSchedule

`func (o *PostcardRecipient) HasSchedule() bool`

HasSchedule returns a boolean if a field has been set.

### GetIpAddress

`func (o *PostcardRecipient) GetIpAddress() string`

GetIpAddress returns the IpAddress field if non-nil, zero value otherwise.

### GetIpAddressOk

`func (o *PostcardRecipient) GetIpAddressOk() (*string, bool)`

GetIpAddressOk returns a tuple with the IpAddress field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetIpAddress

`func (o *PostcardRecipient) SetIpAddress(v string)`

SetIpAddress sets IpAddress field to given value.

### HasIpAddress

`func (o *PostcardRecipient) HasIpAddress() bool`

HasIpAddress returns a boolean if a field has been set.

### GetSource

`func (o *PostcardRecipient) GetSource() string`

GetSource returns the Source field if non-nil, zero value otherwise.

### GetSourceOk

`func (o *PostcardRecipient) GetSourceOk() (*string, bool)`

GetSourceOk returns a tuple with the Source field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSource

`func (o *PostcardRecipient) SetSource(v string)`

SetSource sets Source field to given value.

### HasSource

`func (o *PostcardRecipient) HasSource() bool`

HasSource returns a boolean if a field has been set.

### GetPostPrice

`func (o *PostcardRecipient) GetPostPrice() int32`

GetPostPrice returns the PostPrice field if non-nil, zero value otherwise.

### GetPostPriceOk

`func (o *PostcardRecipient) GetPostPriceOk() (*int32, bool)`

GetPostPriceOk returns a tuple with the PostPrice field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetPostPrice

`func (o *PostcardRecipient) SetPostPrice(v int32)`

SetPostPrice sets PostPrice field to given value.

### HasPostPrice

`func (o *PostcardRecipient) HasPostPrice() bool`

HasPostPrice returns a boolean if a field has been set.

### GetPriority

`func (o *PostcardRecipient) GetPriority() int32`

GetPriority returns the Priority field if non-nil, zero value otherwise.

### GetPriorityOk

`func (o *PostcardRecipient) GetPriorityOk() (*int32, bool)`

GetPriorityOk returns a tuple with the Priority field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetPriority

`func (o *PostcardRecipient) SetPriority(v int32)`

SetPriority sets Priority field to given value.

### HasPriority

`func (o *PostcardRecipient) HasPriority() bool`

HasPriority returns a boolean if a field has been set.

### GetStatus

`func (o *PostcardRecipient) GetStatus() string`

GetStatus returns the Status field if non-nil, zero value otherwise.

### GetStatusOk

`func (o *PostcardRecipient) GetStatusOk() (*string, bool)`

GetStatusOk returns a tuple with the Status field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetStatus

`func (o *PostcardRecipient) SetStatus(v string)`

SetStatus sets Status field to given value.

### HasStatus

`func (o *PostcardRecipient) HasStatus() bool`

HasStatus returns a boolean if a field has been set.

### GetDateAdded

`func (o *PostcardRecipient) GetDateAdded() int32`

GetDateAdded returns the DateAdded field if non-nil, zero value otherwise.

### GetDateAddedOk

`func (o *PostcardRecipient) GetDateAddedOk() (*int32, bool)`

GetDateAddedOk returns a tuple with the DateAdded field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDateAdded

`func (o *PostcardRecipient) SetDateAdded(v int32)`

SetDateAdded sets DateAdded field to given value.

### HasDateAdded

`func (o *PostcardRecipient) HasDateAdded() bool`

HasDateAdded returns a boolean if a field has been set.

### GetFileUrl

`func (o *PostcardRecipient) GetFileUrl() string`

GetFileUrl returns the FileUrl field if non-nil, zero value otherwise.

### GetFileUrlOk

`func (o *PostcardRecipient) GetFileUrlOk() (*string, bool)`

GetFileUrlOk returns a tuple with the FileUrl field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetFileUrl

`func (o *PostcardRecipient) SetFileUrl(v string)`

SetFileUrl sets FileUrl field to given value.

### HasFileUrl

`func (o *PostcardRecipient) HasFileUrl() bool`

HasFileUrl returns a boolean if a field has been set.

### GetReturnAddress

`func (o *PostcardRecipient) GetReturnAddress() PostcardRecipientReturnAddress`

GetReturnAddress returns the ReturnAddress field if non-nil, zero value otherwise.

### GetReturnAddressOk

`func (o *PostcardRecipient) GetReturnAddressOk() (*PostcardRecipientReturnAddress, bool)`

GetReturnAddressOk returns a tuple with the ReturnAddress field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetReturnAddress

`func (o *PostcardRecipient) SetReturnAddress(v PostcardRecipientReturnAddress)`

SetReturnAddress sets ReturnAddress field to given value.

### HasReturnAddress

`func (o *PostcardRecipient) HasReturnAddress() bool`

HasReturnAddress returns a boolean if a field has been set.

### GetApiUsername

`func (o *PostcardRecipient) GetApiUsername() string`

GetApiUsername returns the ApiUsername field if non-nil, zero value otherwise.

### GetApiUsernameOk

`func (o *PostcardRecipient) GetApiUsernameOk() (*string, bool)`

GetApiUsernameOk returns a tuple with the ApiUsername field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetApiUsername

`func (o *PostcardRecipient) SetApiUsername(v string)`

SetApiUsername sets ApiUsername field to given value.

### HasApiUsername

`func (o *PostcardRecipient) HasApiUsername() bool`

HasApiUsername returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


