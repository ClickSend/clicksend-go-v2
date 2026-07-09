# CreateFaxInboundRuleRequest

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**DedicatedNumber** | Pointer to **string** |  | [optional] 
**RuleName** | Pointer to **string** |  | [optional] 
**Action** | Pointer to **string** |  | [optional] 
**ActionAddress** | Pointer to **string** |  | [optional] 
**Enabled** | Pointer to **int32** |  | [optional] 

## Methods

### NewCreateFaxInboundRuleRequest

`func NewCreateFaxInboundRuleRequest() *CreateFaxInboundRuleRequest`

NewCreateFaxInboundRuleRequest instantiates a new CreateFaxInboundRuleRequest object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewCreateFaxInboundRuleRequestWithDefaults

`func NewCreateFaxInboundRuleRequestWithDefaults() *CreateFaxInboundRuleRequest`

NewCreateFaxInboundRuleRequestWithDefaults instantiates a new CreateFaxInboundRuleRequest object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetDedicatedNumber

`func (o *CreateFaxInboundRuleRequest) GetDedicatedNumber() string`

GetDedicatedNumber returns the DedicatedNumber field if non-nil, zero value otherwise.

### GetDedicatedNumberOk

`func (o *CreateFaxInboundRuleRequest) GetDedicatedNumberOk() (*string, bool)`

GetDedicatedNumberOk returns a tuple with the DedicatedNumber field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDedicatedNumber

`func (o *CreateFaxInboundRuleRequest) SetDedicatedNumber(v string)`

SetDedicatedNumber sets DedicatedNumber field to given value.

### HasDedicatedNumber

`func (o *CreateFaxInboundRuleRequest) HasDedicatedNumber() bool`

HasDedicatedNumber returns a boolean if a field has been set.

### GetRuleName

`func (o *CreateFaxInboundRuleRequest) GetRuleName() string`

GetRuleName returns the RuleName field if non-nil, zero value otherwise.

### GetRuleNameOk

`func (o *CreateFaxInboundRuleRequest) GetRuleNameOk() (*string, bool)`

GetRuleNameOk returns a tuple with the RuleName field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetRuleName

`func (o *CreateFaxInboundRuleRequest) SetRuleName(v string)`

SetRuleName sets RuleName field to given value.

### HasRuleName

`func (o *CreateFaxInboundRuleRequest) HasRuleName() bool`

HasRuleName returns a boolean if a field has been set.

### GetAction

`func (o *CreateFaxInboundRuleRequest) GetAction() string`

GetAction returns the Action field if non-nil, zero value otherwise.

### GetActionOk

`func (o *CreateFaxInboundRuleRequest) GetActionOk() (*string, bool)`

GetActionOk returns a tuple with the Action field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAction

`func (o *CreateFaxInboundRuleRequest) SetAction(v string)`

SetAction sets Action field to given value.

### HasAction

`func (o *CreateFaxInboundRuleRequest) HasAction() bool`

HasAction returns a boolean if a field has been set.

### GetActionAddress

`func (o *CreateFaxInboundRuleRequest) GetActionAddress() string`

GetActionAddress returns the ActionAddress field if non-nil, zero value otherwise.

### GetActionAddressOk

`func (o *CreateFaxInboundRuleRequest) GetActionAddressOk() (*string, bool)`

GetActionAddressOk returns a tuple with the ActionAddress field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetActionAddress

`func (o *CreateFaxInboundRuleRequest) SetActionAddress(v string)`

SetActionAddress sets ActionAddress field to given value.

### HasActionAddress

`func (o *CreateFaxInboundRuleRequest) HasActionAddress() bool`

HasActionAddress returns a boolean if a field has been set.

### GetEnabled

`func (o *CreateFaxInboundRuleRequest) GetEnabled() int32`

GetEnabled returns the Enabled field if non-nil, zero value otherwise.

### GetEnabledOk

`func (o *CreateFaxInboundRuleRequest) GetEnabledOk() (*int32, bool)`

GetEnabledOk returns a tuple with the Enabled field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetEnabled

`func (o *CreateFaxInboundRuleRequest) SetEnabled(v int32)`

SetEnabled sets Enabled field to given value.

### HasEnabled

`func (o *CreateFaxInboundRuleRequest) HasEnabled() bool`

HasEnabled returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


