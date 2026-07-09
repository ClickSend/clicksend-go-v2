# UpdateDefaultSenderRequest

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**DefaultSenderStrategies** | [**[]CreateDefaultSenderRequestDefaultSenderStrategiesInner**](CreateDefaultSenderRequestDefaultSenderStrategiesInner.md) | Array detailing sender strategies. Must contain exactly 1 element. Multiple strategies support coming soon. | 

## Methods

### NewUpdateDefaultSenderRequest

`func NewUpdateDefaultSenderRequest(defaultSenderStrategies []CreateDefaultSenderRequestDefaultSenderStrategiesInner, ) *UpdateDefaultSenderRequest`

NewUpdateDefaultSenderRequest instantiates a new UpdateDefaultSenderRequest object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewUpdateDefaultSenderRequestWithDefaults

`func NewUpdateDefaultSenderRequestWithDefaults() *UpdateDefaultSenderRequest`

NewUpdateDefaultSenderRequestWithDefaults instantiates a new UpdateDefaultSenderRequest object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetDefaultSenderStrategies

`func (o *UpdateDefaultSenderRequest) GetDefaultSenderStrategies() []CreateDefaultSenderRequestDefaultSenderStrategiesInner`

GetDefaultSenderStrategies returns the DefaultSenderStrategies field if non-nil, zero value otherwise.

### GetDefaultSenderStrategiesOk

`func (o *UpdateDefaultSenderRequest) GetDefaultSenderStrategiesOk() (*[]CreateDefaultSenderRequestDefaultSenderStrategiesInner, bool)`

GetDefaultSenderStrategiesOk returns a tuple with the DefaultSenderStrategies field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDefaultSenderStrategies

`func (o *UpdateDefaultSenderRequest) SetDefaultSenderStrategies(v []CreateDefaultSenderRequestDefaultSenderStrategiesInner)`

SetDefaultSenderStrategies sets DefaultSenderStrategies field to given value.



[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


