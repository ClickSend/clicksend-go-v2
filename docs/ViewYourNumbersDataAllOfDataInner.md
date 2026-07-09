# ViewYourNumbersDataAllOfDataInner

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**DedicatedNumber** | Pointer to **string** | The dedicated number. | [optional] 
**Country** | Pointer to **string** | The country. | [optional] 
**Price** | Pointer to **string** | The price. | [optional] 
**CountryName** | Pointer to **string** | The country name. | [optional] 
**Notes** | Pointer to **NullableString** | Optional notes about the number. | [optional] 
**Type** | Pointer to **string** | The type of messages this number can send. | [optional] 
**NumberType** | Pointer to **string** | The classification of the number. | [optional] 
**NumberCategory** | Pointer to **NullableString** | The category of the number. | [optional] 
**NumberGuid** | Pointer to **string** | Unique identifier for the number. | [optional] 
**FormSubmissionId** | Pointer to **NullableString** | ID of any associated form submission. | [optional] 
**Status** | Pointer to [**ViewYourNumbersDataAllOfDataInnerStatus**](ViewYourNumbersDataAllOfDataInnerStatus.md) |  | [optional] 

## Methods

### NewViewYourNumbersDataAllOfDataInner

`func NewViewYourNumbersDataAllOfDataInner() *ViewYourNumbersDataAllOfDataInner`

NewViewYourNumbersDataAllOfDataInner instantiates a new ViewYourNumbersDataAllOfDataInner object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewViewYourNumbersDataAllOfDataInnerWithDefaults

`func NewViewYourNumbersDataAllOfDataInnerWithDefaults() *ViewYourNumbersDataAllOfDataInner`

NewViewYourNumbersDataAllOfDataInnerWithDefaults instantiates a new ViewYourNumbersDataAllOfDataInner object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetDedicatedNumber

`func (o *ViewYourNumbersDataAllOfDataInner) GetDedicatedNumber() string`

GetDedicatedNumber returns the DedicatedNumber field if non-nil, zero value otherwise.

### GetDedicatedNumberOk

`func (o *ViewYourNumbersDataAllOfDataInner) GetDedicatedNumberOk() (*string, bool)`

GetDedicatedNumberOk returns a tuple with the DedicatedNumber field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDedicatedNumber

`func (o *ViewYourNumbersDataAllOfDataInner) SetDedicatedNumber(v string)`

SetDedicatedNumber sets DedicatedNumber field to given value.

### HasDedicatedNumber

`func (o *ViewYourNumbersDataAllOfDataInner) HasDedicatedNumber() bool`

HasDedicatedNumber returns a boolean if a field has been set.

### GetCountry

`func (o *ViewYourNumbersDataAllOfDataInner) GetCountry() string`

GetCountry returns the Country field if non-nil, zero value otherwise.

### GetCountryOk

`func (o *ViewYourNumbersDataAllOfDataInner) GetCountryOk() (*string, bool)`

GetCountryOk returns a tuple with the Country field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCountry

`func (o *ViewYourNumbersDataAllOfDataInner) SetCountry(v string)`

SetCountry sets Country field to given value.

### HasCountry

`func (o *ViewYourNumbersDataAllOfDataInner) HasCountry() bool`

HasCountry returns a boolean if a field has been set.

### GetPrice

`func (o *ViewYourNumbersDataAllOfDataInner) GetPrice() string`

GetPrice returns the Price field if non-nil, zero value otherwise.

### GetPriceOk

`func (o *ViewYourNumbersDataAllOfDataInner) GetPriceOk() (*string, bool)`

GetPriceOk returns a tuple with the Price field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetPrice

`func (o *ViewYourNumbersDataAllOfDataInner) SetPrice(v string)`

SetPrice sets Price field to given value.

### HasPrice

`func (o *ViewYourNumbersDataAllOfDataInner) HasPrice() bool`

HasPrice returns a boolean if a field has been set.

### GetCountryName

`func (o *ViewYourNumbersDataAllOfDataInner) GetCountryName() string`

GetCountryName returns the CountryName field if non-nil, zero value otherwise.

### GetCountryNameOk

`func (o *ViewYourNumbersDataAllOfDataInner) GetCountryNameOk() (*string, bool)`

GetCountryNameOk returns a tuple with the CountryName field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCountryName

`func (o *ViewYourNumbersDataAllOfDataInner) SetCountryName(v string)`

SetCountryName sets CountryName field to given value.

### HasCountryName

`func (o *ViewYourNumbersDataAllOfDataInner) HasCountryName() bool`

HasCountryName returns a boolean if a field has been set.

### GetNotes

`func (o *ViewYourNumbersDataAllOfDataInner) GetNotes() string`

GetNotes returns the Notes field if non-nil, zero value otherwise.

### GetNotesOk

`func (o *ViewYourNumbersDataAllOfDataInner) GetNotesOk() (*string, bool)`

GetNotesOk returns a tuple with the Notes field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetNotes

`func (o *ViewYourNumbersDataAllOfDataInner) SetNotes(v string)`

SetNotes sets Notes field to given value.

### HasNotes

`func (o *ViewYourNumbersDataAllOfDataInner) HasNotes() bool`

HasNotes returns a boolean if a field has been set.

### SetNotesNil

`func (o *ViewYourNumbersDataAllOfDataInner) SetNotesNil(b bool)`

 SetNotesNil sets the value for Notes to be an explicit nil

### UnsetNotes
`func (o *ViewYourNumbersDataAllOfDataInner) UnsetNotes()`

UnsetNotes ensures that no value is present for Notes, not even an explicit nil
### GetType

`func (o *ViewYourNumbersDataAllOfDataInner) GetType() string`

GetType returns the Type field if non-nil, zero value otherwise.

### GetTypeOk

`func (o *ViewYourNumbersDataAllOfDataInner) GetTypeOk() (*string, bool)`

GetTypeOk returns a tuple with the Type field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetType

`func (o *ViewYourNumbersDataAllOfDataInner) SetType(v string)`

SetType sets Type field to given value.

### HasType

`func (o *ViewYourNumbersDataAllOfDataInner) HasType() bool`

HasType returns a boolean if a field has been set.

### GetNumberType

`func (o *ViewYourNumbersDataAllOfDataInner) GetNumberType() string`

GetNumberType returns the NumberType field if non-nil, zero value otherwise.

### GetNumberTypeOk

`func (o *ViewYourNumbersDataAllOfDataInner) GetNumberTypeOk() (*string, bool)`

GetNumberTypeOk returns a tuple with the NumberType field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetNumberType

`func (o *ViewYourNumbersDataAllOfDataInner) SetNumberType(v string)`

SetNumberType sets NumberType field to given value.

### HasNumberType

`func (o *ViewYourNumbersDataAllOfDataInner) HasNumberType() bool`

HasNumberType returns a boolean if a field has been set.

### GetNumberCategory

`func (o *ViewYourNumbersDataAllOfDataInner) GetNumberCategory() string`

GetNumberCategory returns the NumberCategory field if non-nil, zero value otherwise.

### GetNumberCategoryOk

`func (o *ViewYourNumbersDataAllOfDataInner) GetNumberCategoryOk() (*string, bool)`

GetNumberCategoryOk returns a tuple with the NumberCategory field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetNumberCategory

`func (o *ViewYourNumbersDataAllOfDataInner) SetNumberCategory(v string)`

SetNumberCategory sets NumberCategory field to given value.

### HasNumberCategory

`func (o *ViewYourNumbersDataAllOfDataInner) HasNumberCategory() bool`

HasNumberCategory returns a boolean if a field has been set.

### SetNumberCategoryNil

`func (o *ViewYourNumbersDataAllOfDataInner) SetNumberCategoryNil(b bool)`

 SetNumberCategoryNil sets the value for NumberCategory to be an explicit nil

### UnsetNumberCategory
`func (o *ViewYourNumbersDataAllOfDataInner) UnsetNumberCategory()`

UnsetNumberCategory ensures that no value is present for NumberCategory, not even an explicit nil
### GetNumberGuid

`func (o *ViewYourNumbersDataAllOfDataInner) GetNumberGuid() string`

GetNumberGuid returns the NumberGuid field if non-nil, zero value otherwise.

### GetNumberGuidOk

`func (o *ViewYourNumbersDataAllOfDataInner) GetNumberGuidOk() (*string, bool)`

GetNumberGuidOk returns a tuple with the NumberGuid field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetNumberGuid

`func (o *ViewYourNumbersDataAllOfDataInner) SetNumberGuid(v string)`

SetNumberGuid sets NumberGuid field to given value.

### HasNumberGuid

`func (o *ViewYourNumbersDataAllOfDataInner) HasNumberGuid() bool`

HasNumberGuid returns a boolean if a field has been set.

### GetFormSubmissionId

`func (o *ViewYourNumbersDataAllOfDataInner) GetFormSubmissionId() string`

GetFormSubmissionId returns the FormSubmissionId field if non-nil, zero value otherwise.

### GetFormSubmissionIdOk

`func (o *ViewYourNumbersDataAllOfDataInner) GetFormSubmissionIdOk() (*string, bool)`

GetFormSubmissionIdOk returns a tuple with the FormSubmissionId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetFormSubmissionId

`func (o *ViewYourNumbersDataAllOfDataInner) SetFormSubmissionId(v string)`

SetFormSubmissionId sets FormSubmissionId field to given value.

### HasFormSubmissionId

`func (o *ViewYourNumbersDataAllOfDataInner) HasFormSubmissionId() bool`

HasFormSubmissionId returns a boolean if a field has been set.

### SetFormSubmissionIdNil

`func (o *ViewYourNumbersDataAllOfDataInner) SetFormSubmissionIdNil(b bool)`

 SetFormSubmissionIdNil sets the value for FormSubmissionId to be an explicit nil

### UnsetFormSubmissionId
`func (o *ViewYourNumbersDataAllOfDataInner) UnsetFormSubmissionId()`

UnsetFormSubmissionId ensures that no value is present for FormSubmissionId, not even an explicit nil
### GetStatus

`func (o *ViewYourNumbersDataAllOfDataInner) GetStatus() ViewYourNumbersDataAllOfDataInnerStatus`

GetStatus returns the Status field if non-nil, zero value otherwise.

### GetStatusOk

`func (o *ViewYourNumbersDataAllOfDataInner) GetStatusOk() (*ViewYourNumbersDataAllOfDataInnerStatus, bool)`

GetStatusOk returns a tuple with the Status field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetStatus

`func (o *ViewYourNumbersDataAllOfDataInner) SetStatus(v ViewYourNumbersDataAllOfDataInnerStatus)`

SetStatus sets Status field to given value.

### HasStatus

`func (o *ViewYourNumbersDataAllOfDataInner) HasStatus() bool`

HasStatus returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


