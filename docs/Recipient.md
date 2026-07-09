# Recipient

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
**CustomString** | Pointer to **string** | A custom string associated with the message. | [optional] 
**Schedule** | Pointer to **int32** | The schedule timestamp of the message. | [optional] 
**Source** | Pointer to **string** | The source of the message. | [optional] 
**Colour** | Pointer to **int32** | The color setting of the message. | [optional] 
**Duplex** | Pointer to **int32** | Whether the message is set to duplex printing. | [optional] 
**PostPages** | Pointer to **int32** | The number of pages in the postal message. | [optional] 
**PostPrice** | Pointer to **string** | The price of the postal message. | [optional] 
**PriorityPost** | Pointer to **int32** | Whether the postal message is set to priority. | [optional] 
**DateAdded** | Pointer to **int32** | The timestamp when the message was added. | [optional] 
**Status** | Pointer to **string** | The status of the message. | [optional] 
**FileUrl** | Pointer to **string** | The URL of the file associated with the message. | [optional] 
**ReturnAddress** | Pointer to [**PostcardRecipientReturnAddress**](PostcardRecipientReturnAddress.md) |  | [optional] 
**ApiUsername** | Pointer to **string** | The API username associated with the message. | [optional] 

## Methods

### NewRecipient

`func NewRecipient() *Recipient`

NewRecipient instantiates a new Recipient object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewRecipientWithDefaults

`func NewRecipientWithDefaults() *Recipient`

NewRecipientWithDefaults instantiates a new Recipient object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetUserId

`func (o *Recipient) GetUserId() int32`

GetUserId returns the UserId field if non-nil, zero value otherwise.

### GetUserIdOk

`func (o *Recipient) GetUserIdOk() (*int32, bool)`

GetUserIdOk returns a tuple with the UserId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetUserId

`func (o *Recipient) SetUserId(v int32)`

SetUserId sets UserId field to given value.

### HasUserId

`func (o *Recipient) HasUserId() bool`

HasUserId returns a boolean if a field has been set.

### GetSubaccountId

`func (o *Recipient) GetSubaccountId() int32`

GetSubaccountId returns the SubaccountId field if non-nil, zero value otherwise.

### GetSubaccountIdOk

`func (o *Recipient) GetSubaccountIdOk() (*int32, bool)`

GetSubaccountIdOk returns a tuple with the SubaccountId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSubaccountId

`func (o *Recipient) SetSubaccountId(v int32)`

SetSubaccountId sets SubaccountId field to given value.

### HasSubaccountId

`func (o *Recipient) HasSubaccountId() bool`

HasSubaccountId returns a boolean if a field has been set.

### GetMessageId

`func (o *Recipient) GetMessageId() string`

GetMessageId returns the MessageId field if non-nil, zero value otherwise.

### GetMessageIdOk

`func (o *Recipient) GetMessageIdOk() (*string, bool)`

GetMessageIdOk returns a tuple with the MessageId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetMessageId

`func (o *Recipient) SetMessageId(v string)`

SetMessageId sets MessageId field to given value.

### HasMessageId

`func (o *Recipient) HasMessageId() bool`

HasMessageId returns a boolean if a field has been set.

### GetAddressName

`func (o *Recipient) GetAddressName() string`

GetAddressName returns the AddressName field if non-nil, zero value otherwise.

### GetAddressNameOk

`func (o *Recipient) GetAddressNameOk() (*string, bool)`

GetAddressNameOk returns a tuple with the AddressName field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAddressName

`func (o *Recipient) SetAddressName(v string)`

SetAddressName sets AddressName field to given value.

### HasAddressName

`func (o *Recipient) HasAddressName() bool`

HasAddressName returns a boolean if a field has been set.

### GetAddressLine1

`func (o *Recipient) GetAddressLine1() string`

GetAddressLine1 returns the AddressLine1 field if non-nil, zero value otherwise.

### GetAddressLine1Ok

`func (o *Recipient) GetAddressLine1Ok() (*string, bool)`

GetAddressLine1Ok returns a tuple with the AddressLine1 field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAddressLine1

`func (o *Recipient) SetAddressLine1(v string)`

SetAddressLine1 sets AddressLine1 field to given value.

### HasAddressLine1

`func (o *Recipient) HasAddressLine1() bool`

HasAddressLine1 returns a boolean if a field has been set.

### GetAddressLine2

`func (o *Recipient) GetAddressLine2() string`

GetAddressLine2 returns the AddressLine2 field if non-nil, zero value otherwise.

### GetAddressLine2Ok

`func (o *Recipient) GetAddressLine2Ok() (*string, bool)`

GetAddressLine2Ok returns a tuple with the AddressLine2 field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAddressLine2

`func (o *Recipient) SetAddressLine2(v string)`

SetAddressLine2 sets AddressLine2 field to given value.

### HasAddressLine2

`func (o *Recipient) HasAddressLine2() bool`

HasAddressLine2 returns a boolean if a field has been set.

### GetAddressCity

`func (o *Recipient) GetAddressCity() string`

GetAddressCity returns the AddressCity field if non-nil, zero value otherwise.

### GetAddressCityOk

`func (o *Recipient) GetAddressCityOk() (*string, bool)`

GetAddressCityOk returns a tuple with the AddressCity field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAddressCity

`func (o *Recipient) SetAddressCity(v string)`

SetAddressCity sets AddressCity field to given value.

### HasAddressCity

`func (o *Recipient) HasAddressCity() bool`

HasAddressCity returns a boolean if a field has been set.

### GetAddressState

`func (o *Recipient) GetAddressState() string`

GetAddressState returns the AddressState field if non-nil, zero value otherwise.

### GetAddressStateOk

`func (o *Recipient) GetAddressStateOk() (*string, bool)`

GetAddressStateOk returns a tuple with the AddressState field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAddressState

`func (o *Recipient) SetAddressState(v string)`

SetAddressState sets AddressState field to given value.

### HasAddressState

`func (o *Recipient) HasAddressState() bool`

HasAddressState returns a boolean if a field has been set.

### GetAddressPostalCode

`func (o *Recipient) GetAddressPostalCode() string`

GetAddressPostalCode returns the AddressPostalCode field if non-nil, zero value otherwise.

### GetAddressPostalCodeOk

`func (o *Recipient) GetAddressPostalCodeOk() (*string, bool)`

GetAddressPostalCodeOk returns a tuple with the AddressPostalCode field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAddressPostalCode

`func (o *Recipient) SetAddressPostalCode(v string)`

SetAddressPostalCode sets AddressPostalCode field to given value.

### HasAddressPostalCode

`func (o *Recipient) HasAddressPostalCode() bool`

HasAddressPostalCode returns a boolean if a field has been set.

### GetAddressCountry

`func (o *Recipient) GetAddressCountry() string`

GetAddressCountry returns the AddressCountry field if non-nil, zero value otherwise.

### GetAddressCountryOk

`func (o *Recipient) GetAddressCountryOk() (*string, bool)`

GetAddressCountryOk returns a tuple with the AddressCountry field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAddressCountry

`func (o *Recipient) SetAddressCountry(v string)`

SetAddressCountry sets AddressCountry field to given value.

### HasAddressCountry

`func (o *Recipient) HasAddressCountry() bool`

HasAddressCountry returns a boolean if a field has been set.

### GetReturnAddressId

`func (o *Recipient) GetReturnAddressId() int32`

GetReturnAddressId returns the ReturnAddressId field if non-nil, zero value otherwise.

### GetReturnAddressIdOk

`func (o *Recipient) GetReturnAddressIdOk() (*int32, bool)`

GetReturnAddressIdOk returns a tuple with the ReturnAddressId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetReturnAddressId

`func (o *Recipient) SetReturnAddressId(v int32)`

SetReturnAddressId sets ReturnAddressId field to given value.

### HasReturnAddressId

`func (o *Recipient) HasReturnAddressId() bool`

HasReturnAddressId returns a boolean if a field has been set.

### GetCustomString

`func (o *Recipient) GetCustomString() string`

GetCustomString returns the CustomString field if non-nil, zero value otherwise.

### GetCustomStringOk

`func (o *Recipient) GetCustomStringOk() (*string, bool)`

GetCustomStringOk returns a tuple with the CustomString field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCustomString

`func (o *Recipient) SetCustomString(v string)`

SetCustomString sets CustomString field to given value.

### HasCustomString

`func (o *Recipient) HasCustomString() bool`

HasCustomString returns a boolean if a field has been set.

### GetSchedule

`func (o *Recipient) GetSchedule() int32`

GetSchedule returns the Schedule field if non-nil, zero value otherwise.

### GetScheduleOk

`func (o *Recipient) GetScheduleOk() (*int32, bool)`

GetScheduleOk returns a tuple with the Schedule field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSchedule

`func (o *Recipient) SetSchedule(v int32)`

SetSchedule sets Schedule field to given value.

### HasSchedule

`func (o *Recipient) HasSchedule() bool`

HasSchedule returns a boolean if a field has been set.

### GetSource

`func (o *Recipient) GetSource() string`

GetSource returns the Source field if non-nil, zero value otherwise.

### GetSourceOk

`func (o *Recipient) GetSourceOk() (*string, bool)`

GetSourceOk returns a tuple with the Source field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSource

`func (o *Recipient) SetSource(v string)`

SetSource sets Source field to given value.

### HasSource

`func (o *Recipient) HasSource() bool`

HasSource returns a boolean if a field has been set.

### GetColour

`func (o *Recipient) GetColour() int32`

GetColour returns the Colour field if non-nil, zero value otherwise.

### GetColourOk

`func (o *Recipient) GetColourOk() (*int32, bool)`

GetColourOk returns a tuple with the Colour field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetColour

`func (o *Recipient) SetColour(v int32)`

SetColour sets Colour field to given value.

### HasColour

`func (o *Recipient) HasColour() bool`

HasColour returns a boolean if a field has been set.

### GetDuplex

`func (o *Recipient) GetDuplex() int32`

GetDuplex returns the Duplex field if non-nil, zero value otherwise.

### GetDuplexOk

`func (o *Recipient) GetDuplexOk() (*int32, bool)`

GetDuplexOk returns a tuple with the Duplex field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDuplex

`func (o *Recipient) SetDuplex(v int32)`

SetDuplex sets Duplex field to given value.

### HasDuplex

`func (o *Recipient) HasDuplex() bool`

HasDuplex returns a boolean if a field has been set.

### GetPostPages

`func (o *Recipient) GetPostPages() int32`

GetPostPages returns the PostPages field if non-nil, zero value otherwise.

### GetPostPagesOk

`func (o *Recipient) GetPostPagesOk() (*int32, bool)`

GetPostPagesOk returns a tuple with the PostPages field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetPostPages

`func (o *Recipient) SetPostPages(v int32)`

SetPostPages sets PostPages field to given value.

### HasPostPages

`func (o *Recipient) HasPostPages() bool`

HasPostPages returns a boolean if a field has been set.

### GetPostPrice

`func (o *Recipient) GetPostPrice() string`

GetPostPrice returns the PostPrice field if non-nil, zero value otherwise.

### GetPostPriceOk

`func (o *Recipient) GetPostPriceOk() (*string, bool)`

GetPostPriceOk returns a tuple with the PostPrice field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetPostPrice

`func (o *Recipient) SetPostPrice(v string)`

SetPostPrice sets PostPrice field to given value.

### HasPostPrice

`func (o *Recipient) HasPostPrice() bool`

HasPostPrice returns a boolean if a field has been set.

### GetPriorityPost

`func (o *Recipient) GetPriorityPost() int32`

GetPriorityPost returns the PriorityPost field if non-nil, zero value otherwise.

### GetPriorityPostOk

`func (o *Recipient) GetPriorityPostOk() (*int32, bool)`

GetPriorityPostOk returns a tuple with the PriorityPost field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetPriorityPost

`func (o *Recipient) SetPriorityPost(v int32)`

SetPriorityPost sets PriorityPost field to given value.

### HasPriorityPost

`func (o *Recipient) HasPriorityPost() bool`

HasPriorityPost returns a boolean if a field has been set.

### GetDateAdded

`func (o *Recipient) GetDateAdded() int32`

GetDateAdded returns the DateAdded field if non-nil, zero value otherwise.

### GetDateAddedOk

`func (o *Recipient) GetDateAddedOk() (*int32, bool)`

GetDateAddedOk returns a tuple with the DateAdded field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDateAdded

`func (o *Recipient) SetDateAdded(v int32)`

SetDateAdded sets DateAdded field to given value.

### HasDateAdded

`func (o *Recipient) HasDateAdded() bool`

HasDateAdded returns a boolean if a field has been set.

### GetStatus

`func (o *Recipient) GetStatus() string`

GetStatus returns the Status field if non-nil, zero value otherwise.

### GetStatusOk

`func (o *Recipient) GetStatusOk() (*string, bool)`

GetStatusOk returns a tuple with the Status field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetStatus

`func (o *Recipient) SetStatus(v string)`

SetStatus sets Status field to given value.

### HasStatus

`func (o *Recipient) HasStatus() bool`

HasStatus returns a boolean if a field has been set.

### GetFileUrl

`func (o *Recipient) GetFileUrl() string`

GetFileUrl returns the FileUrl field if non-nil, zero value otherwise.

### GetFileUrlOk

`func (o *Recipient) GetFileUrlOk() (*string, bool)`

GetFileUrlOk returns a tuple with the FileUrl field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetFileUrl

`func (o *Recipient) SetFileUrl(v string)`

SetFileUrl sets FileUrl field to given value.

### HasFileUrl

`func (o *Recipient) HasFileUrl() bool`

HasFileUrl returns a boolean if a field has been set.

### GetReturnAddress

`func (o *Recipient) GetReturnAddress() PostcardRecipientReturnAddress`

GetReturnAddress returns the ReturnAddress field if non-nil, zero value otherwise.

### GetReturnAddressOk

`func (o *Recipient) GetReturnAddressOk() (*PostcardRecipientReturnAddress, bool)`

GetReturnAddressOk returns a tuple with the ReturnAddress field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetReturnAddress

`func (o *Recipient) SetReturnAddress(v PostcardRecipientReturnAddress)`

SetReturnAddress sets ReturnAddress field to given value.

### HasReturnAddress

`func (o *Recipient) HasReturnAddress() bool`

HasReturnAddress returns a boolean if a field has been set.

### GetApiUsername

`func (o *Recipient) GetApiUsername() string`

GetApiUsername returns the ApiUsername field if non-nil, zero value otherwise.

### GetApiUsernameOk

`func (o *Recipient) GetApiUsernameOk() (*string, bool)`

GetApiUsernameOk returns a tuple with the ApiUsername field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetApiUsername

`func (o *Recipient) SetApiUsername(v string)`

SetApiUsername sets ApiUsername field to given value.

### HasApiUsername

`func (o *Recipient) HasApiUsername() bool`

HasApiUsername returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


