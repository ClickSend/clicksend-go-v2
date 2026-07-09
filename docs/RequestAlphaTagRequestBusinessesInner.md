# RequestAlphaTagRequestBusinessesInner

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Country** | **string** |  | 
**BusinessName** | **string** |  | 
**BusinessRelationship** | **string** | Indicates your relationship to the business being registered.  - **PRIMARY**: Your primary business (linked to your ClickSend account). - **ENTITY_ASSOCIATE**: Sending on behalf of another business you represent or own.  | 
**BusinessInfo** | [**RequestAlphaTagRequestBusinessesInnerBusinessInfo**](RequestAlphaTagRequestBusinessesInnerBusinessInfo.md) |  | 
**BusinessAddress** | [**RequestAlphaTagRequestBusinessesInnerBusinessAddress**](RequestAlphaTagRequestBusinessesInnerBusinessAddress.md) |  | 
**Representative** | [**RequestAlphaTagRequestBusinessesInnerRepresentative**](RequestAlphaTagRequestBusinessesInnerRepresentative.md) |  | 
**Abn** | **string** | Australian Business Number (ABN), 11 digits | 
**PartnerBusinessName** | Pointer to **string** | Partner&#39;s business name. **Required** when &#x60;business_relationship&#x60; is &#x60;ENTITY_ASSOCIATE&#x60;. **Forbidden** otherwise.  | [optional] 
**PartnerAbn** | Pointer to **string** | Partner&#39;s Australian Business Number (ABN). Must contain only digits. **Required** when &#x60;business_relationship&#x60; is &#x60;ENTITY_ASSOCIATE&#x60;. **Forbidden** otherwise.  | [optional] 
**PartnerBusinessInfo** | Pointer to [**RequestAlphaTagRequestBusinessesInnerBusinessInfo**](RequestAlphaTagRequestBusinessesInnerBusinessInfo.md) |  | [optional] 
**PartnerBusinessAddress** | Pointer to [**RequestAlphaTagRequestBusinessesInnerBusinessAddress**](RequestAlphaTagRequestBusinessesInnerBusinessAddress.md) |  | [optional] 
**PartnerRepresentative** | Pointer to [**RequestAlphaTagRequestBusinessesInnerPartnerRepresentative**](RequestAlphaTagRequestBusinessesInnerPartnerRepresentative.md) |  | [optional] 

## Methods

### NewRequestAlphaTagRequestBusinessesInner

`func NewRequestAlphaTagRequestBusinessesInner(country string, businessName string, businessRelationship string, businessInfo RequestAlphaTagRequestBusinessesInnerBusinessInfo, businessAddress RequestAlphaTagRequestBusinessesInnerBusinessAddress, representative RequestAlphaTagRequestBusinessesInnerRepresentative, abn string, ) *RequestAlphaTagRequestBusinessesInner`

NewRequestAlphaTagRequestBusinessesInner instantiates a new RequestAlphaTagRequestBusinessesInner object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewRequestAlphaTagRequestBusinessesInnerWithDefaults

`func NewRequestAlphaTagRequestBusinessesInnerWithDefaults() *RequestAlphaTagRequestBusinessesInner`

NewRequestAlphaTagRequestBusinessesInnerWithDefaults instantiates a new RequestAlphaTagRequestBusinessesInner object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetCountry

`func (o *RequestAlphaTagRequestBusinessesInner) GetCountry() string`

GetCountry returns the Country field if non-nil, zero value otherwise.

### GetCountryOk

`func (o *RequestAlphaTagRequestBusinessesInner) GetCountryOk() (*string, bool)`

GetCountryOk returns a tuple with the Country field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCountry

`func (o *RequestAlphaTagRequestBusinessesInner) SetCountry(v string)`

SetCountry sets Country field to given value.


### GetBusinessName

`func (o *RequestAlphaTagRequestBusinessesInner) GetBusinessName() string`

GetBusinessName returns the BusinessName field if non-nil, zero value otherwise.

### GetBusinessNameOk

`func (o *RequestAlphaTagRequestBusinessesInner) GetBusinessNameOk() (*string, bool)`

GetBusinessNameOk returns a tuple with the BusinessName field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetBusinessName

`func (o *RequestAlphaTagRequestBusinessesInner) SetBusinessName(v string)`

SetBusinessName sets BusinessName field to given value.


### GetBusinessRelationship

`func (o *RequestAlphaTagRequestBusinessesInner) GetBusinessRelationship() string`

GetBusinessRelationship returns the BusinessRelationship field if non-nil, zero value otherwise.

### GetBusinessRelationshipOk

`func (o *RequestAlphaTagRequestBusinessesInner) GetBusinessRelationshipOk() (*string, bool)`

GetBusinessRelationshipOk returns a tuple with the BusinessRelationship field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetBusinessRelationship

`func (o *RequestAlphaTagRequestBusinessesInner) SetBusinessRelationship(v string)`

SetBusinessRelationship sets BusinessRelationship field to given value.


### GetBusinessInfo

`func (o *RequestAlphaTagRequestBusinessesInner) GetBusinessInfo() RequestAlphaTagRequestBusinessesInnerBusinessInfo`

GetBusinessInfo returns the BusinessInfo field if non-nil, zero value otherwise.

### GetBusinessInfoOk

`func (o *RequestAlphaTagRequestBusinessesInner) GetBusinessInfoOk() (*RequestAlphaTagRequestBusinessesInnerBusinessInfo, bool)`

GetBusinessInfoOk returns a tuple with the BusinessInfo field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetBusinessInfo

`func (o *RequestAlphaTagRequestBusinessesInner) SetBusinessInfo(v RequestAlphaTagRequestBusinessesInnerBusinessInfo)`

SetBusinessInfo sets BusinessInfo field to given value.


### GetBusinessAddress

`func (o *RequestAlphaTagRequestBusinessesInner) GetBusinessAddress() RequestAlphaTagRequestBusinessesInnerBusinessAddress`

GetBusinessAddress returns the BusinessAddress field if non-nil, zero value otherwise.

### GetBusinessAddressOk

`func (o *RequestAlphaTagRequestBusinessesInner) GetBusinessAddressOk() (*RequestAlphaTagRequestBusinessesInnerBusinessAddress, bool)`

GetBusinessAddressOk returns a tuple with the BusinessAddress field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetBusinessAddress

`func (o *RequestAlphaTagRequestBusinessesInner) SetBusinessAddress(v RequestAlphaTagRequestBusinessesInnerBusinessAddress)`

SetBusinessAddress sets BusinessAddress field to given value.


### GetRepresentative

`func (o *RequestAlphaTagRequestBusinessesInner) GetRepresentative() RequestAlphaTagRequestBusinessesInnerRepresentative`

GetRepresentative returns the Representative field if non-nil, zero value otherwise.

### GetRepresentativeOk

`func (o *RequestAlphaTagRequestBusinessesInner) GetRepresentativeOk() (*RequestAlphaTagRequestBusinessesInnerRepresentative, bool)`

GetRepresentativeOk returns a tuple with the Representative field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetRepresentative

`func (o *RequestAlphaTagRequestBusinessesInner) SetRepresentative(v RequestAlphaTagRequestBusinessesInnerRepresentative)`

SetRepresentative sets Representative field to given value.


### GetAbn

`func (o *RequestAlphaTagRequestBusinessesInner) GetAbn() string`

GetAbn returns the Abn field if non-nil, zero value otherwise.

### GetAbnOk

`func (o *RequestAlphaTagRequestBusinessesInner) GetAbnOk() (*string, bool)`

GetAbnOk returns a tuple with the Abn field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAbn

`func (o *RequestAlphaTagRequestBusinessesInner) SetAbn(v string)`

SetAbn sets Abn field to given value.


### GetPartnerBusinessName

`func (o *RequestAlphaTagRequestBusinessesInner) GetPartnerBusinessName() string`

GetPartnerBusinessName returns the PartnerBusinessName field if non-nil, zero value otherwise.

### GetPartnerBusinessNameOk

`func (o *RequestAlphaTagRequestBusinessesInner) GetPartnerBusinessNameOk() (*string, bool)`

GetPartnerBusinessNameOk returns a tuple with the PartnerBusinessName field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetPartnerBusinessName

`func (o *RequestAlphaTagRequestBusinessesInner) SetPartnerBusinessName(v string)`

SetPartnerBusinessName sets PartnerBusinessName field to given value.

### HasPartnerBusinessName

`func (o *RequestAlphaTagRequestBusinessesInner) HasPartnerBusinessName() bool`

HasPartnerBusinessName returns a boolean if a field has been set.

### GetPartnerAbn

`func (o *RequestAlphaTagRequestBusinessesInner) GetPartnerAbn() string`

GetPartnerAbn returns the PartnerAbn field if non-nil, zero value otherwise.

### GetPartnerAbnOk

`func (o *RequestAlphaTagRequestBusinessesInner) GetPartnerAbnOk() (*string, bool)`

GetPartnerAbnOk returns a tuple with the PartnerAbn field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetPartnerAbn

`func (o *RequestAlphaTagRequestBusinessesInner) SetPartnerAbn(v string)`

SetPartnerAbn sets PartnerAbn field to given value.

### HasPartnerAbn

`func (o *RequestAlphaTagRequestBusinessesInner) HasPartnerAbn() bool`

HasPartnerAbn returns a boolean if a field has been set.

### GetPartnerBusinessInfo

`func (o *RequestAlphaTagRequestBusinessesInner) GetPartnerBusinessInfo() RequestAlphaTagRequestBusinessesInnerBusinessInfo`

GetPartnerBusinessInfo returns the PartnerBusinessInfo field if non-nil, zero value otherwise.

### GetPartnerBusinessInfoOk

`func (o *RequestAlphaTagRequestBusinessesInner) GetPartnerBusinessInfoOk() (*RequestAlphaTagRequestBusinessesInnerBusinessInfo, bool)`

GetPartnerBusinessInfoOk returns a tuple with the PartnerBusinessInfo field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetPartnerBusinessInfo

`func (o *RequestAlphaTagRequestBusinessesInner) SetPartnerBusinessInfo(v RequestAlphaTagRequestBusinessesInnerBusinessInfo)`

SetPartnerBusinessInfo sets PartnerBusinessInfo field to given value.

### HasPartnerBusinessInfo

`func (o *RequestAlphaTagRequestBusinessesInner) HasPartnerBusinessInfo() bool`

HasPartnerBusinessInfo returns a boolean if a field has been set.

### GetPartnerBusinessAddress

`func (o *RequestAlphaTagRequestBusinessesInner) GetPartnerBusinessAddress() RequestAlphaTagRequestBusinessesInnerBusinessAddress`

GetPartnerBusinessAddress returns the PartnerBusinessAddress field if non-nil, zero value otherwise.

### GetPartnerBusinessAddressOk

`func (o *RequestAlphaTagRequestBusinessesInner) GetPartnerBusinessAddressOk() (*RequestAlphaTagRequestBusinessesInnerBusinessAddress, bool)`

GetPartnerBusinessAddressOk returns a tuple with the PartnerBusinessAddress field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetPartnerBusinessAddress

`func (o *RequestAlphaTagRequestBusinessesInner) SetPartnerBusinessAddress(v RequestAlphaTagRequestBusinessesInnerBusinessAddress)`

SetPartnerBusinessAddress sets PartnerBusinessAddress field to given value.

### HasPartnerBusinessAddress

`func (o *RequestAlphaTagRequestBusinessesInner) HasPartnerBusinessAddress() bool`

HasPartnerBusinessAddress returns a boolean if a field has been set.

### GetPartnerRepresentative

`func (o *RequestAlphaTagRequestBusinessesInner) GetPartnerRepresentative() RequestAlphaTagRequestBusinessesInnerPartnerRepresentative`

GetPartnerRepresentative returns the PartnerRepresentative field if non-nil, zero value otherwise.

### GetPartnerRepresentativeOk

`func (o *RequestAlphaTagRequestBusinessesInner) GetPartnerRepresentativeOk() (*RequestAlphaTagRequestBusinessesInnerPartnerRepresentative, bool)`

GetPartnerRepresentativeOk returns a tuple with the PartnerRepresentative field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetPartnerRepresentative

`func (o *RequestAlphaTagRequestBusinessesInner) SetPartnerRepresentative(v RequestAlphaTagRequestBusinessesInnerPartnerRepresentative)`

SetPartnerRepresentative sets PartnerRepresentative field to given value.

### HasPartnerRepresentative

`func (o *RequestAlphaTagRequestBusinessesInner) HasPartnerRepresentative() bool`

HasPartnerRepresentative returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


