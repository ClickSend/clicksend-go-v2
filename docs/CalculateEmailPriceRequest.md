# CalculateEmailPriceRequest

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**To** | Pointer to [**[]SendEmailRequestToInner**](SendEmailRequestToInner.md) |  | [optional] 
**From** | Pointer to [**SendEmailRequestFrom**](SendEmailRequestFrom.md) |  | [optional] 
**Subject** | Pointer to **string** |  | [optional] 
**Body** | Pointer to **string** |  | [optional] 

## Methods

### NewCalculateEmailPriceRequest

`func NewCalculateEmailPriceRequest() *CalculateEmailPriceRequest`

NewCalculateEmailPriceRequest instantiates a new CalculateEmailPriceRequest object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewCalculateEmailPriceRequestWithDefaults

`func NewCalculateEmailPriceRequestWithDefaults() *CalculateEmailPriceRequest`

NewCalculateEmailPriceRequestWithDefaults instantiates a new CalculateEmailPriceRequest object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetTo

`func (o *CalculateEmailPriceRequest) GetTo() []SendEmailRequestToInner`

GetTo returns the To field if non-nil, zero value otherwise.

### GetToOk

`func (o *CalculateEmailPriceRequest) GetToOk() (*[]SendEmailRequestToInner, bool)`

GetToOk returns a tuple with the To field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTo

`func (o *CalculateEmailPriceRequest) SetTo(v []SendEmailRequestToInner)`

SetTo sets To field to given value.

### HasTo

`func (o *CalculateEmailPriceRequest) HasTo() bool`

HasTo returns a boolean if a field has been set.

### GetFrom

`func (o *CalculateEmailPriceRequest) GetFrom() SendEmailRequestFrom`

GetFrom returns the From field if non-nil, zero value otherwise.

### GetFromOk

`func (o *CalculateEmailPriceRequest) GetFromOk() (*SendEmailRequestFrom, bool)`

GetFromOk returns a tuple with the From field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetFrom

`func (o *CalculateEmailPriceRequest) SetFrom(v SendEmailRequestFrom)`

SetFrom sets From field to given value.

### HasFrom

`func (o *CalculateEmailPriceRequest) HasFrom() bool`

HasFrom returns a boolean if a field has been set.

### GetSubject

`func (o *CalculateEmailPriceRequest) GetSubject() string`

GetSubject returns the Subject field if non-nil, zero value otherwise.

### GetSubjectOk

`func (o *CalculateEmailPriceRequest) GetSubjectOk() (*string, bool)`

GetSubjectOk returns a tuple with the Subject field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSubject

`func (o *CalculateEmailPriceRequest) SetSubject(v string)`

SetSubject sets Subject field to given value.

### HasSubject

`func (o *CalculateEmailPriceRequest) HasSubject() bool`

HasSubject returns a boolean if a field has been set.

### GetBody

`func (o *CalculateEmailPriceRequest) GetBody() string`

GetBody returns the Body field if non-nil, zero value otherwise.

### GetBodyOk

`func (o *CalculateEmailPriceRequest) GetBodyOk() (*string, bool)`

GetBodyOk returns a tuple with the Body field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetBody

`func (o *CalculateEmailPriceRequest) SetBody(v string)`

SetBody sets Body field to given value.

### HasBody

`func (o *CalculateEmailPriceRequest) HasBody() bool`

HasBody returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


