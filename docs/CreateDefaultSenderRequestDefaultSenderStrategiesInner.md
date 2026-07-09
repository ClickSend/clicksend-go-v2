# CreateDefaultSenderRequestDefaultSenderStrategiesInner

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**SenderType** | **string** | The type of sender for this strategy. | 
**SenderId** | **string** | Unique identifier for the sender. Format varies based on &#x60;sender_type&#x60;: - &#x60;shortcode&#x60;: Numeric, 3-8 digits. - &#x60;longcode&#x60;, &#x60;tollfree&#x60;, &#x60;10DLC&#x60;, &#x60;own_number&#x60;: 2-15 digits, may include &#x60;+&#x60; prefix. - &#x60;alpha_tag&#x60;: 3-11 alphanumeric characters, must include at least one letter or &#x60;+&#x60;. - &#x60;shared_longcode&#x60;: Can be null or empty string.  &gt; **Important:** The &#x60;sender_id&#x60; must be in valid format, owned, and has ready to use status for the corresponding &#x60;sender_type&#x60;.  | 
**SenderCountryCode** | Pointer to **string** | The country code of the sender, using the ISO 3166-1 alpha-2 format (e.g., \&quot;US\&quot;).  This field is required in the following cases: - When &#x60;sender_type&#x60; is &#x60;own_number&#x60;, &#x60;longcode&#x60;, &#x60;tollfree&#x60;, or &#x60;10DLC&#x60; - When the &#x60;sender_id&#x60; follows the US/Canada number format (starts with &#x60;+1&#x60;)  For all other cases, this field is optional.  | [optional] 
**Note** | Pointer to **string** | Optional note providing additional context about the sender strategy. | [optional] 

## Methods

### NewCreateDefaultSenderRequestDefaultSenderStrategiesInner

`func NewCreateDefaultSenderRequestDefaultSenderStrategiesInner(senderType string, senderId string, ) *CreateDefaultSenderRequestDefaultSenderStrategiesInner`

NewCreateDefaultSenderRequestDefaultSenderStrategiesInner instantiates a new CreateDefaultSenderRequestDefaultSenderStrategiesInner object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewCreateDefaultSenderRequestDefaultSenderStrategiesInnerWithDefaults

`func NewCreateDefaultSenderRequestDefaultSenderStrategiesInnerWithDefaults() *CreateDefaultSenderRequestDefaultSenderStrategiesInner`

NewCreateDefaultSenderRequestDefaultSenderStrategiesInnerWithDefaults instantiates a new CreateDefaultSenderRequestDefaultSenderStrategiesInner object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetSenderType

`func (o *CreateDefaultSenderRequestDefaultSenderStrategiesInner) GetSenderType() string`

GetSenderType returns the SenderType field if non-nil, zero value otherwise.

### GetSenderTypeOk

`func (o *CreateDefaultSenderRequestDefaultSenderStrategiesInner) GetSenderTypeOk() (*string, bool)`

GetSenderTypeOk returns a tuple with the SenderType field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSenderType

`func (o *CreateDefaultSenderRequestDefaultSenderStrategiesInner) SetSenderType(v string)`

SetSenderType sets SenderType field to given value.


### GetSenderId

`func (o *CreateDefaultSenderRequestDefaultSenderStrategiesInner) GetSenderId() string`

GetSenderId returns the SenderId field if non-nil, zero value otherwise.

### GetSenderIdOk

`func (o *CreateDefaultSenderRequestDefaultSenderStrategiesInner) GetSenderIdOk() (*string, bool)`

GetSenderIdOk returns a tuple with the SenderId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSenderId

`func (o *CreateDefaultSenderRequestDefaultSenderStrategiesInner) SetSenderId(v string)`

SetSenderId sets SenderId field to given value.


### GetSenderCountryCode

`func (o *CreateDefaultSenderRequestDefaultSenderStrategiesInner) GetSenderCountryCode() string`

GetSenderCountryCode returns the SenderCountryCode field if non-nil, zero value otherwise.

### GetSenderCountryCodeOk

`func (o *CreateDefaultSenderRequestDefaultSenderStrategiesInner) GetSenderCountryCodeOk() (*string, bool)`

GetSenderCountryCodeOk returns a tuple with the SenderCountryCode field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSenderCountryCode

`func (o *CreateDefaultSenderRequestDefaultSenderStrategiesInner) SetSenderCountryCode(v string)`

SetSenderCountryCode sets SenderCountryCode field to given value.

### HasSenderCountryCode

`func (o *CreateDefaultSenderRequestDefaultSenderStrategiesInner) HasSenderCountryCode() bool`

HasSenderCountryCode returns a boolean if a field has been set.

### GetNote

`func (o *CreateDefaultSenderRequestDefaultSenderStrategiesInner) GetNote() string`

GetNote returns the Note field if non-nil, zero value otherwise.

### GetNoteOk

`func (o *CreateDefaultSenderRequestDefaultSenderStrategiesInner) GetNoteOk() (*string, bool)`

GetNoteOk returns a tuple with the Note field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetNote

`func (o *CreateDefaultSenderRequestDefaultSenderStrategiesInner) SetNote(v string)`

SetNote sets Note field to given value.

### HasNote

`func (o *CreateDefaultSenderRequestDefaultSenderStrategiesInner) HasNote() bool`

HasNote returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


