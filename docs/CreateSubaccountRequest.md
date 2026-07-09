# CreateSubaccountRequest

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**ApiUsername** | Pointer to **string** |  | [optional] 
**Password** | Pointer to **string** |  | [optional] 
**Email** | Pointer to **string** |  | [optional] 
**PhoneNumber** | Pointer to **string** |  | [optional] 
**FirstName** | Pointer to **string** |  | [optional] 
**LastName** | Pointer to **string** |  | [optional] 
**UserId** | Pointer to **int32** |  | [optional] 
**SmsDeidentifyMessage** | Pointer to **int32** |  | [optional] 
**AccessSmpp** | Pointer to **int32** |  | [optional] 
**AccessUsers** | Pointer to **int32** |  | [optional] 
**AccessBilling** | Pointer to **int32** |  | [optional] 
**AccessReporting** | Pointer to **int32** |  | [optional] 
**AccessContacts** | Pointer to **int32** |  | [optional] 
**AccessSettings** | Pointer to **int32** |  | [optional] 
**Notes** | Pointer to **string** |  | [optional] 

## Methods

### NewCreateSubaccountRequest

`func NewCreateSubaccountRequest() *CreateSubaccountRequest`

NewCreateSubaccountRequest instantiates a new CreateSubaccountRequest object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewCreateSubaccountRequestWithDefaults

`func NewCreateSubaccountRequestWithDefaults() *CreateSubaccountRequest`

NewCreateSubaccountRequestWithDefaults instantiates a new CreateSubaccountRequest object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetApiUsername

`func (o *CreateSubaccountRequest) GetApiUsername() string`

GetApiUsername returns the ApiUsername field if non-nil, zero value otherwise.

### GetApiUsernameOk

`func (o *CreateSubaccountRequest) GetApiUsernameOk() (*string, bool)`

GetApiUsernameOk returns a tuple with the ApiUsername field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetApiUsername

`func (o *CreateSubaccountRequest) SetApiUsername(v string)`

SetApiUsername sets ApiUsername field to given value.

### HasApiUsername

`func (o *CreateSubaccountRequest) HasApiUsername() bool`

HasApiUsername returns a boolean if a field has been set.

### GetPassword

`func (o *CreateSubaccountRequest) GetPassword() string`

GetPassword returns the Password field if non-nil, zero value otherwise.

### GetPasswordOk

`func (o *CreateSubaccountRequest) GetPasswordOk() (*string, bool)`

GetPasswordOk returns a tuple with the Password field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetPassword

`func (o *CreateSubaccountRequest) SetPassword(v string)`

SetPassword sets Password field to given value.

### HasPassword

`func (o *CreateSubaccountRequest) HasPassword() bool`

HasPassword returns a boolean if a field has been set.

### GetEmail

`func (o *CreateSubaccountRequest) GetEmail() string`

GetEmail returns the Email field if non-nil, zero value otherwise.

### GetEmailOk

`func (o *CreateSubaccountRequest) GetEmailOk() (*string, bool)`

GetEmailOk returns a tuple with the Email field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetEmail

`func (o *CreateSubaccountRequest) SetEmail(v string)`

SetEmail sets Email field to given value.

### HasEmail

`func (o *CreateSubaccountRequest) HasEmail() bool`

HasEmail returns a boolean if a field has been set.

### GetPhoneNumber

`func (o *CreateSubaccountRequest) GetPhoneNumber() string`

GetPhoneNumber returns the PhoneNumber field if non-nil, zero value otherwise.

### GetPhoneNumberOk

`func (o *CreateSubaccountRequest) GetPhoneNumberOk() (*string, bool)`

GetPhoneNumberOk returns a tuple with the PhoneNumber field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetPhoneNumber

`func (o *CreateSubaccountRequest) SetPhoneNumber(v string)`

SetPhoneNumber sets PhoneNumber field to given value.

### HasPhoneNumber

`func (o *CreateSubaccountRequest) HasPhoneNumber() bool`

HasPhoneNumber returns a boolean if a field has been set.

### GetFirstName

`func (o *CreateSubaccountRequest) GetFirstName() string`

GetFirstName returns the FirstName field if non-nil, zero value otherwise.

### GetFirstNameOk

`func (o *CreateSubaccountRequest) GetFirstNameOk() (*string, bool)`

GetFirstNameOk returns a tuple with the FirstName field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetFirstName

`func (o *CreateSubaccountRequest) SetFirstName(v string)`

SetFirstName sets FirstName field to given value.

### HasFirstName

`func (o *CreateSubaccountRequest) HasFirstName() bool`

HasFirstName returns a boolean if a field has been set.

### GetLastName

`func (o *CreateSubaccountRequest) GetLastName() string`

GetLastName returns the LastName field if non-nil, zero value otherwise.

### GetLastNameOk

`func (o *CreateSubaccountRequest) GetLastNameOk() (*string, bool)`

GetLastNameOk returns a tuple with the LastName field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetLastName

`func (o *CreateSubaccountRequest) SetLastName(v string)`

SetLastName sets LastName field to given value.

### HasLastName

`func (o *CreateSubaccountRequest) HasLastName() bool`

HasLastName returns a boolean if a field has been set.

### GetUserId

`func (o *CreateSubaccountRequest) GetUserId() int32`

GetUserId returns the UserId field if non-nil, zero value otherwise.

### GetUserIdOk

`func (o *CreateSubaccountRequest) GetUserIdOk() (*int32, bool)`

GetUserIdOk returns a tuple with the UserId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetUserId

`func (o *CreateSubaccountRequest) SetUserId(v int32)`

SetUserId sets UserId field to given value.

### HasUserId

`func (o *CreateSubaccountRequest) HasUserId() bool`

HasUserId returns a boolean if a field has been set.

### GetSmsDeidentifyMessage

`func (o *CreateSubaccountRequest) GetSmsDeidentifyMessage() int32`

GetSmsDeidentifyMessage returns the SmsDeidentifyMessage field if non-nil, zero value otherwise.

### GetSmsDeidentifyMessageOk

`func (o *CreateSubaccountRequest) GetSmsDeidentifyMessageOk() (*int32, bool)`

GetSmsDeidentifyMessageOk returns a tuple with the SmsDeidentifyMessage field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSmsDeidentifyMessage

`func (o *CreateSubaccountRequest) SetSmsDeidentifyMessage(v int32)`

SetSmsDeidentifyMessage sets SmsDeidentifyMessage field to given value.

### HasSmsDeidentifyMessage

`func (o *CreateSubaccountRequest) HasSmsDeidentifyMessage() bool`

HasSmsDeidentifyMessage returns a boolean if a field has been set.

### GetAccessSmpp

`func (o *CreateSubaccountRequest) GetAccessSmpp() int32`

GetAccessSmpp returns the AccessSmpp field if non-nil, zero value otherwise.

### GetAccessSmppOk

`func (o *CreateSubaccountRequest) GetAccessSmppOk() (*int32, bool)`

GetAccessSmppOk returns a tuple with the AccessSmpp field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAccessSmpp

`func (o *CreateSubaccountRequest) SetAccessSmpp(v int32)`

SetAccessSmpp sets AccessSmpp field to given value.

### HasAccessSmpp

`func (o *CreateSubaccountRequest) HasAccessSmpp() bool`

HasAccessSmpp returns a boolean if a field has been set.

### GetAccessUsers

`func (o *CreateSubaccountRequest) GetAccessUsers() int32`

GetAccessUsers returns the AccessUsers field if non-nil, zero value otherwise.

### GetAccessUsersOk

`func (o *CreateSubaccountRequest) GetAccessUsersOk() (*int32, bool)`

GetAccessUsersOk returns a tuple with the AccessUsers field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAccessUsers

`func (o *CreateSubaccountRequest) SetAccessUsers(v int32)`

SetAccessUsers sets AccessUsers field to given value.

### HasAccessUsers

`func (o *CreateSubaccountRequest) HasAccessUsers() bool`

HasAccessUsers returns a boolean if a field has been set.

### GetAccessBilling

`func (o *CreateSubaccountRequest) GetAccessBilling() int32`

GetAccessBilling returns the AccessBilling field if non-nil, zero value otherwise.

### GetAccessBillingOk

`func (o *CreateSubaccountRequest) GetAccessBillingOk() (*int32, bool)`

GetAccessBillingOk returns a tuple with the AccessBilling field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAccessBilling

`func (o *CreateSubaccountRequest) SetAccessBilling(v int32)`

SetAccessBilling sets AccessBilling field to given value.

### HasAccessBilling

`func (o *CreateSubaccountRequest) HasAccessBilling() bool`

HasAccessBilling returns a boolean if a field has been set.

### GetAccessReporting

`func (o *CreateSubaccountRequest) GetAccessReporting() int32`

GetAccessReporting returns the AccessReporting field if non-nil, zero value otherwise.

### GetAccessReportingOk

`func (o *CreateSubaccountRequest) GetAccessReportingOk() (*int32, bool)`

GetAccessReportingOk returns a tuple with the AccessReporting field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAccessReporting

`func (o *CreateSubaccountRequest) SetAccessReporting(v int32)`

SetAccessReporting sets AccessReporting field to given value.

### HasAccessReporting

`func (o *CreateSubaccountRequest) HasAccessReporting() bool`

HasAccessReporting returns a boolean if a field has been set.

### GetAccessContacts

`func (o *CreateSubaccountRequest) GetAccessContacts() int32`

GetAccessContacts returns the AccessContacts field if non-nil, zero value otherwise.

### GetAccessContactsOk

`func (o *CreateSubaccountRequest) GetAccessContactsOk() (*int32, bool)`

GetAccessContactsOk returns a tuple with the AccessContacts field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAccessContacts

`func (o *CreateSubaccountRequest) SetAccessContacts(v int32)`

SetAccessContacts sets AccessContacts field to given value.

### HasAccessContacts

`func (o *CreateSubaccountRequest) HasAccessContacts() bool`

HasAccessContacts returns a boolean if a field has been set.

### GetAccessSettings

`func (o *CreateSubaccountRequest) GetAccessSettings() int32`

GetAccessSettings returns the AccessSettings field if non-nil, zero value otherwise.

### GetAccessSettingsOk

`func (o *CreateSubaccountRequest) GetAccessSettingsOk() (*int32, bool)`

GetAccessSettingsOk returns a tuple with the AccessSettings field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAccessSettings

`func (o *CreateSubaccountRequest) SetAccessSettings(v int32)`

SetAccessSettings sets AccessSettings field to given value.

### HasAccessSettings

`func (o *CreateSubaccountRequest) HasAccessSettings() bool`

HasAccessSettings returns a boolean if a field has been set.

### GetNotes

`func (o *CreateSubaccountRequest) GetNotes() string`

GetNotes returns the Notes field if non-nil, zero value otherwise.

### GetNotesOk

`func (o *CreateSubaccountRequest) GetNotesOk() (*string, bool)`

GetNotesOk returns a tuple with the Notes field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetNotes

`func (o *CreateSubaccountRequest) SetNotes(v string)`

SetNotes sets Notes field to given value.

### HasNotes

`func (o *CreateSubaccountRequest) HasNotes() bool`

HasNotes returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


