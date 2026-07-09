# ListCompliantSenderTypes200ResponseDataDataInner

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**RecipientCountryCode** | **string** | ISO 3166-1 alpha-2 formatted country code | 
**BlockedSenderTypes** | **[]string** | List of blocked sender types in recipient country | 
**AllowedSenderTypes** | [**[]ListCompliantSenderTypes200ResponseDataDataInnerAllowedSenderTypesInner**](ListCompliantSenderTypes200ResponseDataDataInnerAllowedSenderTypesInner.md) |  | 

## Methods

### NewListCompliantSenderTypes200ResponseDataDataInner

`func NewListCompliantSenderTypes200ResponseDataDataInner(recipientCountryCode string, blockedSenderTypes []string, allowedSenderTypes []ListCompliantSenderTypes200ResponseDataDataInnerAllowedSenderTypesInner, ) *ListCompliantSenderTypes200ResponseDataDataInner`

NewListCompliantSenderTypes200ResponseDataDataInner instantiates a new ListCompliantSenderTypes200ResponseDataDataInner object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewListCompliantSenderTypes200ResponseDataDataInnerWithDefaults

`func NewListCompliantSenderTypes200ResponseDataDataInnerWithDefaults() *ListCompliantSenderTypes200ResponseDataDataInner`

NewListCompliantSenderTypes200ResponseDataDataInnerWithDefaults instantiates a new ListCompliantSenderTypes200ResponseDataDataInner object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetRecipientCountryCode

`func (o *ListCompliantSenderTypes200ResponseDataDataInner) GetRecipientCountryCode() string`

GetRecipientCountryCode returns the RecipientCountryCode field if non-nil, zero value otherwise.

### GetRecipientCountryCodeOk

`func (o *ListCompliantSenderTypes200ResponseDataDataInner) GetRecipientCountryCodeOk() (*string, bool)`

GetRecipientCountryCodeOk returns a tuple with the RecipientCountryCode field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetRecipientCountryCode

`func (o *ListCompliantSenderTypes200ResponseDataDataInner) SetRecipientCountryCode(v string)`

SetRecipientCountryCode sets RecipientCountryCode field to given value.


### GetBlockedSenderTypes

`func (o *ListCompliantSenderTypes200ResponseDataDataInner) GetBlockedSenderTypes() []string`

GetBlockedSenderTypes returns the BlockedSenderTypes field if non-nil, zero value otherwise.

### GetBlockedSenderTypesOk

`func (o *ListCompliantSenderTypes200ResponseDataDataInner) GetBlockedSenderTypesOk() (*[]string, bool)`

GetBlockedSenderTypesOk returns a tuple with the BlockedSenderTypes field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetBlockedSenderTypes

`func (o *ListCompliantSenderTypes200ResponseDataDataInner) SetBlockedSenderTypes(v []string)`

SetBlockedSenderTypes sets BlockedSenderTypes field to given value.


### GetAllowedSenderTypes

`func (o *ListCompliantSenderTypes200ResponseDataDataInner) GetAllowedSenderTypes() []ListCompliantSenderTypes200ResponseDataDataInnerAllowedSenderTypesInner`

GetAllowedSenderTypes returns the AllowedSenderTypes field if non-nil, zero value otherwise.

### GetAllowedSenderTypesOk

`func (o *ListCompliantSenderTypes200ResponseDataDataInner) GetAllowedSenderTypesOk() (*[]ListCompliantSenderTypes200ResponseDataDataInnerAllowedSenderTypesInner, bool)`

GetAllowedSenderTypesOk returns a tuple with the AllowedSenderTypes field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAllowedSenderTypes

`func (o *ListCompliantSenderTypes200ResponseDataDataInner) SetAllowedSenderTypes(v []ListCompliantSenderTypes200ResponseDataDataInnerAllowedSenderTypesInner)`

SetAllowedSenderTypes sets AllowedSenderTypes field to given value.



[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


