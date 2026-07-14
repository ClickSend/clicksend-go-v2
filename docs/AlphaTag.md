# AlphaTag

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Id** | Pointer to **string** | The unique identifier for the record. | [optional] 
**AccountId** | Pointer to **string** | The unique identifier for the account. | [optional] 
**WorkspaceId** | Pointer to **string** | The unique identifier for the workspace. | [optional] 
**UserId** | Pointer to **string** | The unique identifier for the user. | [optional] 
**AlphaTag** | Pointer to **string** | The alpha tag. | [optional] 
**Status** | Pointer to **string** | The status of the record. | [optional] 
**Reason** | Pointer to **string** | The reason for the status. | [optional] 
**Countries** | Pointer to **[]string** | List of country codes where the alpha tag is requested. If not provided, it means a global alpha tag. | [optional] 
**CreatedTimestamp** | Pointer to **string** | The timestamp when the record was created. Usually ISO 8601 (e.g. \&quot;2021-05-11T01:00:00.123Z\&quot;), but returned as a plain string rather than a strict date-time since some older records don&#39;t include a UTC offset (e.g. \&quot;2024-01-10T10:55:26.818097\&quot;). | [optional] 
**UpdatedTimestamp** | Pointer to **string** | The timestamp when the record was last updated. Usually ISO 8601 (e.g. \&quot;2021-05-11T01:05:00.123Z\&quot;), but returned as a plain string rather than a strict date-time since some older records don&#39;t include a UTC offset. | [optional] 

## Methods

### NewAlphaTag

`func NewAlphaTag() *AlphaTag`

NewAlphaTag instantiates a new AlphaTag object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewAlphaTagWithDefaults

`func NewAlphaTagWithDefaults() *AlphaTag`

NewAlphaTagWithDefaults instantiates a new AlphaTag object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetId

`func (o *AlphaTag) GetId() string`

GetId returns the Id field if non-nil, zero value otherwise.

### GetIdOk

`func (o *AlphaTag) GetIdOk() (*string, bool)`

GetIdOk returns a tuple with the Id field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetId

`func (o *AlphaTag) SetId(v string)`

SetId sets Id field to given value.

### HasId

`func (o *AlphaTag) HasId() bool`

HasId returns a boolean if a field has been set.

### GetAccountId

`func (o *AlphaTag) GetAccountId() string`

GetAccountId returns the AccountId field if non-nil, zero value otherwise.

### GetAccountIdOk

`func (o *AlphaTag) GetAccountIdOk() (*string, bool)`

GetAccountIdOk returns a tuple with the AccountId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAccountId

`func (o *AlphaTag) SetAccountId(v string)`

SetAccountId sets AccountId field to given value.

### HasAccountId

`func (o *AlphaTag) HasAccountId() bool`

HasAccountId returns a boolean if a field has been set.

### GetWorkspaceId

`func (o *AlphaTag) GetWorkspaceId() string`

GetWorkspaceId returns the WorkspaceId field if non-nil, zero value otherwise.

### GetWorkspaceIdOk

`func (o *AlphaTag) GetWorkspaceIdOk() (*string, bool)`

GetWorkspaceIdOk returns a tuple with the WorkspaceId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetWorkspaceId

`func (o *AlphaTag) SetWorkspaceId(v string)`

SetWorkspaceId sets WorkspaceId field to given value.

### HasWorkspaceId

`func (o *AlphaTag) HasWorkspaceId() bool`

HasWorkspaceId returns a boolean if a field has been set.

### GetUserId

`func (o *AlphaTag) GetUserId() string`

GetUserId returns the UserId field if non-nil, zero value otherwise.

### GetUserIdOk

`func (o *AlphaTag) GetUserIdOk() (*string, bool)`

GetUserIdOk returns a tuple with the UserId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetUserId

`func (o *AlphaTag) SetUserId(v string)`

SetUserId sets UserId field to given value.

### HasUserId

`func (o *AlphaTag) HasUserId() bool`

HasUserId returns a boolean if a field has been set.

### GetAlphaTag

`func (o *AlphaTag) GetAlphaTag() string`

GetAlphaTag returns the AlphaTag field if non-nil, zero value otherwise.

### GetAlphaTagOk

`func (o *AlphaTag) GetAlphaTagOk() (*string, bool)`

GetAlphaTagOk returns a tuple with the AlphaTag field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAlphaTag

`func (o *AlphaTag) SetAlphaTag(v string)`

SetAlphaTag sets AlphaTag field to given value.

### HasAlphaTag

`func (o *AlphaTag) HasAlphaTag() bool`

HasAlphaTag returns a boolean if a field has been set.

### GetStatus

`func (o *AlphaTag) GetStatus() string`

GetStatus returns the Status field if non-nil, zero value otherwise.

### GetStatusOk

`func (o *AlphaTag) GetStatusOk() (*string, bool)`

GetStatusOk returns a tuple with the Status field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetStatus

`func (o *AlphaTag) SetStatus(v string)`

SetStatus sets Status field to given value.

### HasStatus

`func (o *AlphaTag) HasStatus() bool`

HasStatus returns a boolean if a field has been set.

### GetReason

`func (o *AlphaTag) GetReason() string`

GetReason returns the Reason field if non-nil, zero value otherwise.

### GetReasonOk

`func (o *AlphaTag) GetReasonOk() (*string, bool)`

GetReasonOk returns a tuple with the Reason field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetReason

`func (o *AlphaTag) SetReason(v string)`

SetReason sets Reason field to given value.

### HasReason

`func (o *AlphaTag) HasReason() bool`

HasReason returns a boolean if a field has been set.

### GetCountries

`func (o *AlphaTag) GetCountries() []string`

GetCountries returns the Countries field if non-nil, zero value otherwise.

### GetCountriesOk

`func (o *AlphaTag) GetCountriesOk() (*[]string, bool)`

GetCountriesOk returns a tuple with the Countries field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCountries

`func (o *AlphaTag) SetCountries(v []string)`

SetCountries sets Countries field to given value.

### HasCountries

`func (o *AlphaTag) HasCountries() bool`

HasCountries returns a boolean if a field has been set.

### SetCountriesNil

`func (o *AlphaTag) SetCountriesNil(b bool)`

 SetCountriesNil sets the value for Countries to be an explicit nil

### UnsetCountries
`func (o *AlphaTag) UnsetCountries()`

UnsetCountries ensures that no value is present for Countries, not even an explicit nil
### GetCreatedTimestamp

`func (o *AlphaTag) GetCreatedTimestamp() string`

GetCreatedTimestamp returns the CreatedTimestamp field if non-nil, zero value otherwise.

### GetCreatedTimestampOk

`func (o *AlphaTag) GetCreatedTimestampOk() (*string, bool)`

GetCreatedTimestampOk returns a tuple with the CreatedTimestamp field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCreatedTimestamp

`func (o *AlphaTag) SetCreatedTimestamp(v string)`

SetCreatedTimestamp sets CreatedTimestamp field to given value.

### HasCreatedTimestamp

`func (o *AlphaTag) HasCreatedTimestamp() bool`

HasCreatedTimestamp returns a boolean if a field has been set.

### GetUpdatedTimestamp

`func (o *AlphaTag) GetUpdatedTimestamp() string`

GetUpdatedTimestamp returns the UpdatedTimestamp field if non-nil, zero value otherwise.

### GetUpdatedTimestampOk

`func (o *AlphaTag) GetUpdatedTimestampOk() (*string, bool)`

GetUpdatedTimestampOk returns a tuple with the UpdatedTimestamp field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetUpdatedTimestamp

`func (o *AlphaTag) SetUpdatedTimestamp(v string)`

SetUpdatedTimestamp sets UpdatedTimestamp field to given value.

### HasUpdatedTimestamp

`func (o *AlphaTag) HasUpdatedTimestamp() bool`

HasUpdatedTimestamp returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


