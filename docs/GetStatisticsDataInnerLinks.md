# GetStatisticsDataInnerLinks

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Total** | Pointer to **float32** | Total number of recipients | [optional] 
**OpenedUnique** | Pointer to **float32** | Total number of recipients that clicked the short URL | [optional] 
**OpenedTotal** | Pointer to **float32** | Total number of clicks on the short URL (e.g. when a recipient clicked the short URL twice, then it will add 2 here) | [optional] 
**Unopened** | Pointer to **float32** | Total number of recipients that did not click the short URL (i.e. &#x60;total&#x60; - &#x60;opened_unique&#x60;) | [optional] 

## Methods

### NewGetStatisticsDataInnerLinks

`func NewGetStatisticsDataInnerLinks() *GetStatisticsDataInnerLinks`

NewGetStatisticsDataInnerLinks instantiates a new GetStatisticsDataInnerLinks object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewGetStatisticsDataInnerLinksWithDefaults

`func NewGetStatisticsDataInnerLinksWithDefaults() *GetStatisticsDataInnerLinks`

NewGetStatisticsDataInnerLinksWithDefaults instantiates a new GetStatisticsDataInnerLinks object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetTotal

`func (o *GetStatisticsDataInnerLinks) GetTotal() float32`

GetTotal returns the Total field if non-nil, zero value otherwise.

### GetTotalOk

`func (o *GetStatisticsDataInnerLinks) GetTotalOk() (*float32, bool)`

GetTotalOk returns a tuple with the Total field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTotal

`func (o *GetStatisticsDataInnerLinks) SetTotal(v float32)`

SetTotal sets Total field to given value.

### HasTotal

`func (o *GetStatisticsDataInnerLinks) HasTotal() bool`

HasTotal returns a boolean if a field has been set.

### GetOpenedUnique

`func (o *GetStatisticsDataInnerLinks) GetOpenedUnique() float32`

GetOpenedUnique returns the OpenedUnique field if non-nil, zero value otherwise.

### GetOpenedUniqueOk

`func (o *GetStatisticsDataInnerLinks) GetOpenedUniqueOk() (*float32, bool)`

GetOpenedUniqueOk returns a tuple with the OpenedUnique field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetOpenedUnique

`func (o *GetStatisticsDataInnerLinks) SetOpenedUnique(v float32)`

SetOpenedUnique sets OpenedUnique field to given value.

### HasOpenedUnique

`func (o *GetStatisticsDataInnerLinks) HasOpenedUnique() bool`

HasOpenedUnique returns a boolean if a field has been set.

### GetOpenedTotal

`func (o *GetStatisticsDataInnerLinks) GetOpenedTotal() float32`

GetOpenedTotal returns the OpenedTotal field if non-nil, zero value otherwise.

### GetOpenedTotalOk

`func (o *GetStatisticsDataInnerLinks) GetOpenedTotalOk() (*float32, bool)`

GetOpenedTotalOk returns a tuple with the OpenedTotal field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetOpenedTotal

`func (o *GetStatisticsDataInnerLinks) SetOpenedTotal(v float32)`

SetOpenedTotal sets OpenedTotal field to given value.

### HasOpenedTotal

`func (o *GetStatisticsDataInnerLinks) HasOpenedTotal() bool`

HasOpenedTotal returns a boolean if a field has been set.

### GetUnopened

`func (o *GetStatisticsDataInnerLinks) GetUnopened() float32`

GetUnopened returns the Unopened field if non-nil, zero value otherwise.

### GetUnopenedOk

`func (o *GetStatisticsDataInnerLinks) GetUnopenedOk() (*float32, bool)`

GetUnopenedOk returns a tuple with the Unopened field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetUnopened

`func (o *GetStatisticsDataInnerLinks) SetUnopened(v float32)`

SetUnopened sets Unopened field to given value.

### HasUnopened

`func (o *GetStatisticsDataInnerLinks) HasUnopened() bool`

HasUnopened returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


