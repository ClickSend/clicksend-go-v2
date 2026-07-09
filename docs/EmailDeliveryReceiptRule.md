# EmailDeliveryReceiptRule

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**ReceiptRuleId** | Pointer to **int32** | The ID of the receipt rule. | [optional] 
**RuleName** | Pointer to **string** | The name of the receipt rule. | [optional] 
**MatchType** | Pointer to **int32** | The type of match for the rule. | [optional] 
**Action** | Pointer to **string** | The action to be taken by the rule. | [optional] 
**ActionAddress** | Pointer to **string** | The address associated with the action. | [optional] 
**Enabled** | Pointer to **int32** | Indicates whether the rule is enabled. | [optional] 

## Methods

### NewEmailDeliveryReceiptRule

`func NewEmailDeliveryReceiptRule() *EmailDeliveryReceiptRule`

NewEmailDeliveryReceiptRule instantiates a new EmailDeliveryReceiptRule object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewEmailDeliveryReceiptRuleWithDefaults

`func NewEmailDeliveryReceiptRuleWithDefaults() *EmailDeliveryReceiptRule`

NewEmailDeliveryReceiptRuleWithDefaults instantiates a new EmailDeliveryReceiptRule object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetReceiptRuleId

`func (o *EmailDeliveryReceiptRule) GetReceiptRuleId() int32`

GetReceiptRuleId returns the ReceiptRuleId field if non-nil, zero value otherwise.

### GetReceiptRuleIdOk

`func (o *EmailDeliveryReceiptRule) GetReceiptRuleIdOk() (*int32, bool)`

GetReceiptRuleIdOk returns a tuple with the ReceiptRuleId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetReceiptRuleId

`func (o *EmailDeliveryReceiptRule) SetReceiptRuleId(v int32)`

SetReceiptRuleId sets ReceiptRuleId field to given value.

### HasReceiptRuleId

`func (o *EmailDeliveryReceiptRule) HasReceiptRuleId() bool`

HasReceiptRuleId returns a boolean if a field has been set.

### GetRuleName

`func (o *EmailDeliveryReceiptRule) GetRuleName() string`

GetRuleName returns the RuleName field if non-nil, zero value otherwise.

### GetRuleNameOk

`func (o *EmailDeliveryReceiptRule) GetRuleNameOk() (*string, bool)`

GetRuleNameOk returns a tuple with the RuleName field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetRuleName

`func (o *EmailDeliveryReceiptRule) SetRuleName(v string)`

SetRuleName sets RuleName field to given value.

### HasRuleName

`func (o *EmailDeliveryReceiptRule) HasRuleName() bool`

HasRuleName returns a boolean if a field has been set.

### GetMatchType

`func (o *EmailDeliveryReceiptRule) GetMatchType() int32`

GetMatchType returns the MatchType field if non-nil, zero value otherwise.

### GetMatchTypeOk

`func (o *EmailDeliveryReceiptRule) GetMatchTypeOk() (*int32, bool)`

GetMatchTypeOk returns a tuple with the MatchType field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetMatchType

`func (o *EmailDeliveryReceiptRule) SetMatchType(v int32)`

SetMatchType sets MatchType field to given value.

### HasMatchType

`func (o *EmailDeliveryReceiptRule) HasMatchType() bool`

HasMatchType returns a boolean if a field has been set.

### GetAction

`func (o *EmailDeliveryReceiptRule) GetAction() string`

GetAction returns the Action field if non-nil, zero value otherwise.

### GetActionOk

`func (o *EmailDeliveryReceiptRule) GetActionOk() (*string, bool)`

GetActionOk returns a tuple with the Action field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAction

`func (o *EmailDeliveryReceiptRule) SetAction(v string)`

SetAction sets Action field to given value.

### HasAction

`func (o *EmailDeliveryReceiptRule) HasAction() bool`

HasAction returns a boolean if a field has been set.

### GetActionAddress

`func (o *EmailDeliveryReceiptRule) GetActionAddress() string`

GetActionAddress returns the ActionAddress field if non-nil, zero value otherwise.

### GetActionAddressOk

`func (o *EmailDeliveryReceiptRule) GetActionAddressOk() (*string, bool)`

GetActionAddressOk returns a tuple with the ActionAddress field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetActionAddress

`func (o *EmailDeliveryReceiptRule) SetActionAddress(v string)`

SetActionAddress sets ActionAddress field to given value.

### HasActionAddress

`func (o *EmailDeliveryReceiptRule) HasActionAddress() bool`

HasActionAddress returns a boolean if a field has been set.

### GetEnabled

`func (o *EmailDeliveryReceiptRule) GetEnabled() int32`

GetEnabled returns the Enabled field if non-nil, zero value otherwise.

### GetEnabledOk

`func (o *EmailDeliveryReceiptRule) GetEnabledOk() (*int32, bool)`

GetEnabledOk returns a tuple with the Enabled field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetEnabled

`func (o *EmailDeliveryReceiptRule) SetEnabled(v int32)`

SetEnabled sets Enabled field to given value.

### HasEnabled

`func (o *EmailDeliveryReceiptRule) HasEnabled() bool`

HasEnabled returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


