# DefaultSenderDefaultSenderStrategiesInner

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**SenderType** | **string** | Type of the sender. | 
**SenderId** | **string** | Identifier for the sender. Must be between 3-20 characters. | 
**SenderCountryCode** | Pointer to **string** | ISO 3166-1 alpha-2 formatted country code. | [optional] 
**Priority** | **int32** | Priority level of the sender in the strategy. Must be a positive integer. | 
**Status** | **string** | Status of the sender in the strategy. | 
**Note** | Pointer to **string** | Note providing additional context about the sender. Maximum length of 200 characters. Optional. | [optional] 

## Methods

### NewDefaultSenderDefaultSenderStrategiesInner

`func NewDefaultSenderDefaultSenderStrategiesInner(senderType string, senderId string, priority int32, status string, ) *DefaultSenderDefaultSenderStrategiesInner`

NewDefaultSenderDefaultSenderStrategiesInner instantiates a new DefaultSenderDefaultSenderStrategiesInner object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewDefaultSenderDefaultSenderStrategiesInnerWithDefaults

`func NewDefaultSenderDefaultSenderStrategiesInnerWithDefaults() *DefaultSenderDefaultSenderStrategiesInner`

NewDefaultSenderDefaultSenderStrategiesInnerWithDefaults instantiates a new DefaultSenderDefaultSenderStrategiesInner object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetSenderType

`func (o *DefaultSenderDefaultSenderStrategiesInner) GetSenderType() string`

GetSenderType returns the SenderType field if non-nil, zero value otherwise.

### GetSenderTypeOk

`func (o *DefaultSenderDefaultSenderStrategiesInner) GetSenderTypeOk() (*string, bool)`

GetSenderTypeOk returns a tuple with the SenderType field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSenderType

`func (o *DefaultSenderDefaultSenderStrategiesInner) SetSenderType(v string)`

SetSenderType sets SenderType field to given value.


### GetSenderId

`func (o *DefaultSenderDefaultSenderStrategiesInner) GetSenderId() string`

GetSenderId returns the SenderId field if non-nil, zero value otherwise.

### GetSenderIdOk

`func (o *DefaultSenderDefaultSenderStrategiesInner) GetSenderIdOk() (*string, bool)`

GetSenderIdOk returns a tuple with the SenderId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSenderId

`func (o *DefaultSenderDefaultSenderStrategiesInner) SetSenderId(v string)`

SetSenderId sets SenderId field to given value.


### GetSenderCountryCode

`func (o *DefaultSenderDefaultSenderStrategiesInner) GetSenderCountryCode() string`

GetSenderCountryCode returns the SenderCountryCode field if non-nil, zero value otherwise.

### GetSenderCountryCodeOk

`func (o *DefaultSenderDefaultSenderStrategiesInner) GetSenderCountryCodeOk() (*string, bool)`

GetSenderCountryCodeOk returns a tuple with the SenderCountryCode field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSenderCountryCode

`func (o *DefaultSenderDefaultSenderStrategiesInner) SetSenderCountryCode(v string)`

SetSenderCountryCode sets SenderCountryCode field to given value.

### HasSenderCountryCode

`func (o *DefaultSenderDefaultSenderStrategiesInner) HasSenderCountryCode() bool`

HasSenderCountryCode returns a boolean if a field has been set.

### GetPriority

`func (o *DefaultSenderDefaultSenderStrategiesInner) GetPriority() int32`

GetPriority returns the Priority field if non-nil, zero value otherwise.

### GetPriorityOk

`func (o *DefaultSenderDefaultSenderStrategiesInner) GetPriorityOk() (*int32, bool)`

GetPriorityOk returns a tuple with the Priority field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetPriority

`func (o *DefaultSenderDefaultSenderStrategiesInner) SetPriority(v int32)`

SetPriority sets Priority field to given value.


### GetStatus

`func (o *DefaultSenderDefaultSenderStrategiesInner) GetStatus() string`

GetStatus returns the Status field if non-nil, zero value otherwise.

### GetStatusOk

`func (o *DefaultSenderDefaultSenderStrategiesInner) GetStatusOk() (*string, bool)`

GetStatusOk returns a tuple with the Status field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetStatus

`func (o *DefaultSenderDefaultSenderStrategiesInner) SetStatus(v string)`

SetStatus sets Status field to given value.


### GetNote

`func (o *DefaultSenderDefaultSenderStrategiesInner) GetNote() string`

GetNote returns the Note field if non-nil, zero value otherwise.

### GetNoteOk

`func (o *DefaultSenderDefaultSenderStrategiesInner) GetNoteOk() (*string, bool)`

GetNoteOk returns a tuple with the Note field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetNote

`func (o *DefaultSenderDefaultSenderStrategiesInner) SetNote(v string)`

SetNote sets Note field to given value.

### HasNote

`func (o *DefaultSenderDefaultSenderStrategiesInner) HasNote() bool`

HasNote returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


