# SmsCampaignSendersInner

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**RecipientCountryCode** | Pointer to **string** | Recipient ISO country code | [optional] 
**SenderId** | Pointer to **string** | The sender ID you specified in the request. This parameter would not be returned if you did specify it in the SMS campaign. | [optional] 
**SenderType** | Pointer to **string** | The type of sender ID you specified in the request. This parameter would not be returned if you did specify it in the SMS campaign. | [optional] 
**SenderCountryCode** | Pointer to **string** | The country code of the sender you specified in the request. It is in two-letter format (e.g. US, UK, AU, NZ, &lt;a href&#x3D;\&quot;https://help.clicksend.com/article/7wtbhhy6sy-country-code-calling-code-list\&quot; target&#x3D;\&quot;_blank\&quot;&gt;etc&lt;/a&gt;).  For certain countries, you can receive SMS from abroad. This parameter would not be returned if you did specify it in the SMS campaign. | [optional] 

## Methods

### NewSmsCampaignSendersInner

`func NewSmsCampaignSendersInner() *SmsCampaignSendersInner`

NewSmsCampaignSendersInner instantiates a new SmsCampaignSendersInner object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewSmsCampaignSendersInnerWithDefaults

`func NewSmsCampaignSendersInnerWithDefaults() *SmsCampaignSendersInner`

NewSmsCampaignSendersInnerWithDefaults instantiates a new SmsCampaignSendersInner object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetRecipientCountryCode

`func (o *SmsCampaignSendersInner) GetRecipientCountryCode() string`

GetRecipientCountryCode returns the RecipientCountryCode field if non-nil, zero value otherwise.

### GetRecipientCountryCodeOk

`func (o *SmsCampaignSendersInner) GetRecipientCountryCodeOk() (*string, bool)`

GetRecipientCountryCodeOk returns a tuple with the RecipientCountryCode field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetRecipientCountryCode

`func (o *SmsCampaignSendersInner) SetRecipientCountryCode(v string)`

SetRecipientCountryCode sets RecipientCountryCode field to given value.

### HasRecipientCountryCode

`func (o *SmsCampaignSendersInner) HasRecipientCountryCode() bool`

HasRecipientCountryCode returns a boolean if a field has been set.

### GetSenderId

`func (o *SmsCampaignSendersInner) GetSenderId() string`

GetSenderId returns the SenderId field if non-nil, zero value otherwise.

### GetSenderIdOk

`func (o *SmsCampaignSendersInner) GetSenderIdOk() (*string, bool)`

GetSenderIdOk returns a tuple with the SenderId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSenderId

`func (o *SmsCampaignSendersInner) SetSenderId(v string)`

SetSenderId sets SenderId field to given value.

### HasSenderId

`func (o *SmsCampaignSendersInner) HasSenderId() bool`

HasSenderId returns a boolean if a field has been set.

### GetSenderType

`func (o *SmsCampaignSendersInner) GetSenderType() string`

GetSenderType returns the SenderType field if non-nil, zero value otherwise.

### GetSenderTypeOk

`func (o *SmsCampaignSendersInner) GetSenderTypeOk() (*string, bool)`

GetSenderTypeOk returns a tuple with the SenderType field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSenderType

`func (o *SmsCampaignSendersInner) SetSenderType(v string)`

SetSenderType sets SenderType field to given value.

### HasSenderType

`func (o *SmsCampaignSendersInner) HasSenderType() bool`

HasSenderType returns a boolean if a field has been set.

### GetSenderCountryCode

`func (o *SmsCampaignSendersInner) GetSenderCountryCode() string`

GetSenderCountryCode returns the SenderCountryCode field if non-nil, zero value otherwise.

### GetSenderCountryCodeOk

`func (o *SmsCampaignSendersInner) GetSenderCountryCodeOk() (*string, bool)`

GetSenderCountryCodeOk returns a tuple with the SenderCountryCode field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSenderCountryCode

`func (o *SmsCampaignSendersInner) SetSenderCountryCode(v string)`

SetSenderCountryCode sets SenderCountryCode field to given value.

### HasSenderCountryCode

`func (o *SmsCampaignSendersInner) HasSenderCountryCode() bool`

HasSenderCountryCode returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


