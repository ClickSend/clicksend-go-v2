# SmsDeliveryReceiptRule

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**ReceiptRuleId** | Pointer to **int32** | The ID of the receipt rule. | [optional] 
**RuleName** | Pointer to **string** | The name of the receipt rule. | [optional] 
**MatchType** | Pointer to **int32** | The type of match. | [optional] 
**Action** | Pointer to **string** | The type of action. | [optional] 
**ActionAddress** | Pointer to **string** | The address associated with the action. | [optional] 
**Enabled** | Pointer to **int32** | Indicates whether the rule is enabled. | [optional] 

## Methods

### NewSmsDeliveryReceiptRule

`func NewSmsDeliveryReceiptRule() *SmsDeliveryReceiptRule`

NewSmsDeliveryReceiptRule instantiates a new SmsDeliveryReceiptRule object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewSmsDeliveryReceiptRuleWithDefaults

`func NewSmsDeliveryReceiptRuleWithDefaults() *SmsDeliveryReceiptRule`

NewSmsDeliveryReceiptRuleWithDefaults instantiates a new SmsDeliveryReceiptRule object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetReceiptRuleId

`func (o *SmsDeliveryReceiptRule) GetReceiptRuleId() int32`

GetReceiptRuleId returns the ReceiptRuleId field if non-nil, zero value otherwise.

### GetReceiptRuleIdOk

`func (o *SmsDeliveryReceiptRule) GetReceiptRuleIdOk() (*int32, bool)`

GetReceiptRuleIdOk returns a tuple with the ReceiptRuleId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetReceiptRuleId

`func (o *SmsDeliveryReceiptRule) SetReceiptRuleId(v int32)`

SetReceiptRuleId sets ReceiptRuleId field to given value.

### HasReceiptRuleId

`func (o *SmsDeliveryReceiptRule) HasReceiptRuleId() bool`

HasReceiptRuleId returns a boolean if a field has been set.

### GetRuleName

`func (o *SmsDeliveryReceiptRule) GetRuleName() string`

GetRuleName returns the RuleName field if non-nil, zero value otherwise.

### GetRuleNameOk

`func (o *SmsDeliveryReceiptRule) GetRuleNameOk() (*string, bool)`

GetRuleNameOk returns a tuple with the RuleName field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetRuleName

`func (o *SmsDeliveryReceiptRule) SetRuleName(v string)`

SetRuleName sets RuleName field to given value.

### HasRuleName

`func (o *SmsDeliveryReceiptRule) HasRuleName() bool`

HasRuleName returns a boolean if a field has been set.

### GetMatchType

`func (o *SmsDeliveryReceiptRule) GetMatchType() int32`

GetMatchType returns the MatchType field if non-nil, zero value otherwise.

### GetMatchTypeOk

`func (o *SmsDeliveryReceiptRule) GetMatchTypeOk() (*int32, bool)`

GetMatchTypeOk returns a tuple with the MatchType field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetMatchType

`func (o *SmsDeliveryReceiptRule) SetMatchType(v int32)`

SetMatchType sets MatchType field to given value.

### HasMatchType

`func (o *SmsDeliveryReceiptRule) HasMatchType() bool`

HasMatchType returns a boolean if a field has been set.

### GetAction

`func (o *SmsDeliveryReceiptRule) GetAction() string`

GetAction returns the Action field if non-nil, zero value otherwise.

### GetActionOk

`func (o *SmsDeliveryReceiptRule) GetActionOk() (*string, bool)`

GetActionOk returns a tuple with the Action field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAction

`func (o *SmsDeliveryReceiptRule) SetAction(v string)`

SetAction sets Action field to given value.

### HasAction

`func (o *SmsDeliveryReceiptRule) HasAction() bool`

HasAction returns a boolean if a field has been set.

### GetActionAddress

`func (o *SmsDeliveryReceiptRule) GetActionAddress() string`

GetActionAddress returns the ActionAddress field if non-nil, zero value otherwise.

### GetActionAddressOk

`func (o *SmsDeliveryReceiptRule) GetActionAddressOk() (*string, bool)`

GetActionAddressOk returns a tuple with the ActionAddress field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetActionAddress

`func (o *SmsDeliveryReceiptRule) SetActionAddress(v string)`

SetActionAddress sets ActionAddress field to given value.

### HasActionAddress

`func (o *SmsDeliveryReceiptRule) HasActionAddress() bool`

HasActionAddress returns a boolean if a field has been set.

### GetEnabled

`func (o *SmsDeliveryReceiptRule) GetEnabled() int32`

GetEnabled returns the Enabled field if non-nil, zero value otherwise.

### GetEnabledOk

`func (o *SmsDeliveryReceiptRule) GetEnabledOk() (*int32, bool)`

GetEnabledOk returns a tuple with the Enabled field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetEnabled

`func (o *SmsDeliveryReceiptRule) SetEnabled(v int32)`

SetEnabled sets Enabled field to given value.

### HasEnabled

`func (o *SmsDeliveryReceiptRule) HasEnabled() bool`

HasEnabled returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


