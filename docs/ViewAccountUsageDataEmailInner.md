# ViewAccountUsageDataEmailInner

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**SubaccountId** | Pointer to **int32** | The subaccount identifier. | [optional] 
**Username** | Pointer to **string** | The username associated with the subaccount. | [optional] 
**TotalCount** | Pointer to **int32** | The total count of emails. | [optional] 
**TotalPrice** | Pointer to **float32** |  | [optional] 
**Notes** | Pointer to **NullableString** | Optional notes. | [optional] 

## Methods

### NewViewAccountUsageDataEmailInner

`func NewViewAccountUsageDataEmailInner() *ViewAccountUsageDataEmailInner`

NewViewAccountUsageDataEmailInner instantiates a new ViewAccountUsageDataEmailInner object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewViewAccountUsageDataEmailInnerWithDefaults

`func NewViewAccountUsageDataEmailInnerWithDefaults() *ViewAccountUsageDataEmailInner`

NewViewAccountUsageDataEmailInnerWithDefaults instantiates a new ViewAccountUsageDataEmailInner object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetSubaccountId

`func (o *ViewAccountUsageDataEmailInner) GetSubaccountId() int32`

GetSubaccountId returns the SubaccountId field if non-nil, zero value otherwise.

### GetSubaccountIdOk

`func (o *ViewAccountUsageDataEmailInner) GetSubaccountIdOk() (*int32, bool)`

GetSubaccountIdOk returns a tuple with the SubaccountId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSubaccountId

`func (o *ViewAccountUsageDataEmailInner) SetSubaccountId(v int32)`

SetSubaccountId sets SubaccountId field to given value.

### HasSubaccountId

`func (o *ViewAccountUsageDataEmailInner) HasSubaccountId() bool`

HasSubaccountId returns a boolean if a field has been set.

### GetUsername

`func (o *ViewAccountUsageDataEmailInner) GetUsername() string`

GetUsername returns the Username field if non-nil, zero value otherwise.

### GetUsernameOk

`func (o *ViewAccountUsageDataEmailInner) GetUsernameOk() (*string, bool)`

GetUsernameOk returns a tuple with the Username field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetUsername

`func (o *ViewAccountUsageDataEmailInner) SetUsername(v string)`

SetUsername sets Username field to given value.

### HasUsername

`func (o *ViewAccountUsageDataEmailInner) HasUsername() bool`

HasUsername returns a boolean if a field has been set.

### GetTotalCount

`func (o *ViewAccountUsageDataEmailInner) GetTotalCount() int32`

GetTotalCount returns the TotalCount field if non-nil, zero value otherwise.

### GetTotalCountOk

`func (o *ViewAccountUsageDataEmailInner) GetTotalCountOk() (*int32, bool)`

GetTotalCountOk returns a tuple with the TotalCount field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTotalCount

`func (o *ViewAccountUsageDataEmailInner) SetTotalCount(v int32)`

SetTotalCount sets TotalCount field to given value.

### HasTotalCount

`func (o *ViewAccountUsageDataEmailInner) HasTotalCount() bool`

HasTotalCount returns a boolean if a field has been set.

### GetTotalPrice

`func (o *ViewAccountUsageDataEmailInner) GetTotalPrice() float32`

GetTotalPrice returns the TotalPrice field if non-nil, zero value otherwise.

### GetTotalPriceOk

`func (o *ViewAccountUsageDataEmailInner) GetTotalPriceOk() (*float32, bool)`

GetTotalPriceOk returns a tuple with the TotalPrice field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTotalPrice

`func (o *ViewAccountUsageDataEmailInner) SetTotalPrice(v float32)`

SetTotalPrice sets TotalPrice field to given value.

### HasTotalPrice

`func (o *ViewAccountUsageDataEmailInner) HasTotalPrice() bool`

HasTotalPrice returns a boolean if a field has been set.

### GetNotes

`func (o *ViewAccountUsageDataEmailInner) GetNotes() string`

GetNotes returns the Notes field if non-nil, zero value otherwise.

### GetNotesOk

`func (o *ViewAccountUsageDataEmailInner) GetNotesOk() (*string, bool)`

GetNotesOk returns a tuple with the Notes field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetNotes

`func (o *ViewAccountUsageDataEmailInner) SetNotes(v string)`

SetNotes sets Notes field to given value.

### HasNotes

`func (o *ViewAccountUsageDataEmailInner) HasNotes() bool`

HasNotes returns a boolean if a field has been set.

### SetNotesNil

`func (o *ViewAccountUsageDataEmailInner) SetNotesNil(b bool)`

 SetNotesNil sets the value for Notes to be an explicit nil

### UnsetNotes
`func (o *ViewAccountUsageDataEmailInner) UnsetNotes()`

UnsetNotes ensures that no value is present for Notes, not even an explicit nil

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


