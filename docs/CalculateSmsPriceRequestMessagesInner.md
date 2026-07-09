# CalculateSmsPriceRequestMessagesInner

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Body** | **string** | The message to send. The price of sending a message depends on the number of characters and the type of message. There are two types:  - Standard message: Contains only characters in the &lt;a href&#x3D;\&quot;https://en.wikipedia.org/wiki/GSM_03.38\&quot; target&#x3D;\&quot;_blank\&quot;&gt;GSM&lt;/a&gt; set, with a maximum of 160 characters.      - Unicode message: Contains characters outside the &lt;a href&#x3D;\&quot;https://en.wikipedia.org/wiki/GSM_03.38\&quot; target&#x3D;\&quot;_blank\&quot;&gt;GSM&lt;/a&gt; set, with a maximum of 70 characters.      Longer messages will be sent as multiple messages (parts), but the recipient will receive them as a single long message. Visit &lt;a href&#x3D;\&quot;https://help.clicksend.com/article/h474eseq3a-how-many-characters-can-i-send-in-an-sms\&quot; target&#x3D;\&quot;_blank\&quot;&gt;this page&lt;/a&gt; to learn more about the number of characters per message, and &lt;a href&#x3D;\&quot;http://smscharactercount.com/\&quot; target&#x3D;\&quot;_blank\&quot;&gt;this page&lt;/a&gt; to count the number of characters. | 
**To** | Pointer to **string** | The phone number of the recipient. It should be in the international format (&lt;a href&#x3D;\&quot;https://en.wikipedia.org/wiki/E.164\&quot; target&#x3D;\&quot;_blank\&quot;&gt;E.164&lt;/a&gt;). You can send to a contact list using the _list_id_ parameter. You need to provide the to parameter or the _list_id_ parameter.  &lt;div class&#x3D;\&quot;info-box\&quot;&gt;   &lt;h4&gt;&lt;i class&#x3D;\&quot;fas fa-info-circle\&quot;&gt;&lt;/i&gt; Note:&lt;/h4&gt;   &lt;p&gt;To send SMS overseas, enable the &lt;a href&#x3D;\&quot;https://help.clicksend.com/article/qdavyt16qs-global-sending\&quot; target&#x3D;\&quot;_blank\&quot;&gt;global sending&lt;/a&gt; feature on your account either through the &lt;a href&#x3D;\&quot;https://dashboard.clicksend.com/global-sending\&quot; target&#x3D;\&quot;_blank\&quot;&gt;Dashboard&lt;/a&gt;, or by contacting &lt;a href&#x3D;\&quot;https://www.clicksend.com/au/help/\&quot; target&#x3D;\&quot;_blank\&quot;&gt;customer support.&lt;/a&gt;&lt;/p&gt; &lt;/div&gt;  | [optional] 
**From** | Pointer to **string** | The sender of the message. This is also referred to as the **&lt;a href&#x3D;\&quot;https://help.clicksend.com/article/4kgj7krx00-what-is-a-sender-id-or-sender-number\&quot; target&#x3D;\&quot;_blank\&quot;&gt;Sender ID&lt;/a&gt;**. You can use:  - Shared number: A number that is randomly selected from a pool if no number is specified. This is not available in the US and Canada. You can’t use a shared number if you have a dedicated number.      - Dedicated number: A number you&#39;ve purchased from ClickSend. You can purchase a dedicated number using the &lt;a href&#x3D;\&quot;https://dashboard.clicksend.com/sender-ids/manage-senders\&quot; target&#x3D;\&quot;_blank\&quot;&gt;Dashboard&lt;/a&gt; or the [**Purchase Dedicated Number**](/) endpoint. It should be in the international format (&lt;a href&#x3D;\&quot;https://en.wikipedia.org/wiki/E.164\&quot; target&#x3D;\&quot;_blank\&quot;&gt;E.164&lt;/a&gt;).      - Alpha tag: A sender name, like the name of your business, used as the **Sender ID** instead of a number. Recipients cannot reply to an alpha tag. You can register an alpha tag using the &lt;a href&#x3D;\&quot;https://dashboard.clicksend.com/sender-ids/manage-senders\&quot; target&#x3D;\&quot;_blank\&quot;&gt;dashboard&lt;/a&gt; or the [**Request Alpha Tag**](/) endpoint. Check which countries support alpha tags &lt;a href&#x3D;\&quot;https://help.clicksend.com/article/532u04vhaq-which-countries-support-alpha-tags\&quot; target&#x3D;\&quot;_blank\&quot;&gt;here&lt;/a&gt;.      - Own number: Your own number that is connected to your account. Replies from recipients are sent directly to your number. You can register your own number using the &lt;a href&#x3D;\&quot;https://dashboard.clicksend.com/sender-ids/manage-senders\&quot; target&#x3D;\&quot;_blank\&quot;&gt;dashboard&lt;/a&gt; or the [**Request Own Number Verification OTP**](/) endpoint to get the verification_id and OTP code needed for the [**Verify Own Number OTP**](/) endpoint. This isn&#39;t available in the US and Canada.      If your **Sender ID** has a different country code to the recipient’s, it&#39;ll be replaced by a local number, except in &lt;a href&#x3D;\&quot;https://help.clicksend.com/category/mfdctha7f0-country-specific-features-and-restrictions\&quot; target&#x3D;\&quot;_blank\&quot;&gt;certain countries&lt;/a&gt;. If the sender number is blocked, a different number will replace it. | [optional] 
**Source** | Pointer to **string** | The source of the request. For example, the name of your application. It&#39;s used to identify messages sent from various applications. | [optional] 
**Schedule** | Pointer to **int32** | The time you want the message to be sent. It should be in &lt;a href&#x3D;\&quot;http://help.clicksend.com/what-is-a-unix-timestamp\&quot; target&#x3D;\&quot;_blank\&quot;&gt;Unix format&lt;/a&gt;. | [optional] 
**CustomString** | Pointer to **string** | A note that will be sent back to you with the response from the endpoint. | [optional] 
**ListId** | Pointer to **string** | The _list_id_ of the contact list to send the message to. Use the [**View Contact List**](/contacts/lists/other/view-list-contacts) endpoint to see your contact lists. You can also use the other [lists endpoints](/contacts/lists/) to create and manage your contact list. You need to provide the _to_ parameter or the _list_id_ parameter. | [optional] 
**ContactId** | Pointer to **string** | The _contact_id_ of the contact to send the message to. A _contact_id_ is connected to a _list_id_. Use the [**Search Contact list**](/contacts/lists/#search-contact-lists) endpoint to view the _contact_id_ of the specified number. This parameter will be sent back to you with the response from the endpoint.  &lt;div class&#x3D;\&quot;warning-box\&quot;&gt;   &lt;h4&gt;&lt;i class&#x3D;\&quot;fas fa-exclamation-triangle\&quot;&gt;&lt;/i&gt; Warning:&lt;/h4&gt;   &lt;p&gt;This parameter is no longer in use.&lt;/p&gt; &lt;/div&gt; | [optional] 
**Country** | Pointer to **string** | The country code of the recipient in two-letter format (e.g. US, UK, AU, NZ, &lt;a href&#x3D;\&quot;https://help.clicksend.com/article/7wtbhhy6sy-country-code-calling-code-list\&quot; target&#x3D;\&quot;_blank\&quot; &gt;etc&lt;/a&gt;). | [optional] 
**ShowSummary** | Pointer to **bool** | Used for showing additional information in the response. You can either specify:   - **True:** It will show the additional information.        - **False:** It will only show the basic information. This is the default value.               | [optional] 

## Methods

### NewCalculateSmsPriceRequestMessagesInner

`func NewCalculateSmsPriceRequestMessagesInner(body string, ) *CalculateSmsPriceRequestMessagesInner`

NewCalculateSmsPriceRequestMessagesInner instantiates a new CalculateSmsPriceRequestMessagesInner object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewCalculateSmsPriceRequestMessagesInnerWithDefaults

`func NewCalculateSmsPriceRequestMessagesInnerWithDefaults() *CalculateSmsPriceRequestMessagesInner`

NewCalculateSmsPriceRequestMessagesInnerWithDefaults instantiates a new CalculateSmsPriceRequestMessagesInner object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetBody

`func (o *CalculateSmsPriceRequestMessagesInner) GetBody() string`

GetBody returns the Body field if non-nil, zero value otherwise.

### GetBodyOk

`func (o *CalculateSmsPriceRequestMessagesInner) GetBodyOk() (*string, bool)`

GetBodyOk returns a tuple with the Body field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetBody

`func (o *CalculateSmsPriceRequestMessagesInner) SetBody(v string)`

SetBody sets Body field to given value.


### GetTo

`func (o *CalculateSmsPriceRequestMessagesInner) GetTo() string`

GetTo returns the To field if non-nil, zero value otherwise.

### GetToOk

`func (o *CalculateSmsPriceRequestMessagesInner) GetToOk() (*string, bool)`

GetToOk returns a tuple with the To field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTo

`func (o *CalculateSmsPriceRequestMessagesInner) SetTo(v string)`

SetTo sets To field to given value.

### HasTo

`func (o *CalculateSmsPriceRequestMessagesInner) HasTo() bool`

HasTo returns a boolean if a field has been set.

### GetFrom

`func (o *CalculateSmsPriceRequestMessagesInner) GetFrom() string`

GetFrom returns the From field if non-nil, zero value otherwise.

### GetFromOk

`func (o *CalculateSmsPriceRequestMessagesInner) GetFromOk() (*string, bool)`

GetFromOk returns a tuple with the From field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetFrom

`func (o *CalculateSmsPriceRequestMessagesInner) SetFrom(v string)`

SetFrom sets From field to given value.

### HasFrom

`func (o *CalculateSmsPriceRequestMessagesInner) HasFrom() bool`

HasFrom returns a boolean if a field has been set.

### GetSource

`func (o *CalculateSmsPriceRequestMessagesInner) GetSource() string`

GetSource returns the Source field if non-nil, zero value otherwise.

### GetSourceOk

`func (o *CalculateSmsPriceRequestMessagesInner) GetSourceOk() (*string, bool)`

GetSourceOk returns a tuple with the Source field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSource

`func (o *CalculateSmsPriceRequestMessagesInner) SetSource(v string)`

SetSource sets Source field to given value.

### HasSource

`func (o *CalculateSmsPriceRequestMessagesInner) HasSource() bool`

HasSource returns a boolean if a field has been set.

### GetSchedule

`func (o *CalculateSmsPriceRequestMessagesInner) GetSchedule() int32`

GetSchedule returns the Schedule field if non-nil, zero value otherwise.

### GetScheduleOk

`func (o *CalculateSmsPriceRequestMessagesInner) GetScheduleOk() (*int32, bool)`

GetScheduleOk returns a tuple with the Schedule field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSchedule

`func (o *CalculateSmsPriceRequestMessagesInner) SetSchedule(v int32)`

SetSchedule sets Schedule field to given value.

### HasSchedule

`func (o *CalculateSmsPriceRequestMessagesInner) HasSchedule() bool`

HasSchedule returns a boolean if a field has been set.

### GetCustomString

`func (o *CalculateSmsPriceRequestMessagesInner) GetCustomString() string`

GetCustomString returns the CustomString field if non-nil, zero value otherwise.

### GetCustomStringOk

`func (o *CalculateSmsPriceRequestMessagesInner) GetCustomStringOk() (*string, bool)`

GetCustomStringOk returns a tuple with the CustomString field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCustomString

`func (o *CalculateSmsPriceRequestMessagesInner) SetCustomString(v string)`

SetCustomString sets CustomString field to given value.

### HasCustomString

`func (o *CalculateSmsPriceRequestMessagesInner) HasCustomString() bool`

HasCustomString returns a boolean if a field has been set.

### GetListId

`func (o *CalculateSmsPriceRequestMessagesInner) GetListId() string`

GetListId returns the ListId field if non-nil, zero value otherwise.

### GetListIdOk

`func (o *CalculateSmsPriceRequestMessagesInner) GetListIdOk() (*string, bool)`

GetListIdOk returns a tuple with the ListId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetListId

`func (o *CalculateSmsPriceRequestMessagesInner) SetListId(v string)`

SetListId sets ListId field to given value.

### HasListId

`func (o *CalculateSmsPriceRequestMessagesInner) HasListId() bool`

HasListId returns a boolean if a field has been set.

### GetContactId

`func (o *CalculateSmsPriceRequestMessagesInner) GetContactId() string`

GetContactId returns the ContactId field if non-nil, zero value otherwise.

### GetContactIdOk

`func (o *CalculateSmsPriceRequestMessagesInner) GetContactIdOk() (*string, bool)`

GetContactIdOk returns a tuple with the ContactId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetContactId

`func (o *CalculateSmsPriceRequestMessagesInner) SetContactId(v string)`

SetContactId sets ContactId field to given value.

### HasContactId

`func (o *CalculateSmsPriceRequestMessagesInner) HasContactId() bool`

HasContactId returns a boolean if a field has been set.

### GetCountry

`func (o *CalculateSmsPriceRequestMessagesInner) GetCountry() string`

GetCountry returns the Country field if non-nil, zero value otherwise.

### GetCountryOk

`func (o *CalculateSmsPriceRequestMessagesInner) GetCountryOk() (*string, bool)`

GetCountryOk returns a tuple with the Country field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCountry

`func (o *CalculateSmsPriceRequestMessagesInner) SetCountry(v string)`

SetCountry sets Country field to given value.

### HasCountry

`func (o *CalculateSmsPriceRequestMessagesInner) HasCountry() bool`

HasCountry returns a boolean if a field has been set.

### GetShowSummary

`func (o *CalculateSmsPriceRequestMessagesInner) GetShowSummary() bool`

GetShowSummary returns the ShowSummary field if non-nil, zero value otherwise.

### GetShowSummaryOk

`func (o *CalculateSmsPriceRequestMessagesInner) GetShowSummaryOk() (*bool, bool)`

GetShowSummaryOk returns a tuple with the ShowSummary field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetShowSummary

`func (o *CalculateSmsPriceRequestMessagesInner) SetShowSummary(v bool)`

SetShowSummary sets ShowSummary field to given value.

### HasShowSummary

`func (o *CalculateSmsPriceRequestMessagesInner) HasShowSummary() bool`

HasShowSummary returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


