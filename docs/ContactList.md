# ContactList

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**ListId** | Pointer to **int32** | The unique identifier for the list. | [optional] 
**ListName** | Pointer to **string** | The name of the list. | [optional] 
**ListEmailId** | Pointer to **string** | The email address id of the list. | [optional] 
**ContactsCount** | Pointer to **int32** | The number of contacts in the list. | [optional] 
**ImportInProgress** | Pointer to **int32** | Flag indicating if a contact import is currently in progress for this list. | [optional] 
**OptoutInProgress** | Pointer to **int32** | Flag indicating if an opt-out removal is currently in progress for this list. | [optional] 

## Methods

### NewContactList

`func NewContactList() *ContactList`

NewContactList instantiates a new ContactList object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewContactListWithDefaults

`func NewContactListWithDefaults() *ContactList`

NewContactListWithDefaults instantiates a new ContactList object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetListId

`func (o *ContactList) GetListId() int32`

GetListId returns the ListId field if non-nil, zero value otherwise.

### GetListIdOk

`func (o *ContactList) GetListIdOk() (*int32, bool)`

GetListIdOk returns a tuple with the ListId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetListId

`func (o *ContactList) SetListId(v int32)`

SetListId sets ListId field to given value.

### HasListId

`func (o *ContactList) HasListId() bool`

HasListId returns a boolean if a field has been set.

### GetListName

`func (o *ContactList) GetListName() string`

GetListName returns the ListName field if non-nil, zero value otherwise.

### GetListNameOk

`func (o *ContactList) GetListNameOk() (*string, bool)`

GetListNameOk returns a tuple with the ListName field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetListName

`func (o *ContactList) SetListName(v string)`

SetListName sets ListName field to given value.

### HasListName

`func (o *ContactList) HasListName() bool`

HasListName returns a boolean if a field has been set.

### GetListEmailId

`func (o *ContactList) GetListEmailId() string`

GetListEmailId returns the ListEmailId field if non-nil, zero value otherwise.

### GetListEmailIdOk

`func (o *ContactList) GetListEmailIdOk() (*string, bool)`

GetListEmailIdOk returns a tuple with the ListEmailId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetListEmailId

`func (o *ContactList) SetListEmailId(v string)`

SetListEmailId sets ListEmailId field to given value.

### HasListEmailId

`func (o *ContactList) HasListEmailId() bool`

HasListEmailId returns a boolean if a field has been set.

### GetContactsCount

`func (o *ContactList) GetContactsCount() int32`

GetContactsCount returns the ContactsCount field if non-nil, zero value otherwise.

### GetContactsCountOk

`func (o *ContactList) GetContactsCountOk() (*int32, bool)`

GetContactsCountOk returns a tuple with the ContactsCount field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetContactsCount

`func (o *ContactList) SetContactsCount(v int32)`

SetContactsCount sets ContactsCount field to given value.

### HasContactsCount

`func (o *ContactList) HasContactsCount() bool`

HasContactsCount returns a boolean if a field has been set.

### GetImportInProgress

`func (o *ContactList) GetImportInProgress() int32`

GetImportInProgress returns the ImportInProgress field if non-nil, zero value otherwise.

### GetImportInProgressOk

`func (o *ContactList) GetImportInProgressOk() (*int32, bool)`

GetImportInProgressOk returns a tuple with the ImportInProgress field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetImportInProgress

`func (o *ContactList) SetImportInProgress(v int32)`

SetImportInProgress sets ImportInProgress field to given value.

### HasImportInProgress

`func (o *ContactList) HasImportInProgress() bool`

HasImportInProgress returns a boolean if a field has been set.

### GetOptoutInProgress

`func (o *ContactList) GetOptoutInProgress() int32`

GetOptoutInProgress returns the OptoutInProgress field if non-nil, zero value otherwise.

### GetOptoutInProgressOk

`func (o *ContactList) GetOptoutInProgressOk() (*int32, bool)`

GetOptoutInProgressOk returns a tuple with the OptoutInProgress field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetOptoutInProgress

`func (o *ContactList) SetOptoutInProgress(v int32)`

SetOptoutInProgress sets OptoutInProgress field to given value.

### HasOptoutInProgress

`func (o *ContactList) HasOptoutInProgress() bool`

HasOptoutInProgress returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


