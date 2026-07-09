# GetStatisticsDataInner

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**LongUrlId** | Pointer to **string** | ID of a URL under the specified source and source_id | [optional] 
**Links** | Pointer to [**GetStatisticsDataInnerLinks**](GetStatisticsDataInnerLinks.md) |  | [optional] 
**Device** | Pointer to [**[]GetStatisticsDataInnerDeviceInner**](GetStatisticsDataInnerDeviceInner.md) | Device statistics of the recipients that clicked the short URL | [optional] 
**Os** | Pointer to [**[]GetStatisticsDataInnerDeviceInner**](GetStatisticsDataInnerDeviceInner.md) | OS statistics of the recipients that clicked the short URL | [optional] 
**Browser** | Pointer to [**[]GetStatisticsDataInnerDeviceInner**](GetStatisticsDataInnerDeviceInner.md) | Browser statistics of the recipients that clicked the short URL | [optional] 
**Country** | Pointer to [**[]GetStatisticsDataInnerDeviceInner**](GetStatisticsDataInnerDeviceInner.md) | Country statistics of the recipients that clicked the short URL | [optional] 
**Region** | Pointer to [**[]GetStatisticsDataInnerDeviceInner**](GetStatisticsDataInnerDeviceInner.md) | Region statistics of the recipients that clicked the short URL | [optional] 

## Methods

### NewGetStatisticsDataInner

`func NewGetStatisticsDataInner() *GetStatisticsDataInner`

NewGetStatisticsDataInner instantiates a new GetStatisticsDataInner object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewGetStatisticsDataInnerWithDefaults

`func NewGetStatisticsDataInnerWithDefaults() *GetStatisticsDataInner`

NewGetStatisticsDataInnerWithDefaults instantiates a new GetStatisticsDataInner object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetLongUrlId

`func (o *GetStatisticsDataInner) GetLongUrlId() string`

GetLongUrlId returns the LongUrlId field if non-nil, zero value otherwise.

### GetLongUrlIdOk

`func (o *GetStatisticsDataInner) GetLongUrlIdOk() (*string, bool)`

GetLongUrlIdOk returns a tuple with the LongUrlId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetLongUrlId

`func (o *GetStatisticsDataInner) SetLongUrlId(v string)`

SetLongUrlId sets LongUrlId field to given value.

### HasLongUrlId

`func (o *GetStatisticsDataInner) HasLongUrlId() bool`

HasLongUrlId returns a boolean if a field has been set.

### GetLinks

`func (o *GetStatisticsDataInner) GetLinks() GetStatisticsDataInnerLinks`

GetLinks returns the Links field if non-nil, zero value otherwise.

### GetLinksOk

`func (o *GetStatisticsDataInner) GetLinksOk() (*GetStatisticsDataInnerLinks, bool)`

GetLinksOk returns a tuple with the Links field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetLinks

`func (o *GetStatisticsDataInner) SetLinks(v GetStatisticsDataInnerLinks)`

SetLinks sets Links field to given value.

### HasLinks

`func (o *GetStatisticsDataInner) HasLinks() bool`

HasLinks returns a boolean if a field has been set.

### GetDevice

`func (o *GetStatisticsDataInner) GetDevice() []GetStatisticsDataInnerDeviceInner`

GetDevice returns the Device field if non-nil, zero value otherwise.

### GetDeviceOk

`func (o *GetStatisticsDataInner) GetDeviceOk() (*[]GetStatisticsDataInnerDeviceInner, bool)`

GetDeviceOk returns a tuple with the Device field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDevice

`func (o *GetStatisticsDataInner) SetDevice(v []GetStatisticsDataInnerDeviceInner)`

SetDevice sets Device field to given value.

### HasDevice

`func (o *GetStatisticsDataInner) HasDevice() bool`

HasDevice returns a boolean if a field has been set.

### GetOs

`func (o *GetStatisticsDataInner) GetOs() []GetStatisticsDataInnerDeviceInner`

GetOs returns the Os field if non-nil, zero value otherwise.

### GetOsOk

`func (o *GetStatisticsDataInner) GetOsOk() (*[]GetStatisticsDataInnerDeviceInner, bool)`

GetOsOk returns a tuple with the Os field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetOs

`func (o *GetStatisticsDataInner) SetOs(v []GetStatisticsDataInnerDeviceInner)`

SetOs sets Os field to given value.

### HasOs

`func (o *GetStatisticsDataInner) HasOs() bool`

HasOs returns a boolean if a field has been set.

### GetBrowser

`func (o *GetStatisticsDataInner) GetBrowser() []GetStatisticsDataInnerDeviceInner`

GetBrowser returns the Browser field if non-nil, zero value otherwise.

### GetBrowserOk

`func (o *GetStatisticsDataInner) GetBrowserOk() (*[]GetStatisticsDataInnerDeviceInner, bool)`

GetBrowserOk returns a tuple with the Browser field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetBrowser

`func (o *GetStatisticsDataInner) SetBrowser(v []GetStatisticsDataInnerDeviceInner)`

SetBrowser sets Browser field to given value.

### HasBrowser

`func (o *GetStatisticsDataInner) HasBrowser() bool`

HasBrowser returns a boolean if a field has been set.

### GetCountry

`func (o *GetStatisticsDataInner) GetCountry() []GetStatisticsDataInnerDeviceInner`

GetCountry returns the Country field if non-nil, zero value otherwise.

### GetCountryOk

`func (o *GetStatisticsDataInner) GetCountryOk() (*[]GetStatisticsDataInnerDeviceInner, bool)`

GetCountryOk returns a tuple with the Country field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCountry

`func (o *GetStatisticsDataInner) SetCountry(v []GetStatisticsDataInnerDeviceInner)`

SetCountry sets Country field to given value.

### HasCountry

`func (o *GetStatisticsDataInner) HasCountry() bool`

HasCountry returns a boolean if a field has been set.

### GetRegion

`func (o *GetStatisticsDataInner) GetRegion() []GetStatisticsDataInnerDeviceInner`

GetRegion returns the Region field if non-nil, zero value otherwise.

### GetRegionOk

`func (o *GetStatisticsDataInner) GetRegionOk() (*[]GetStatisticsDataInnerDeviceInner, bool)`

GetRegionOk returns a tuple with the Region field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetRegion

`func (o *GetStatisticsDataInner) SetRegion(v []GetStatisticsDataInnerDeviceInner)`

SetRegion sets Region field to given value.

### HasRegion

`func (o *GetStatisticsDataInner) HasRegion() bool`

HasRegion returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


