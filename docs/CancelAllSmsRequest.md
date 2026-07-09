# CancelAllSmsRequest

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**CustomString** | Pointer to **string** | The scheduled messages to cancel with the specified _custom_string_. When you send an SMS, you can add an optional _custom_string_ to it. This parameter allows you to cancel messages that have this _custom_string_.  It&#39;s commonly used for canceling scheduled [SMS campaigns](/messaging/sms-campaigns/). When you send an SMS campaign, the system automatically adds a _custom_string_ to each message, and this parameter lets you cancel only those specific messages. | [optional] 

## Methods

### NewCancelAllSmsRequest

`func NewCancelAllSmsRequest() *CancelAllSmsRequest`

NewCancelAllSmsRequest instantiates a new CancelAllSmsRequest object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewCancelAllSmsRequestWithDefaults

`func NewCancelAllSmsRequestWithDefaults() *CancelAllSmsRequest`

NewCancelAllSmsRequestWithDefaults instantiates a new CancelAllSmsRequest object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetCustomString

`func (o *CancelAllSmsRequest) GetCustomString() string`

GetCustomString returns the CustomString field if non-nil, zero value otherwise.

### GetCustomStringOk

`func (o *CancelAllSmsRequest) GetCustomStringOk() (*string, bool)`

GetCustomStringOk returns a tuple with the CustomString field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCustomString

`func (o *CancelAllSmsRequest) SetCustomString(v string)`

SetCustomString sets CustomString field to given value.

### HasCustomString

`func (o *CancelAllSmsRequest) HasCustomString() bool`

HasCustomString returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


