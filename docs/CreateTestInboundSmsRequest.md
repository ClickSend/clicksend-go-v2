# CreateTestInboundSmsRequest

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Url** | **string** | The webhook URL where the inbound SMS will be sent to.  &lt;div class&#x3D;\&quot;info-box\&quot;&gt;   &lt;h4&gt;&lt;i class&#x3D;\&quot;fas fa-info-circle\&quot;&gt;&lt;/i&gt; Note:&lt;/h4&gt;   &lt;p&gt;You can create a webhook URL in &lt;em&gt;Pipedream&lt;/em&gt; to test receiving the inbound SMS. Follow the instructions &lt;a href&#x3D;\&quot;https://help.clicksend.com/en/articles/43703-integration-guide-pipedream\&quot; target&#x3D;\&quot;_blank\&quot;&gt;here.&lt;/a&gt;&lt;/p&gt; &lt;/div&gt;   | 
**WebhookType** | Pointer to **string** | Specifies the HTTP method used when the webhook sends a request to the URL. The available options are:  - **post** (Default): Sends the event data using an HTTP POST request.      - **get**: Sends the event data as query parameters in an HTTP GET request.      - **json**: Sends the event data using a custom JSON format (via a POST request).      This parameter is used to determine how the data will be transmitted, depending on your preferred method and how the receiving system is designed to process incoming requests. | [optional] 

## Methods

### NewCreateTestInboundSmsRequest

`func NewCreateTestInboundSmsRequest(url string, ) *CreateTestInboundSmsRequest`

NewCreateTestInboundSmsRequest instantiates a new CreateTestInboundSmsRequest object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewCreateTestInboundSmsRequestWithDefaults

`func NewCreateTestInboundSmsRequestWithDefaults() *CreateTestInboundSmsRequest`

NewCreateTestInboundSmsRequestWithDefaults instantiates a new CreateTestInboundSmsRequest object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetUrl

`func (o *CreateTestInboundSmsRequest) GetUrl() string`

GetUrl returns the Url field if non-nil, zero value otherwise.

### GetUrlOk

`func (o *CreateTestInboundSmsRequest) GetUrlOk() (*string, bool)`

GetUrlOk returns a tuple with the Url field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetUrl

`func (o *CreateTestInboundSmsRequest) SetUrl(v string)`

SetUrl sets Url field to given value.


### GetWebhookType

`func (o *CreateTestInboundSmsRequest) GetWebhookType() string`

GetWebhookType returns the WebhookType field if non-nil, zero value otherwise.

### GetWebhookTypeOk

`func (o *CreateTestInboundSmsRequest) GetWebhookTypeOk() (*string, bool)`

GetWebhookTypeOk returns a tuple with the WebhookType field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetWebhookType

`func (o *CreateTestInboundSmsRequest) SetWebhookType(v string)`

SetWebhookType sets WebhookType field to given value.

### HasWebhookType

`func (o *CreateTestInboundSmsRequest) HasWebhookType() bool`

HasWebhookType returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


