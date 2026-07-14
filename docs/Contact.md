# Contact

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**ContactId** | Pointer to **int32** | The unique identifier for the contact. | [optional] 
**ListId** | Pointer to **int32** | The identifier of the list the contact belongs to. | [optional] 
**PhoneNumber** | Pointer to **string** | The phone number of the contact. | [optional] 
**FirstName** | Pointer to **string** | The first name of the contact. | [optional] 
**LastName** | Pointer to **string** | The last name of the contact. | [optional] 
**Custom1** | Pointer to **string** | Custom field 1. | [optional] 
**Custom2** | Pointer to **string** | Custom field 2. | [optional] 
**Custom3** | Pointer to **string** | Custom field 3. | [optional] 
**Custom4** | Pointer to **string** | Custom field 4. | [optional] 
**DateAdded** | Pointer to **string** | The date when the contact was added. Returned as a plain string rather than a strict date-time since the API sometimes returns a raw Unix timestamp (e.g. \&quot;1783997542\&quot;) instead of ISO 8601. | [optional] 
**DateUpdated** | Pointer to **string** | The date when the contact was last updated. Returned as a plain string rather than a strict date-time since the API sometimes returns a raw Unix timestamp (e.g. \&quot;1783997542\&quot;) instead of ISO 8601. | [optional] 
**FaxNumber** | Pointer to **NullableString** | The fax number of the contact. | [optional] 
**OrganizationName** | Pointer to **NullableString** | The organization name of the contact. | [optional] 
**Email** | Pointer to **NullableString** | The email address of the contact. | [optional] 
**AddressLine1** | Pointer to **NullableString** | The address line 1 of the contact. | [optional] 
**AddressLine2** | Pointer to **NullableString** | The address line 2 of the contact. | [optional] 
**AddressCity** | Pointer to **NullableString** | The address city of the contact. | [optional] 
**AddressState** | Pointer to **NullableString** | The address state of the contact. | [optional] 
**AddressPostalCode** | Pointer to **NullableString** | The address postal code of the contact. | [optional] 
**AddressCountry** | Pointer to **NullableString** | The address country of the contact. | [optional] 
**ListName** | Pointer to **string** | The name of the list the contact belongs to. | [optional] 

## Methods

### NewContact

`func NewContact() *Contact`

NewContact instantiates a new Contact object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewContactWithDefaults

`func NewContactWithDefaults() *Contact`

NewContactWithDefaults instantiates a new Contact object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetContactId

`func (o *Contact) GetContactId() int32`

GetContactId returns the ContactId field if non-nil, zero value otherwise.

### GetContactIdOk

`func (o *Contact) GetContactIdOk() (*int32, bool)`

GetContactIdOk returns a tuple with the ContactId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetContactId

`func (o *Contact) SetContactId(v int32)`

SetContactId sets ContactId field to given value.

### HasContactId

`func (o *Contact) HasContactId() bool`

HasContactId returns a boolean if a field has been set.

### GetListId

`func (o *Contact) GetListId() int32`

GetListId returns the ListId field if non-nil, zero value otherwise.

### GetListIdOk

`func (o *Contact) GetListIdOk() (*int32, bool)`

GetListIdOk returns a tuple with the ListId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetListId

`func (o *Contact) SetListId(v int32)`

SetListId sets ListId field to given value.

### HasListId

`func (o *Contact) HasListId() bool`

HasListId returns a boolean if a field has been set.

### GetPhoneNumber

`func (o *Contact) GetPhoneNumber() string`

GetPhoneNumber returns the PhoneNumber field if non-nil, zero value otherwise.

### GetPhoneNumberOk

`func (o *Contact) GetPhoneNumberOk() (*string, bool)`

GetPhoneNumberOk returns a tuple with the PhoneNumber field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetPhoneNumber

`func (o *Contact) SetPhoneNumber(v string)`

SetPhoneNumber sets PhoneNumber field to given value.

### HasPhoneNumber

`func (o *Contact) HasPhoneNumber() bool`

HasPhoneNumber returns a boolean if a field has been set.

### GetFirstName

`func (o *Contact) GetFirstName() string`

GetFirstName returns the FirstName field if non-nil, zero value otherwise.

### GetFirstNameOk

`func (o *Contact) GetFirstNameOk() (*string, bool)`

GetFirstNameOk returns a tuple with the FirstName field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetFirstName

`func (o *Contact) SetFirstName(v string)`

SetFirstName sets FirstName field to given value.

### HasFirstName

`func (o *Contact) HasFirstName() bool`

HasFirstName returns a boolean if a field has been set.

### GetLastName

`func (o *Contact) GetLastName() string`

GetLastName returns the LastName field if non-nil, zero value otherwise.

### GetLastNameOk

`func (o *Contact) GetLastNameOk() (*string, bool)`

GetLastNameOk returns a tuple with the LastName field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetLastName

`func (o *Contact) SetLastName(v string)`

SetLastName sets LastName field to given value.

### HasLastName

`func (o *Contact) HasLastName() bool`

HasLastName returns a boolean if a field has been set.

### GetCustom1

`func (o *Contact) GetCustom1() string`

GetCustom1 returns the Custom1 field if non-nil, zero value otherwise.

### GetCustom1Ok

`func (o *Contact) GetCustom1Ok() (*string, bool)`

GetCustom1Ok returns a tuple with the Custom1 field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCustom1

`func (o *Contact) SetCustom1(v string)`

SetCustom1 sets Custom1 field to given value.

### HasCustom1

`func (o *Contact) HasCustom1() bool`

HasCustom1 returns a boolean if a field has been set.

### GetCustom2

`func (o *Contact) GetCustom2() string`

GetCustom2 returns the Custom2 field if non-nil, zero value otherwise.

### GetCustom2Ok

`func (o *Contact) GetCustom2Ok() (*string, bool)`

GetCustom2Ok returns a tuple with the Custom2 field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCustom2

`func (o *Contact) SetCustom2(v string)`

SetCustom2 sets Custom2 field to given value.

### HasCustom2

`func (o *Contact) HasCustom2() bool`

HasCustom2 returns a boolean if a field has been set.

### GetCustom3

`func (o *Contact) GetCustom3() string`

GetCustom3 returns the Custom3 field if non-nil, zero value otherwise.

### GetCustom3Ok

`func (o *Contact) GetCustom3Ok() (*string, bool)`

GetCustom3Ok returns a tuple with the Custom3 field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCustom3

`func (o *Contact) SetCustom3(v string)`

SetCustom3 sets Custom3 field to given value.

### HasCustom3

`func (o *Contact) HasCustom3() bool`

HasCustom3 returns a boolean if a field has been set.

### GetCustom4

`func (o *Contact) GetCustom4() string`

GetCustom4 returns the Custom4 field if non-nil, zero value otherwise.

### GetCustom4Ok

`func (o *Contact) GetCustom4Ok() (*string, bool)`

GetCustom4Ok returns a tuple with the Custom4 field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCustom4

`func (o *Contact) SetCustom4(v string)`

SetCustom4 sets Custom4 field to given value.

### HasCustom4

`func (o *Contact) HasCustom4() bool`

HasCustom4 returns a boolean if a field has been set.

### GetDateAdded

`func (o *Contact) GetDateAdded() string`

GetDateAdded returns the DateAdded field if non-nil, zero value otherwise.

### GetDateAddedOk

`func (o *Contact) GetDateAddedOk() (*string, bool)`

GetDateAddedOk returns a tuple with the DateAdded field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDateAdded

`func (o *Contact) SetDateAdded(v string)`

SetDateAdded sets DateAdded field to given value.

### HasDateAdded

`func (o *Contact) HasDateAdded() bool`

HasDateAdded returns a boolean if a field has been set.

### GetDateUpdated

`func (o *Contact) GetDateUpdated() string`

GetDateUpdated returns the DateUpdated field if non-nil, zero value otherwise.

### GetDateUpdatedOk

`func (o *Contact) GetDateUpdatedOk() (*string, bool)`

GetDateUpdatedOk returns a tuple with the DateUpdated field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDateUpdated

`func (o *Contact) SetDateUpdated(v string)`

SetDateUpdated sets DateUpdated field to given value.

### HasDateUpdated

`func (o *Contact) HasDateUpdated() bool`

HasDateUpdated returns a boolean if a field has been set.

### GetFaxNumber

`func (o *Contact) GetFaxNumber() string`

GetFaxNumber returns the FaxNumber field if non-nil, zero value otherwise.

### GetFaxNumberOk

`func (o *Contact) GetFaxNumberOk() (*string, bool)`

GetFaxNumberOk returns a tuple with the FaxNumber field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetFaxNumber

`func (o *Contact) SetFaxNumber(v string)`

SetFaxNumber sets FaxNumber field to given value.

### HasFaxNumber

`func (o *Contact) HasFaxNumber() bool`

HasFaxNumber returns a boolean if a field has been set.

### SetFaxNumberNil

`func (o *Contact) SetFaxNumberNil(b bool)`

 SetFaxNumberNil sets the value for FaxNumber to be an explicit nil

### UnsetFaxNumber
`func (o *Contact) UnsetFaxNumber()`

UnsetFaxNumber ensures that no value is present for FaxNumber, not even an explicit nil
### GetOrganizationName

`func (o *Contact) GetOrganizationName() string`

GetOrganizationName returns the OrganizationName field if non-nil, zero value otherwise.

### GetOrganizationNameOk

`func (o *Contact) GetOrganizationNameOk() (*string, bool)`

GetOrganizationNameOk returns a tuple with the OrganizationName field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetOrganizationName

`func (o *Contact) SetOrganizationName(v string)`

SetOrganizationName sets OrganizationName field to given value.

### HasOrganizationName

`func (o *Contact) HasOrganizationName() bool`

HasOrganizationName returns a boolean if a field has been set.

### SetOrganizationNameNil

`func (o *Contact) SetOrganizationNameNil(b bool)`

 SetOrganizationNameNil sets the value for OrganizationName to be an explicit nil

### UnsetOrganizationName
`func (o *Contact) UnsetOrganizationName()`

UnsetOrganizationName ensures that no value is present for OrganizationName, not even an explicit nil
### GetEmail

`func (o *Contact) GetEmail() string`

GetEmail returns the Email field if non-nil, zero value otherwise.

### GetEmailOk

`func (o *Contact) GetEmailOk() (*string, bool)`

GetEmailOk returns a tuple with the Email field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetEmail

`func (o *Contact) SetEmail(v string)`

SetEmail sets Email field to given value.

### HasEmail

`func (o *Contact) HasEmail() bool`

HasEmail returns a boolean if a field has been set.

### SetEmailNil

`func (o *Contact) SetEmailNil(b bool)`

 SetEmailNil sets the value for Email to be an explicit nil

### UnsetEmail
`func (o *Contact) UnsetEmail()`

UnsetEmail ensures that no value is present for Email, not even an explicit nil
### GetAddressLine1

`func (o *Contact) GetAddressLine1() string`

GetAddressLine1 returns the AddressLine1 field if non-nil, zero value otherwise.

### GetAddressLine1Ok

`func (o *Contact) GetAddressLine1Ok() (*string, bool)`

GetAddressLine1Ok returns a tuple with the AddressLine1 field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAddressLine1

`func (o *Contact) SetAddressLine1(v string)`

SetAddressLine1 sets AddressLine1 field to given value.

### HasAddressLine1

`func (o *Contact) HasAddressLine1() bool`

HasAddressLine1 returns a boolean if a field has been set.

### SetAddressLine1Nil

`func (o *Contact) SetAddressLine1Nil(b bool)`

 SetAddressLine1Nil sets the value for AddressLine1 to be an explicit nil

### UnsetAddressLine1
`func (o *Contact) UnsetAddressLine1()`

UnsetAddressLine1 ensures that no value is present for AddressLine1, not even an explicit nil
### GetAddressLine2

`func (o *Contact) GetAddressLine2() string`

GetAddressLine2 returns the AddressLine2 field if non-nil, zero value otherwise.

### GetAddressLine2Ok

`func (o *Contact) GetAddressLine2Ok() (*string, bool)`

GetAddressLine2Ok returns a tuple with the AddressLine2 field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAddressLine2

`func (o *Contact) SetAddressLine2(v string)`

SetAddressLine2 sets AddressLine2 field to given value.

### HasAddressLine2

`func (o *Contact) HasAddressLine2() bool`

HasAddressLine2 returns a boolean if a field has been set.

### SetAddressLine2Nil

`func (o *Contact) SetAddressLine2Nil(b bool)`

 SetAddressLine2Nil sets the value for AddressLine2 to be an explicit nil

### UnsetAddressLine2
`func (o *Contact) UnsetAddressLine2()`

UnsetAddressLine2 ensures that no value is present for AddressLine2, not even an explicit nil
### GetAddressCity

`func (o *Contact) GetAddressCity() string`

GetAddressCity returns the AddressCity field if non-nil, zero value otherwise.

### GetAddressCityOk

`func (o *Contact) GetAddressCityOk() (*string, bool)`

GetAddressCityOk returns a tuple with the AddressCity field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAddressCity

`func (o *Contact) SetAddressCity(v string)`

SetAddressCity sets AddressCity field to given value.

### HasAddressCity

`func (o *Contact) HasAddressCity() bool`

HasAddressCity returns a boolean if a field has been set.

### SetAddressCityNil

`func (o *Contact) SetAddressCityNil(b bool)`

 SetAddressCityNil sets the value for AddressCity to be an explicit nil

### UnsetAddressCity
`func (o *Contact) UnsetAddressCity()`

UnsetAddressCity ensures that no value is present for AddressCity, not even an explicit nil
### GetAddressState

`func (o *Contact) GetAddressState() string`

GetAddressState returns the AddressState field if non-nil, zero value otherwise.

### GetAddressStateOk

`func (o *Contact) GetAddressStateOk() (*string, bool)`

GetAddressStateOk returns a tuple with the AddressState field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAddressState

`func (o *Contact) SetAddressState(v string)`

SetAddressState sets AddressState field to given value.

### HasAddressState

`func (o *Contact) HasAddressState() bool`

HasAddressState returns a boolean if a field has been set.

### SetAddressStateNil

`func (o *Contact) SetAddressStateNil(b bool)`

 SetAddressStateNil sets the value for AddressState to be an explicit nil

### UnsetAddressState
`func (o *Contact) UnsetAddressState()`

UnsetAddressState ensures that no value is present for AddressState, not even an explicit nil
### GetAddressPostalCode

`func (o *Contact) GetAddressPostalCode() string`

GetAddressPostalCode returns the AddressPostalCode field if non-nil, zero value otherwise.

### GetAddressPostalCodeOk

`func (o *Contact) GetAddressPostalCodeOk() (*string, bool)`

GetAddressPostalCodeOk returns a tuple with the AddressPostalCode field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAddressPostalCode

`func (o *Contact) SetAddressPostalCode(v string)`

SetAddressPostalCode sets AddressPostalCode field to given value.

### HasAddressPostalCode

`func (o *Contact) HasAddressPostalCode() bool`

HasAddressPostalCode returns a boolean if a field has been set.

### SetAddressPostalCodeNil

`func (o *Contact) SetAddressPostalCodeNil(b bool)`

 SetAddressPostalCodeNil sets the value for AddressPostalCode to be an explicit nil

### UnsetAddressPostalCode
`func (o *Contact) UnsetAddressPostalCode()`

UnsetAddressPostalCode ensures that no value is present for AddressPostalCode, not even an explicit nil
### GetAddressCountry

`func (o *Contact) GetAddressCountry() string`

GetAddressCountry returns the AddressCountry field if non-nil, zero value otherwise.

### GetAddressCountryOk

`func (o *Contact) GetAddressCountryOk() (*string, bool)`

GetAddressCountryOk returns a tuple with the AddressCountry field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAddressCountry

`func (o *Contact) SetAddressCountry(v string)`

SetAddressCountry sets AddressCountry field to given value.

### HasAddressCountry

`func (o *Contact) HasAddressCountry() bool`

HasAddressCountry returns a boolean if a field has been set.

### SetAddressCountryNil

`func (o *Contact) SetAddressCountryNil(b bool)`

 SetAddressCountryNil sets the value for AddressCountry to be an explicit nil

### UnsetAddressCountry
`func (o *Contact) UnsetAddressCountry()`

UnsetAddressCountry ensures that no value is present for AddressCountry, not even an explicit nil
### GetListName

`func (o *Contact) GetListName() string`

GetListName returns the ListName field if non-nil, zero value otherwise.

### GetListNameOk

`func (o *Contact) GetListNameOk() (*string, bool)`

GetListNameOk returns a tuple with the ListName field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetListName

`func (o *Contact) SetListName(v string)`

SetListName sets ListName field to given value.

### HasListName

`func (o *Contact) HasListName() bool`

HasListName returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


