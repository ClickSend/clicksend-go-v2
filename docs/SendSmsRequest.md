# SendSmsRequest

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Senders** | Pointer to [**[]SendersInner**](SendersInner.md) | The &#x60;senders&#x60; property specifies sender IDs for each recipient country. - **Want to leverage the default sender settings:**   - If the &#x60;senders&#x60; property is missing or left empty, the system uses the default sender settings configured for each recipient country.  - **Want to override the default sender settings:**   - When the &#x60;senders&#x60; property is provided, it should contain valid sender IDs for each recipient country listed under recipients. These IDs will override the default sender settings for the specified countries.   - If an invalid sender ID is provided, or a sender ID for a specific recipient country is missing, the system will revert to using the default sender settings for that country.  | [optional] 
**ShortenUrls** | Pointer to **bool** | This controls whether URLs are automatically shortened. This affects all messages in the request. You can either specify:  - **True** - Automatically detects and shortens one URL on each message. - **False** - Leaves all URLs in their original form. This is the default value.  You will be able to retrieve the open rates and statistics for the link from this &lt;a href&#x3D;\&quot;/messaging/url-shortening/other/short-url-get-statistics\&quot;&gt;link&lt;/a&gt;.  More info about shortening URLs &lt;a href&#x3D;\&quot;/messaging/url-shortening/\&quot;&gt; here&lt;/a&gt;.  | [optional] 
**Messages** | Pointer to [**[]SendSmsRequestMessagesInner**](SendSmsRequestMessagesInner.md) | Messages to send to customers. | [optional] 

## Methods

### NewSendSmsRequest

`func NewSendSmsRequest() *SendSmsRequest`

NewSendSmsRequest instantiates a new SendSmsRequest object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewSendSmsRequestWithDefaults

`func NewSendSmsRequestWithDefaults() *SendSmsRequest`

NewSendSmsRequestWithDefaults instantiates a new SendSmsRequest object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetSenders

`func (o *SendSmsRequest) GetSenders() []SendersInner`

GetSenders returns the Senders field if non-nil, zero value otherwise.

### GetSendersOk

`func (o *SendSmsRequest) GetSendersOk() (*[]SendersInner, bool)`

GetSendersOk returns a tuple with the Senders field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSenders

`func (o *SendSmsRequest) SetSenders(v []SendersInner)`

SetSenders sets Senders field to given value.

### HasSenders

`func (o *SendSmsRequest) HasSenders() bool`

HasSenders returns a boolean if a field has been set.

### GetShortenUrls

`func (o *SendSmsRequest) GetShortenUrls() bool`

GetShortenUrls returns the ShortenUrls field if non-nil, zero value otherwise.

### GetShortenUrlsOk

`func (o *SendSmsRequest) GetShortenUrlsOk() (*bool, bool)`

GetShortenUrlsOk returns a tuple with the ShortenUrls field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetShortenUrls

`func (o *SendSmsRequest) SetShortenUrls(v bool)`

SetShortenUrls sets ShortenUrls field to given value.

### HasShortenUrls

`func (o *SendSmsRequest) HasShortenUrls() bool`

HasShortenUrls returns a boolean if a field has been set.

### GetMessages

`func (o *SendSmsRequest) GetMessages() []SendSmsRequestMessagesInner`

GetMessages returns the Messages field if non-nil, zero value otherwise.

### GetMessagesOk

`func (o *SendSmsRequest) GetMessagesOk() (*[]SendSmsRequestMessagesInner, bool)`

GetMessagesOk returns a tuple with the Messages field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetMessages

`func (o *SendSmsRequest) SetMessages(v []SendSmsRequestMessagesInner)`

SetMessages sets Messages field to given value.

### HasMessages

`func (o *SendSmsRequest) HasMessages() bool`

HasMessages returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


