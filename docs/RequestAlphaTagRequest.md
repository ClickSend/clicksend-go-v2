# RequestAlphaTagRequest

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**AlphaTag** | Pointer to **string** |  | [optional] 
**Reason** | Pointer to **string** |  | [optional] 
**Countries** | Pointer to **[]string** |  | [optional] 
**Businesses** | Pointer to [**[]RequestAlphaTagRequestBusinessesInner**](RequestAlphaTagRequestBusinessesInner.md) |  | [optional] 

## Methods

### NewRequestAlphaTagRequest

`func NewRequestAlphaTagRequest() *RequestAlphaTagRequest`

NewRequestAlphaTagRequest instantiates a new RequestAlphaTagRequest object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewRequestAlphaTagRequestWithDefaults

`func NewRequestAlphaTagRequestWithDefaults() *RequestAlphaTagRequest`

NewRequestAlphaTagRequestWithDefaults instantiates a new RequestAlphaTagRequest object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetAlphaTag

`func (o *RequestAlphaTagRequest) GetAlphaTag() string`

GetAlphaTag returns the AlphaTag field if non-nil, zero value otherwise.

### GetAlphaTagOk

`func (o *RequestAlphaTagRequest) GetAlphaTagOk() (*string, bool)`

GetAlphaTagOk returns a tuple with the AlphaTag field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAlphaTag

`func (o *RequestAlphaTagRequest) SetAlphaTag(v string)`

SetAlphaTag sets AlphaTag field to given value.

### HasAlphaTag

`func (o *RequestAlphaTagRequest) HasAlphaTag() bool`

HasAlphaTag returns a boolean if a field has been set.

### GetReason

`func (o *RequestAlphaTagRequest) GetReason() string`

GetReason returns the Reason field if non-nil, zero value otherwise.

### GetReasonOk

`func (o *RequestAlphaTagRequest) GetReasonOk() (*string, bool)`

GetReasonOk returns a tuple with the Reason field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetReason

`func (o *RequestAlphaTagRequest) SetReason(v string)`

SetReason sets Reason field to given value.

### HasReason

`func (o *RequestAlphaTagRequest) HasReason() bool`

HasReason returns a boolean if a field has been set.

### GetCountries

`func (o *RequestAlphaTagRequest) GetCountries() []string`

GetCountries returns the Countries field if non-nil, zero value otherwise.

### GetCountriesOk

`func (o *RequestAlphaTagRequest) GetCountriesOk() (*[]string, bool)`

GetCountriesOk returns a tuple with the Countries field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCountries

`func (o *RequestAlphaTagRequest) SetCountries(v []string)`

SetCountries sets Countries field to given value.

### HasCountries

`func (o *RequestAlphaTagRequest) HasCountries() bool`

HasCountries returns a boolean if a field has been set.

### GetBusinesses

`func (o *RequestAlphaTagRequest) GetBusinesses() []RequestAlphaTagRequestBusinessesInner`

GetBusinesses returns the Businesses field if non-nil, zero value otherwise.

### GetBusinessesOk

`func (o *RequestAlphaTagRequest) GetBusinessesOk() (*[]RequestAlphaTagRequestBusinessesInner, bool)`

GetBusinessesOk returns a tuple with the Businesses field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetBusinesses

`func (o *RequestAlphaTagRequest) SetBusinesses(v []RequestAlphaTagRequestBusinessesInner)`

SetBusinesses sets Businesses field to given value.

### HasBusinesses

`func (o *RequestAlphaTagRequest) HasBusinesses() bool`

HasBusinesses returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


