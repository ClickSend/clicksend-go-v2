# CreateTestSmsReceiptRequest

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Url** | **string** | The webhook URL where the delivery receipt will be sent to. You can set the value to **poll** to send it to the ClickSend   system, and then retrieve it with the **View SMS Receipt** endpoint  &lt;div class&#x3D;\&quot;info-box\&quot;&gt;   &lt;h4&gt;&lt;i class&#x3D;\&quot;fas fa-info-circle\&quot;&gt;&lt;/i&gt; Note:&lt;/h4&gt;   &lt;p&gt;You can create a webhook URL in Pipedream to test receiving the SMS receipt. Follow the instructions &lt;a target&#x3D;\&quot;_blank\&quot; href&#x3D;\&quot;https://help.clicksend.com/en/articles/43703-integration-guide-pipedream\&quot;&gt;here&lt;/a&gt;.&lt;/p&gt; &lt;/div&gt; | 

## Methods

### NewCreateTestSmsReceiptRequest

`func NewCreateTestSmsReceiptRequest(url string, ) *CreateTestSmsReceiptRequest`

NewCreateTestSmsReceiptRequest instantiates a new CreateTestSmsReceiptRequest object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewCreateTestSmsReceiptRequestWithDefaults

`func NewCreateTestSmsReceiptRequestWithDefaults() *CreateTestSmsReceiptRequest`

NewCreateTestSmsReceiptRequestWithDefaults instantiates a new CreateTestSmsReceiptRequest object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetUrl

`func (o *CreateTestSmsReceiptRequest) GetUrl() string`

GetUrl returns the Url field if non-nil, zero value otherwise.

### GetUrlOk

`func (o *CreateTestSmsReceiptRequest) GetUrlOk() (*string, bool)`

GetUrlOk returns a tuple with the Url field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetUrl

`func (o *CreateTestSmsReceiptRequest) SetUrl(v string)`

SetUrl sets Url field to given value.



[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


