# CreateSmsInboundAutomationRequest

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**DedicatedNumber** | Pointer to **string** |  | [optional] 
**RuleName** | Pointer to **string** |  | [optional] 
**MessageSearchType** | Pointer to **int32** |  | [optional] 
**MessageSearchTerm** | Pointer to **NullableString** |  | [optional] 
**Action** | Pointer to **string** |  | [optional] 
**ActionAddress** | Pointer to **string** |  | [optional] 
**Body** | Pointer to **NullableString** |  | [optional] 
**Enabled** | Pointer to **int32** |  | [optional] 

## Methods

### NewCreateSmsInboundAutomationRequest

`func NewCreateSmsInboundAutomationRequest() *CreateSmsInboundAutomationRequest`

NewCreateSmsInboundAutomationRequest instantiates a new CreateSmsInboundAutomationRequest object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewCreateSmsInboundAutomationRequestWithDefaults

`func NewCreateSmsInboundAutomationRequestWithDefaults() *CreateSmsInboundAutomationRequest`

NewCreateSmsInboundAutomationRequestWithDefaults instantiates a new CreateSmsInboundAutomationRequest object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetDedicatedNumber

`func (o *CreateSmsInboundAutomationRequest) GetDedicatedNumber() string`

GetDedicatedNumber returns the DedicatedNumber field if non-nil, zero value otherwise.

### GetDedicatedNumberOk

`func (o *CreateSmsInboundAutomationRequest) GetDedicatedNumberOk() (*string, bool)`

GetDedicatedNumberOk returns a tuple with the DedicatedNumber field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDedicatedNumber

`func (o *CreateSmsInboundAutomationRequest) SetDedicatedNumber(v string)`

SetDedicatedNumber sets DedicatedNumber field to given value.

### HasDedicatedNumber

`func (o *CreateSmsInboundAutomationRequest) HasDedicatedNumber() bool`

HasDedicatedNumber returns a boolean if a field has been set.

### GetRuleName

`func (o *CreateSmsInboundAutomationRequest) GetRuleName() string`

GetRuleName returns the RuleName field if non-nil, zero value otherwise.

### GetRuleNameOk

`func (o *CreateSmsInboundAutomationRequest) GetRuleNameOk() (*string, bool)`

GetRuleNameOk returns a tuple with the RuleName field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetRuleName

`func (o *CreateSmsInboundAutomationRequest) SetRuleName(v string)`

SetRuleName sets RuleName field to given value.

### HasRuleName

`func (o *CreateSmsInboundAutomationRequest) HasRuleName() bool`

HasRuleName returns a boolean if a field has been set.

### GetMessageSearchType

`func (o *CreateSmsInboundAutomationRequest) GetMessageSearchType() int32`

GetMessageSearchType returns the MessageSearchType field if non-nil, zero value otherwise.

### GetMessageSearchTypeOk

`func (o *CreateSmsInboundAutomationRequest) GetMessageSearchTypeOk() (*int32, bool)`

GetMessageSearchTypeOk returns a tuple with the MessageSearchType field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetMessageSearchType

`func (o *CreateSmsInboundAutomationRequest) SetMessageSearchType(v int32)`

SetMessageSearchType sets MessageSearchType field to given value.

### HasMessageSearchType

`func (o *CreateSmsInboundAutomationRequest) HasMessageSearchType() bool`

HasMessageSearchType returns a boolean if a field has been set.

### GetMessageSearchTerm

`func (o *CreateSmsInboundAutomationRequest) GetMessageSearchTerm() string`

GetMessageSearchTerm returns the MessageSearchTerm field if non-nil, zero value otherwise.

### GetMessageSearchTermOk

`func (o *CreateSmsInboundAutomationRequest) GetMessageSearchTermOk() (*string, bool)`

GetMessageSearchTermOk returns a tuple with the MessageSearchTerm field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetMessageSearchTerm

`func (o *CreateSmsInboundAutomationRequest) SetMessageSearchTerm(v string)`

SetMessageSearchTerm sets MessageSearchTerm field to given value.

### HasMessageSearchTerm

`func (o *CreateSmsInboundAutomationRequest) HasMessageSearchTerm() bool`

HasMessageSearchTerm returns a boolean if a field has been set.

### SetMessageSearchTermNil

`func (o *CreateSmsInboundAutomationRequest) SetMessageSearchTermNil(b bool)`

 SetMessageSearchTermNil sets the value for MessageSearchTerm to be an explicit nil

### UnsetMessageSearchTerm
`func (o *CreateSmsInboundAutomationRequest) UnsetMessageSearchTerm()`

UnsetMessageSearchTerm ensures that no value is present for MessageSearchTerm, not even an explicit nil
### GetAction

`func (o *CreateSmsInboundAutomationRequest) GetAction() string`

GetAction returns the Action field if non-nil, zero value otherwise.

### GetActionOk

`func (o *CreateSmsInboundAutomationRequest) GetActionOk() (*string, bool)`

GetActionOk returns a tuple with the Action field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAction

`func (o *CreateSmsInboundAutomationRequest) SetAction(v string)`

SetAction sets Action field to given value.

### HasAction

`func (o *CreateSmsInboundAutomationRequest) HasAction() bool`

HasAction returns a boolean if a field has been set.

### GetActionAddress

`func (o *CreateSmsInboundAutomationRequest) GetActionAddress() string`

GetActionAddress returns the ActionAddress field if non-nil, zero value otherwise.

### GetActionAddressOk

`func (o *CreateSmsInboundAutomationRequest) GetActionAddressOk() (*string, bool)`

GetActionAddressOk returns a tuple with the ActionAddress field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetActionAddress

`func (o *CreateSmsInboundAutomationRequest) SetActionAddress(v string)`

SetActionAddress sets ActionAddress field to given value.

### HasActionAddress

`func (o *CreateSmsInboundAutomationRequest) HasActionAddress() bool`

HasActionAddress returns a boolean if a field has been set.

### GetBody

`func (o *CreateSmsInboundAutomationRequest) GetBody() string`

GetBody returns the Body field if non-nil, zero value otherwise.

### GetBodyOk

`func (o *CreateSmsInboundAutomationRequest) GetBodyOk() (*string, bool)`

GetBodyOk returns a tuple with the Body field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetBody

`func (o *CreateSmsInboundAutomationRequest) SetBody(v string)`

SetBody sets Body field to given value.

### HasBody

`func (o *CreateSmsInboundAutomationRequest) HasBody() bool`

HasBody returns a boolean if a field has been set.

### SetBodyNil

`func (o *CreateSmsInboundAutomationRequest) SetBodyNil(b bool)`

 SetBodyNil sets the value for Body to be an explicit nil

### UnsetBody
`func (o *CreateSmsInboundAutomationRequest) UnsetBody()`

UnsetBody ensures that no value is present for Body, not even an explicit nil
### GetEnabled

`func (o *CreateSmsInboundAutomationRequest) GetEnabled() int32`

GetEnabled returns the Enabled field if non-nil, zero value otherwise.

### GetEnabledOk

`func (o *CreateSmsInboundAutomationRequest) GetEnabledOk() (*int32, bool)`

GetEnabledOk returns a tuple with the Enabled field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetEnabled

`func (o *CreateSmsInboundAutomationRequest) SetEnabled(v int32)`

SetEnabled sets Enabled field to given value.

### HasEnabled

`func (o *CreateSmsInboundAutomationRequest) HasEnabled() bool`

HasEnabled returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


