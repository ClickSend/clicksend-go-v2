# SendersInner

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**RecipientCountryCode** | **string** | Recipient ISO country code | 
**SenderId** | Pointer to **string** | The sender ID must be either an alpha tag or a phone number. It is a required field unless the sender type is a &#x60;shared_longcode&#x60;.   If the sender ID is an **alpha tag**, it must be between 3 and 11 characters long and contains only letters, numbers, and pluses.  | [optional] 
**SenderType** | Pointer to **string** | The type of sender ID, it only supports &#x60;shared_longcode&#x60; at the moment. | [optional] 
**SenderCountryCode** | Pointer to **string** | The ISO 3166-1 alpha-2 country code that identifies the country associated with the sender’s number in a shared pool. This is affected only when &#x60;sender_type&#x60; is set to &#x60;shared_longcode&#x60; to determine the appropriate number based on the sender’s geographic location. If this field is not provided or left empty, it will default to the recipient&#39;s country code.  | [optional] 

## Methods

### NewSendersInner

`func NewSendersInner(recipientCountryCode string, ) *SendersInner`

NewSendersInner instantiates a new SendersInner object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewSendersInnerWithDefaults

`func NewSendersInnerWithDefaults() *SendersInner`

NewSendersInnerWithDefaults instantiates a new SendersInner object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetRecipientCountryCode

`func (o *SendersInner) GetRecipientCountryCode() string`

GetRecipientCountryCode returns the RecipientCountryCode field if non-nil, zero value otherwise.

### GetRecipientCountryCodeOk

`func (o *SendersInner) GetRecipientCountryCodeOk() (*string, bool)`

GetRecipientCountryCodeOk returns a tuple with the RecipientCountryCode field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetRecipientCountryCode

`func (o *SendersInner) SetRecipientCountryCode(v string)`

SetRecipientCountryCode sets RecipientCountryCode field to given value.


### GetSenderId

`func (o *SendersInner) GetSenderId() string`

GetSenderId returns the SenderId field if non-nil, zero value otherwise.

### GetSenderIdOk

`func (o *SendersInner) GetSenderIdOk() (*string, bool)`

GetSenderIdOk returns a tuple with the SenderId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSenderId

`func (o *SendersInner) SetSenderId(v string)`

SetSenderId sets SenderId field to given value.

### HasSenderId

`func (o *SendersInner) HasSenderId() bool`

HasSenderId returns a boolean if a field has been set.

### GetSenderType

`func (o *SendersInner) GetSenderType() string`

GetSenderType returns the SenderType field if non-nil, zero value otherwise.

### GetSenderTypeOk

`func (o *SendersInner) GetSenderTypeOk() (*string, bool)`

GetSenderTypeOk returns a tuple with the SenderType field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSenderType

`func (o *SendersInner) SetSenderType(v string)`

SetSenderType sets SenderType field to given value.

### HasSenderType

`func (o *SendersInner) HasSenderType() bool`

HasSenderType returns a boolean if a field has been set.

### GetSenderCountryCode

`func (o *SendersInner) GetSenderCountryCode() string`

GetSenderCountryCode returns the SenderCountryCode field if non-nil, zero value otherwise.

### GetSenderCountryCodeOk

`func (o *SendersInner) GetSenderCountryCodeOk() (*string, bool)`

GetSenderCountryCodeOk returns a tuple with the SenderCountryCode field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSenderCountryCode

`func (o *SendersInner) SetSenderCountryCode(v string)`

SetSenderCountryCode sets SenderCountryCode field to given value.

### HasSenderCountryCode

`func (o *SendersInner) HasSenderCountryCode() bool`

HasSenderCountryCode returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


