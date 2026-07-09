# SendPostcardRequest

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**FileUrls** | Pointer to **[]string** |  | [optional] 
**Recipients** | Pointer to [**[]SendPostcardRequestRecipientsInner**](SendPostcardRequestRecipientsInner.md) |  | [optional] 

## Methods

### NewSendPostcardRequest

`func NewSendPostcardRequest() *SendPostcardRequest`

NewSendPostcardRequest instantiates a new SendPostcardRequest object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewSendPostcardRequestWithDefaults

`func NewSendPostcardRequestWithDefaults() *SendPostcardRequest`

NewSendPostcardRequestWithDefaults instantiates a new SendPostcardRequest object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetFileUrls

`func (o *SendPostcardRequest) GetFileUrls() []string`

GetFileUrls returns the FileUrls field if non-nil, zero value otherwise.

### GetFileUrlsOk

`func (o *SendPostcardRequest) GetFileUrlsOk() (*[]string, bool)`

GetFileUrlsOk returns a tuple with the FileUrls field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetFileUrls

`func (o *SendPostcardRequest) SetFileUrls(v []string)`

SetFileUrls sets FileUrls field to given value.

### HasFileUrls

`func (o *SendPostcardRequest) HasFileUrls() bool`

HasFileUrls returns a boolean if a field has been set.

### GetRecipients

`func (o *SendPostcardRequest) GetRecipients() []SendPostcardRequestRecipientsInner`

GetRecipients returns the Recipients field if non-nil, zero value otherwise.

### GetRecipientsOk

`func (o *SendPostcardRequest) GetRecipientsOk() (*[]SendPostcardRequestRecipientsInner, bool)`

GetRecipientsOk returns a tuple with the Recipients field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetRecipients

`func (o *SendPostcardRequest) SetRecipients(v []SendPostcardRequestRecipientsInner)`

SetRecipients sets Recipients field to given value.

### HasRecipients

`func (o *SendPostcardRequest) HasRecipients() bool`

HasRecipients returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


