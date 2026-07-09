# ViewYourNumbersDataAllOfDataInnerStatus

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Value** | Pointer to **int32** | Numeric status code (0-5): - 0: Your number is ready to go. - 1: Your number is unregistered. You will not be able to send messages to certain countries. - 2: Your number registration is in progress. Email updates will follow. - 3: Action required on your number registration. Please resolve to start using it. - 4: You can send to all countries but may get restricted to some before full registration. - 5: Your number is registered and you can start using it immediately.  | [optional] 
**Label** | Pointer to **string** | Status label identifier corresponding to the numeric value above, following the same order. | [optional] 
**Description** | Pointer to **string** | Human readable description of the status. | [optional] 
**Name** | Pointer to **string** | Display name for the status corresponding to the numeric value above, following the same order. | [optional] 

## Methods

### NewViewYourNumbersDataAllOfDataInnerStatus

`func NewViewYourNumbersDataAllOfDataInnerStatus() *ViewYourNumbersDataAllOfDataInnerStatus`

NewViewYourNumbersDataAllOfDataInnerStatus instantiates a new ViewYourNumbersDataAllOfDataInnerStatus object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewViewYourNumbersDataAllOfDataInnerStatusWithDefaults

`func NewViewYourNumbersDataAllOfDataInnerStatusWithDefaults() *ViewYourNumbersDataAllOfDataInnerStatus`

NewViewYourNumbersDataAllOfDataInnerStatusWithDefaults instantiates a new ViewYourNumbersDataAllOfDataInnerStatus object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetValue

`func (o *ViewYourNumbersDataAllOfDataInnerStatus) GetValue() int32`

GetValue returns the Value field if non-nil, zero value otherwise.

### GetValueOk

`func (o *ViewYourNumbersDataAllOfDataInnerStatus) GetValueOk() (*int32, bool)`

GetValueOk returns a tuple with the Value field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetValue

`func (o *ViewYourNumbersDataAllOfDataInnerStatus) SetValue(v int32)`

SetValue sets Value field to given value.

### HasValue

`func (o *ViewYourNumbersDataAllOfDataInnerStatus) HasValue() bool`

HasValue returns a boolean if a field has been set.

### GetLabel

`func (o *ViewYourNumbersDataAllOfDataInnerStatus) GetLabel() string`

GetLabel returns the Label field if non-nil, zero value otherwise.

### GetLabelOk

`func (o *ViewYourNumbersDataAllOfDataInnerStatus) GetLabelOk() (*string, bool)`

GetLabelOk returns a tuple with the Label field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetLabel

`func (o *ViewYourNumbersDataAllOfDataInnerStatus) SetLabel(v string)`

SetLabel sets Label field to given value.

### HasLabel

`func (o *ViewYourNumbersDataAllOfDataInnerStatus) HasLabel() bool`

HasLabel returns a boolean if a field has been set.

### GetDescription

`func (o *ViewYourNumbersDataAllOfDataInnerStatus) GetDescription() string`

GetDescription returns the Description field if non-nil, zero value otherwise.

### GetDescriptionOk

`func (o *ViewYourNumbersDataAllOfDataInnerStatus) GetDescriptionOk() (*string, bool)`

GetDescriptionOk returns a tuple with the Description field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDescription

`func (o *ViewYourNumbersDataAllOfDataInnerStatus) SetDescription(v string)`

SetDescription sets Description field to given value.

### HasDescription

`func (o *ViewYourNumbersDataAllOfDataInnerStatus) HasDescription() bool`

HasDescription returns a boolean if a field has been set.

### GetName

`func (o *ViewYourNumbersDataAllOfDataInnerStatus) GetName() string`

GetName returns the Name field if non-nil, zero value otherwise.

### GetNameOk

`func (o *ViewYourNumbersDataAllOfDataInnerStatus) GetNameOk() (*string, bool)`

GetNameOk returns a tuple with the Name field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetName

`func (o *ViewYourNumbersDataAllOfDataInnerStatus) SetName(v string)`

SetName sets Name field to given value.

### HasName

`func (o *ViewYourNumbersDataAllOfDataInnerStatus) HasName() bool`

HasName returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


