# OwnNumber

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Id** | Pointer to **string** | The unique identifier for the record. | [optional] 
**AccountId** | Pointer to **string** | The unique identifier for the account. | [optional] 
**WorkspaceId** | Pointer to **string** | The unique identifier for the workspace. | [optional] 
**UserId** | Pointer to **string** | The unique identifier for the user. | [optional] 
**PhoneNumber** | Pointer to **string** | The user&#39;s phone number. | [optional] 
**Country** | Pointer to **string** | The country code of the phone number. | [optional] 
**Label** | Pointer to **string** | A label for the phone number. | [optional] 
**Status** | Pointer to **string** | The status of the phone number. | [optional] 
**VerifiedTimestamp** | Pointer to **time.Time** | The timestamp when the phone number was verified. | [optional] 
**IsNearingExpiration** | Pointer to **bool** | Indicates whether the phone number verification is nearing its expiration date: - **true:** The verification was completed more than 11 months ago and will expire soon. You should re-verify your phone number to maintain uninterrupted service. - **false:** The verification is still valid and not approaching expiration. | [optional] 
**CreatedTimestamp** | Pointer to **time.Time** | The timestamp when the record was created. | [optional] 
**UpdatedTimestamp** | Pointer to **time.Time** | The timestamp when the record was last updated. | [optional] 

## Methods

### NewOwnNumber

`func NewOwnNumber() *OwnNumber`

NewOwnNumber instantiates a new OwnNumber object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewOwnNumberWithDefaults

`func NewOwnNumberWithDefaults() *OwnNumber`

NewOwnNumberWithDefaults instantiates a new OwnNumber object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetId

`func (o *OwnNumber) GetId() string`

GetId returns the Id field if non-nil, zero value otherwise.

### GetIdOk

`func (o *OwnNumber) GetIdOk() (*string, bool)`

GetIdOk returns a tuple with the Id field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetId

`func (o *OwnNumber) SetId(v string)`

SetId sets Id field to given value.

### HasId

`func (o *OwnNumber) HasId() bool`

HasId returns a boolean if a field has been set.

### GetAccountId

`func (o *OwnNumber) GetAccountId() string`

GetAccountId returns the AccountId field if non-nil, zero value otherwise.

### GetAccountIdOk

`func (o *OwnNumber) GetAccountIdOk() (*string, bool)`

GetAccountIdOk returns a tuple with the AccountId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAccountId

`func (o *OwnNumber) SetAccountId(v string)`

SetAccountId sets AccountId field to given value.

### HasAccountId

`func (o *OwnNumber) HasAccountId() bool`

HasAccountId returns a boolean if a field has been set.

### GetWorkspaceId

`func (o *OwnNumber) GetWorkspaceId() string`

GetWorkspaceId returns the WorkspaceId field if non-nil, zero value otherwise.

### GetWorkspaceIdOk

`func (o *OwnNumber) GetWorkspaceIdOk() (*string, bool)`

GetWorkspaceIdOk returns a tuple with the WorkspaceId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetWorkspaceId

`func (o *OwnNumber) SetWorkspaceId(v string)`

SetWorkspaceId sets WorkspaceId field to given value.

### HasWorkspaceId

`func (o *OwnNumber) HasWorkspaceId() bool`

HasWorkspaceId returns a boolean if a field has been set.

### GetUserId

`func (o *OwnNumber) GetUserId() string`

GetUserId returns the UserId field if non-nil, zero value otherwise.

### GetUserIdOk

`func (o *OwnNumber) GetUserIdOk() (*string, bool)`

GetUserIdOk returns a tuple with the UserId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetUserId

`func (o *OwnNumber) SetUserId(v string)`

SetUserId sets UserId field to given value.

### HasUserId

`func (o *OwnNumber) HasUserId() bool`

HasUserId returns a boolean if a field has been set.

### GetPhoneNumber

`func (o *OwnNumber) GetPhoneNumber() string`

GetPhoneNumber returns the PhoneNumber field if non-nil, zero value otherwise.

### GetPhoneNumberOk

`func (o *OwnNumber) GetPhoneNumberOk() (*string, bool)`

GetPhoneNumberOk returns a tuple with the PhoneNumber field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetPhoneNumber

`func (o *OwnNumber) SetPhoneNumber(v string)`

SetPhoneNumber sets PhoneNumber field to given value.

### HasPhoneNumber

`func (o *OwnNumber) HasPhoneNumber() bool`

HasPhoneNumber returns a boolean if a field has been set.

### GetCountry

`func (o *OwnNumber) GetCountry() string`

GetCountry returns the Country field if non-nil, zero value otherwise.

### GetCountryOk

`func (o *OwnNumber) GetCountryOk() (*string, bool)`

GetCountryOk returns a tuple with the Country field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCountry

`func (o *OwnNumber) SetCountry(v string)`

SetCountry sets Country field to given value.

### HasCountry

`func (o *OwnNumber) HasCountry() bool`

HasCountry returns a boolean if a field has been set.

### GetLabel

`func (o *OwnNumber) GetLabel() string`

GetLabel returns the Label field if non-nil, zero value otherwise.

### GetLabelOk

`func (o *OwnNumber) GetLabelOk() (*string, bool)`

GetLabelOk returns a tuple with the Label field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetLabel

`func (o *OwnNumber) SetLabel(v string)`

SetLabel sets Label field to given value.

### HasLabel

`func (o *OwnNumber) HasLabel() bool`

HasLabel returns a boolean if a field has been set.

### GetStatus

`func (o *OwnNumber) GetStatus() string`

GetStatus returns the Status field if non-nil, zero value otherwise.

### GetStatusOk

`func (o *OwnNumber) GetStatusOk() (*string, bool)`

GetStatusOk returns a tuple with the Status field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetStatus

`func (o *OwnNumber) SetStatus(v string)`

SetStatus sets Status field to given value.

### HasStatus

`func (o *OwnNumber) HasStatus() bool`

HasStatus returns a boolean if a field has been set.

### GetVerifiedTimestamp

`func (o *OwnNumber) GetVerifiedTimestamp() time.Time`

GetVerifiedTimestamp returns the VerifiedTimestamp field if non-nil, zero value otherwise.

### GetVerifiedTimestampOk

`func (o *OwnNumber) GetVerifiedTimestampOk() (*time.Time, bool)`

GetVerifiedTimestampOk returns a tuple with the VerifiedTimestamp field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetVerifiedTimestamp

`func (o *OwnNumber) SetVerifiedTimestamp(v time.Time)`

SetVerifiedTimestamp sets VerifiedTimestamp field to given value.

### HasVerifiedTimestamp

`func (o *OwnNumber) HasVerifiedTimestamp() bool`

HasVerifiedTimestamp returns a boolean if a field has been set.

### GetIsNearingExpiration

`func (o *OwnNumber) GetIsNearingExpiration() bool`

GetIsNearingExpiration returns the IsNearingExpiration field if non-nil, zero value otherwise.

### GetIsNearingExpirationOk

`func (o *OwnNumber) GetIsNearingExpirationOk() (*bool, bool)`

GetIsNearingExpirationOk returns a tuple with the IsNearingExpiration field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetIsNearingExpiration

`func (o *OwnNumber) SetIsNearingExpiration(v bool)`

SetIsNearingExpiration sets IsNearingExpiration field to given value.

### HasIsNearingExpiration

`func (o *OwnNumber) HasIsNearingExpiration() bool`

HasIsNearingExpiration returns a boolean if a field has been set.

### GetCreatedTimestamp

`func (o *OwnNumber) GetCreatedTimestamp() time.Time`

GetCreatedTimestamp returns the CreatedTimestamp field if non-nil, zero value otherwise.

### GetCreatedTimestampOk

`func (o *OwnNumber) GetCreatedTimestampOk() (*time.Time, bool)`

GetCreatedTimestampOk returns a tuple with the CreatedTimestamp field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCreatedTimestamp

`func (o *OwnNumber) SetCreatedTimestamp(v time.Time)`

SetCreatedTimestamp sets CreatedTimestamp field to given value.

### HasCreatedTimestamp

`func (o *OwnNumber) HasCreatedTimestamp() bool`

HasCreatedTimestamp returns a boolean if a field has been set.

### GetUpdatedTimestamp

`func (o *OwnNumber) GetUpdatedTimestamp() time.Time`

GetUpdatedTimestamp returns the UpdatedTimestamp field if non-nil, zero value otherwise.

### GetUpdatedTimestampOk

`func (o *OwnNumber) GetUpdatedTimestampOk() (*time.Time, bool)`

GetUpdatedTimestampOk returns a tuple with the UpdatedTimestamp field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetUpdatedTimestamp

`func (o *OwnNumber) SetUpdatedTimestamp(v time.Time)`

SetUpdatedTimestamp sets UpdatedTimestamp field to given value.

### HasUpdatedTimestamp

`func (o *OwnNumber) HasUpdatedTimestamp() bool`

HasUpdatedTimestamp returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


