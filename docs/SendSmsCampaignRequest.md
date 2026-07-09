# SendSmsCampaignRequest

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**ListId** | **int32** | The &#x60;list_id&#x60; of the contact list to send the message to. Use the  **&lt;a href&#x3D;\&quot;https://developers-dev.clicksend.net/docs/rest/v3/contacts/lists/other/view-list-contacts\&quot; target&#x3D;\&quot;_blank\&quot;&gt;View Contact List&lt;/a&gt;** endpoint to see your contact lists.  You can also use the other **&lt;a href&#x3D;\&quot;https://developers-dev.clicksend.net/docs/rest/v3/contacts/lists\&quot; target&#x3D;\&quot;_blank\&quot;&gt;list endpoints&lt;/a&gt;** to create and manage your contact list.  You need to provide the to parameter or the &#x60;list_id&#x60; parameter.  | 
**Name** | **string** | The SMS campaign name. | 
**From** | **string** | The sender of the message. This is also referred to as the **&lt;a href&#x3D;\&quot;https://help.clicksend.com/article/4kgj7krx00-what-is-a-sender-id-or-sender-number\&quot; target&#x3D;\&quot;_blank\&quot;&gt;Sender ID&lt;/a&gt;**. You can use: - **Shared number:** A number that is randomly selected from a pool if no number is specified. This is not available in the US and Canada. You can’t use a shared number if you have a dedicated number. - **Dedicated number:** A number you&#39;ve purchased from ClickSend. You can purchase a dedicated number using the &lt;a href&#x3D;\&quot;https://dashboard.clicksend.com/sender-ids/manage-senders\&quot; target&#x3D;\&quot;_blank\&quot;&gt;Dashboard&lt;/a&gt; or the [**Purchase Dedicated Number**](/) endpoint. It should be in the international format (&lt;a href&#x3D;\&quot;https://en.wikipedia.org/wiki/E.164\&quot; target&#x3D;\&quot;_blank\&quot;&gt;E.164&lt;/a&gt;). - **Alpha tag:** A sender name, like the name of your business, used as the **Sender ID** instead of a number. Recipients cannot reply to an alpha tag. You can register an alpha tag using the &lt;a href&#x3D;\&quot;https://dashboard.clicksend.com/sender-ids/manage-senders\&quot; target&#x3D;\&quot;_blank\&quot;&gt;dashboard&lt;/a&gt; or the **[Request Alpha Tag](/)** endpoint. Check which countries support alpha tags &lt;a href&#x3D;\&quot;https://help.clicksend.com/article/532u04vhaq-which-countries-support-alpha-tags\&quot; target&#x3D;\&quot;_blank\&quot;&gt;here&lt;/a&gt;. - **Own number:** Your own number that is connected to your account. Replies from recipients are sent directly to your number. You can register your own number using the &lt;a href&#x3D;\&quot;https://dashboard.clicksend.com/sender-ids/manage-senders\&quot; target&#x3D;\&quot;_blank\&quot;&gt;dashboard&lt;/a&gt; or the [**Request Own Number Verification OTP**](/) endpoint to get the _verification_id_ and OTP code needed for the [**Verify Own Number OTP**](/) endpoint. This isn&#39;t available in the US and Canada. If your **Sender ID** has a different country code to the recipient’s, it&#39;ll be replaced by a local number, except in &lt;a href&#x3D;\&quot;https://help.clicksend.com/category/mfdctha7f0-country-specific-features-and-restrictions\&quot; target&#x3D;\&quot;_blank\&quot;&gt;certain countries&lt;/a&gt;. If the sender number is blocked, a different number will replace it. | 
**Body** | **string** | The message to send. The price of sending a message depends on the number of characters and the type of message. There are two types:   - Standard message - Contains only characters in the &lt;a href&#x3D;\&quot;https://en.wikipedia.org/wiki/GSM_03.38\&quot; target&#x3D;\&quot;_blank\&quot;&gt;GSM&lt;/a&gt; set, with a maximum of 160 characters.   - Unicode message - Contains characters outside the &lt;a href&#x3D;\&quot;https://en.wikipedia.org/wiki/GSM_03.38\&quot; target&#x3D;\&quot;_blank\&quot;&gt;GSM&lt;/a&gt; set, with a maximum of 70 characters.   Longer messages will be sent as multiple messages (parts), but the recipient will receive them as a single long message. Visit &lt;a href&#x3D;\&quot;https://help.clicksend.com/article/h474eseq3a-how-many-characters-can-i-send-in-an-sms\&quot; target&#x3D;\&quot;_blank\&quot;&gt;this page&lt;/a&gt; to learn more about the number of characters per message, and &lt;a href&#x3D;\&quot;http://smscharactercount.com/#/counter\&quot; target&#x3D;\&quot;_blank\&quot;&gt;this page&lt;/a&gt; to count the number of characters. | 
**Source** | Pointer to **string** | The source of the request. For example, the name of your application. It&#39;s used to identify messages sent from various applications. | [optional] 
**Schedule** | Pointer to **int32** | The time you want the message to be sent. It should be in &lt;a href&#x3D;\&quot;http://help.clicksend.com/what-is-a-unix-timestamp\&quot; target&#x3D;\&quot;_blank\&quot;&gt;Unix format&lt;/a&gt;. | [optional] 
**Senders** | [**[]SendersInner**](SendersInner.md) | The &#x60;senders&#x60; property specifies sender IDs for each recipient country. - **Want to leverage the default sender settings:**   - If the &#x60;senders&#x60; property is missing or left empty, the system uses the default sender settings configured for each recipient country.  - **Want to override the default sender settings:**   - When the &#x60;senders&#x60; property is provided, it should contain valid sender IDs for each recipient country listed under recipients. These IDs will override the default sender settings for the specified countries.   - If an invalid sender ID is provided, or a sender ID for a specific recipient country is missing, the system will revert to using the default sender settings for that country.  | 
**UrlToShorten** | Pointer to **string** | The URL you want to shorten. The shortened URL will be appended to the end of the message body.   | [optional] 

## Methods

### NewSendSmsCampaignRequest

`func NewSendSmsCampaignRequest(listId int32, name string, from string, body string, senders []SendersInner, ) *SendSmsCampaignRequest`

NewSendSmsCampaignRequest instantiates a new SendSmsCampaignRequest object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewSendSmsCampaignRequestWithDefaults

`func NewSendSmsCampaignRequestWithDefaults() *SendSmsCampaignRequest`

NewSendSmsCampaignRequestWithDefaults instantiates a new SendSmsCampaignRequest object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetListId

`func (o *SendSmsCampaignRequest) GetListId() int32`

GetListId returns the ListId field if non-nil, zero value otherwise.

### GetListIdOk

`func (o *SendSmsCampaignRequest) GetListIdOk() (*int32, bool)`

GetListIdOk returns a tuple with the ListId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetListId

`func (o *SendSmsCampaignRequest) SetListId(v int32)`

SetListId sets ListId field to given value.


### GetName

`func (o *SendSmsCampaignRequest) GetName() string`

GetName returns the Name field if non-nil, zero value otherwise.

### GetNameOk

`func (o *SendSmsCampaignRequest) GetNameOk() (*string, bool)`

GetNameOk returns a tuple with the Name field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetName

`func (o *SendSmsCampaignRequest) SetName(v string)`

SetName sets Name field to given value.


### GetFrom

`func (o *SendSmsCampaignRequest) GetFrom() string`

GetFrom returns the From field if non-nil, zero value otherwise.

### GetFromOk

`func (o *SendSmsCampaignRequest) GetFromOk() (*string, bool)`

GetFromOk returns a tuple with the From field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetFrom

`func (o *SendSmsCampaignRequest) SetFrom(v string)`

SetFrom sets From field to given value.


### GetBody

`func (o *SendSmsCampaignRequest) GetBody() string`

GetBody returns the Body field if non-nil, zero value otherwise.

### GetBodyOk

`func (o *SendSmsCampaignRequest) GetBodyOk() (*string, bool)`

GetBodyOk returns a tuple with the Body field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetBody

`func (o *SendSmsCampaignRequest) SetBody(v string)`

SetBody sets Body field to given value.


### GetSource

`func (o *SendSmsCampaignRequest) GetSource() string`

GetSource returns the Source field if non-nil, zero value otherwise.

### GetSourceOk

`func (o *SendSmsCampaignRequest) GetSourceOk() (*string, bool)`

GetSourceOk returns a tuple with the Source field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSource

`func (o *SendSmsCampaignRequest) SetSource(v string)`

SetSource sets Source field to given value.

### HasSource

`func (o *SendSmsCampaignRequest) HasSource() bool`

HasSource returns a boolean if a field has been set.

### GetSchedule

`func (o *SendSmsCampaignRequest) GetSchedule() int32`

GetSchedule returns the Schedule field if non-nil, zero value otherwise.

### GetScheduleOk

`func (o *SendSmsCampaignRequest) GetScheduleOk() (*int32, bool)`

GetScheduleOk returns a tuple with the Schedule field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSchedule

`func (o *SendSmsCampaignRequest) SetSchedule(v int32)`

SetSchedule sets Schedule field to given value.

### HasSchedule

`func (o *SendSmsCampaignRequest) HasSchedule() bool`

HasSchedule returns a boolean if a field has been set.

### GetSenders

`func (o *SendSmsCampaignRequest) GetSenders() []SendersInner`

GetSenders returns the Senders field if non-nil, zero value otherwise.

### GetSendersOk

`func (o *SendSmsCampaignRequest) GetSendersOk() (*[]SendersInner, bool)`

GetSendersOk returns a tuple with the Senders field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSenders

`func (o *SendSmsCampaignRequest) SetSenders(v []SendersInner)`

SetSenders sets Senders field to given value.


### GetUrlToShorten

`func (o *SendSmsCampaignRequest) GetUrlToShorten() string`

GetUrlToShorten returns the UrlToShorten field if non-nil, zero value otherwise.

### GetUrlToShortenOk

`func (o *SendSmsCampaignRequest) GetUrlToShortenOk() (*string, bool)`

GetUrlToShortenOk returns a tuple with the UrlToShorten field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetUrlToShorten

`func (o *SendSmsCampaignRequest) SetUrlToShorten(v string)`

SetUrlToShorten sets UrlToShorten field to given value.

### HasUrlToShorten

`func (o *SendSmsCampaignRequest) HasUrlToShorten() bool`

HasUrlToShorten returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


