# SmsInboundRule

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**InboundRuleId** | Pointer to **int32** | The ID of the inbound rule. | [optional] 
**DedicatedNumber** | Pointer to **string** | The number to be used in the inbound rule. | [optional] 
**RuleName** | Pointer to **string** | The name of the inbound rule. | [optional] 
**MessageSearchType** | Pointer to **int32** | The type of message search to be used in the inbound rule. | [optional] 
**MessageSearchTerm** | Pointer to **string** | The message search term to be used in the inbound rule. | [optional] 
**Action** | Pointer to **string** | The action to be taken in the inbound rule. | [optional] 
**ActionAddress** | Pointer to **string** | The action address to be used in the inbound rule. | [optional] 
**Body** | Pointer to **NullableString** | The body of the inbound rule. | [optional] 
**Enabled** | Pointer to **int32** | The status of the inbound rule. | [optional] 
**WebhookType** | Pointer to **NullableString** | The format used when calling the webhook (e.g. post, json). | [optional] 

## Methods

### NewSmsInboundRule

`func NewSmsInboundRule() *SmsInboundRule`

NewSmsInboundRule instantiates a new SmsInboundRule object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewSmsInboundRuleWithDefaults

`func NewSmsInboundRuleWithDefaults() *SmsInboundRule`

NewSmsInboundRuleWithDefaults instantiates a new SmsInboundRule object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetInboundRuleId

`func (o *SmsInboundRule) GetInboundRuleId() int32`

GetInboundRuleId returns the InboundRuleId field if non-nil, zero value otherwise.

### GetInboundRuleIdOk

`func (o *SmsInboundRule) GetInboundRuleIdOk() (*int32, bool)`

GetInboundRuleIdOk returns a tuple with the InboundRuleId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetInboundRuleId

`func (o *SmsInboundRule) SetInboundRuleId(v int32)`

SetInboundRuleId sets InboundRuleId field to given value.

### HasInboundRuleId

`func (o *SmsInboundRule) HasInboundRuleId() bool`

HasInboundRuleId returns a boolean if a field has been set.

### GetDedicatedNumber

`func (o *SmsInboundRule) GetDedicatedNumber() string`

GetDedicatedNumber returns the DedicatedNumber field if non-nil, zero value otherwise.

### GetDedicatedNumberOk

`func (o *SmsInboundRule) GetDedicatedNumberOk() (*string, bool)`

GetDedicatedNumberOk returns a tuple with the DedicatedNumber field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDedicatedNumber

`func (o *SmsInboundRule) SetDedicatedNumber(v string)`

SetDedicatedNumber sets DedicatedNumber field to given value.

### HasDedicatedNumber

`func (o *SmsInboundRule) HasDedicatedNumber() bool`

HasDedicatedNumber returns a boolean if a field has been set.

### GetRuleName

`func (o *SmsInboundRule) GetRuleName() string`

GetRuleName returns the RuleName field if non-nil, zero value otherwise.

### GetRuleNameOk

`func (o *SmsInboundRule) GetRuleNameOk() (*string, bool)`

GetRuleNameOk returns a tuple with the RuleName field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetRuleName

`func (o *SmsInboundRule) SetRuleName(v string)`

SetRuleName sets RuleName field to given value.

### HasRuleName

`func (o *SmsInboundRule) HasRuleName() bool`

HasRuleName returns a boolean if a field has been set.

### GetMessageSearchType

`func (o *SmsInboundRule) GetMessageSearchType() int32`

GetMessageSearchType returns the MessageSearchType field if non-nil, zero value otherwise.

### GetMessageSearchTypeOk

`func (o *SmsInboundRule) GetMessageSearchTypeOk() (*int32, bool)`

GetMessageSearchTypeOk returns a tuple with the MessageSearchType field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetMessageSearchType

`func (o *SmsInboundRule) SetMessageSearchType(v int32)`

SetMessageSearchType sets MessageSearchType field to given value.

### HasMessageSearchType

`func (o *SmsInboundRule) HasMessageSearchType() bool`

HasMessageSearchType returns a boolean if a field has been set.

### GetMessageSearchTerm

`func (o *SmsInboundRule) GetMessageSearchTerm() string`

GetMessageSearchTerm returns the MessageSearchTerm field if non-nil, zero value otherwise.

### GetMessageSearchTermOk

`func (o *SmsInboundRule) GetMessageSearchTermOk() (*string, bool)`

GetMessageSearchTermOk returns a tuple with the MessageSearchTerm field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetMessageSearchTerm

`func (o *SmsInboundRule) SetMessageSearchTerm(v string)`

SetMessageSearchTerm sets MessageSearchTerm field to given value.

### HasMessageSearchTerm

`func (o *SmsInboundRule) HasMessageSearchTerm() bool`

HasMessageSearchTerm returns a boolean if a field has been set.

### GetAction

`func (o *SmsInboundRule) GetAction() string`

GetAction returns the Action field if non-nil, zero value otherwise.

### GetActionOk

`func (o *SmsInboundRule) GetActionOk() (*string, bool)`

GetActionOk returns a tuple with the Action field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAction

`func (o *SmsInboundRule) SetAction(v string)`

SetAction sets Action field to given value.

### HasAction

`func (o *SmsInboundRule) HasAction() bool`

HasAction returns a boolean if a field has been set.

### GetActionAddress

`func (o *SmsInboundRule) GetActionAddress() string`

GetActionAddress returns the ActionAddress field if non-nil, zero value otherwise.

### GetActionAddressOk

`func (o *SmsInboundRule) GetActionAddressOk() (*string, bool)`

GetActionAddressOk returns a tuple with the ActionAddress field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetActionAddress

`func (o *SmsInboundRule) SetActionAddress(v string)`

SetActionAddress sets ActionAddress field to given value.

### HasActionAddress

`func (o *SmsInboundRule) HasActionAddress() bool`

HasActionAddress returns a boolean if a field has been set.

### GetBody

`func (o *SmsInboundRule) GetBody() string`

GetBody returns the Body field if non-nil, zero value otherwise.

### GetBodyOk

`func (o *SmsInboundRule) GetBodyOk() (*string, bool)`

GetBodyOk returns a tuple with the Body field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetBody

`func (o *SmsInboundRule) SetBody(v string)`

SetBody sets Body field to given value.

### HasBody

`func (o *SmsInboundRule) HasBody() bool`

HasBody returns a boolean if a field has been set.

### SetBodyNil

`func (o *SmsInboundRule) SetBodyNil(b bool)`

 SetBodyNil sets the value for Body to be an explicit nil

### UnsetBody
`func (o *SmsInboundRule) UnsetBody()`

UnsetBody ensures that no value is present for Body, not even an explicit nil
### GetEnabled

`func (o *SmsInboundRule) GetEnabled() int32`

GetEnabled returns the Enabled field if non-nil, zero value otherwise.

### GetEnabledOk

`func (o *SmsInboundRule) GetEnabledOk() (*int32, bool)`

GetEnabledOk returns a tuple with the Enabled field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetEnabled

`func (o *SmsInboundRule) SetEnabled(v int32)`

SetEnabled sets Enabled field to given value.

### HasEnabled

`func (o *SmsInboundRule) HasEnabled() bool`

HasEnabled returns a boolean if a field has been set.

### GetWebhookType

`func (o *SmsInboundRule) GetWebhookType() string`

GetWebhookType returns the WebhookType field if non-nil, zero value otherwise.

### GetWebhookTypeOk

`func (o *SmsInboundRule) GetWebhookTypeOk() (*string, bool)`

GetWebhookTypeOk returns a tuple with the WebhookType field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetWebhookType

`func (o *SmsInboundRule) SetWebhookType(v string)`

SetWebhookType sets WebhookType field to given value.

### HasWebhookType

`func (o *SmsInboundRule) HasWebhookType() bool`

HasWebhookType returns a boolean if a field has been set.

### SetWebhookTypeNil

`func (o *SmsInboundRule) SetWebhookTypeNil(b bool)`

 SetWebhookTypeNil sets the value for WebhookType to be an explicit nil

### UnsetWebhookType
`func (o *SmsInboundRule) UnsetWebhookType()`

UnsetWebhookType ensures that no value is present for WebhookType, not even an explicit nil

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


