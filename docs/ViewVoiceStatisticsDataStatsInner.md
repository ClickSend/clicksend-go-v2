# ViewVoiceStatisticsDataStatsInner

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Date** | Pointer to **float32** | The date. | [optional] 
**Outbound** | Pointer to [**ViewVoiceStatisticsDataStatsInnerOutbound**](ViewVoiceStatisticsDataStatsInnerOutbound.md) |  | [optional] 
**Bounced** | Pointer to [**CancelAllSmsData**](CancelAllSmsData.md) |  | [optional] 

## Methods

### NewViewVoiceStatisticsDataStatsInner

`func NewViewVoiceStatisticsDataStatsInner() *ViewVoiceStatisticsDataStatsInner`

NewViewVoiceStatisticsDataStatsInner instantiates a new ViewVoiceStatisticsDataStatsInner object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewViewVoiceStatisticsDataStatsInnerWithDefaults

`func NewViewVoiceStatisticsDataStatsInnerWithDefaults() *ViewVoiceStatisticsDataStatsInner`

NewViewVoiceStatisticsDataStatsInnerWithDefaults instantiates a new ViewVoiceStatisticsDataStatsInner object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetDate

`func (o *ViewVoiceStatisticsDataStatsInner) GetDate() float32`

GetDate returns the Date field if non-nil, zero value otherwise.

### GetDateOk

`func (o *ViewVoiceStatisticsDataStatsInner) GetDateOk() (*float32, bool)`

GetDateOk returns a tuple with the Date field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDate

`func (o *ViewVoiceStatisticsDataStatsInner) SetDate(v float32)`

SetDate sets Date field to given value.

### HasDate

`func (o *ViewVoiceStatisticsDataStatsInner) HasDate() bool`

HasDate returns a boolean if a field has been set.

### GetOutbound

`func (o *ViewVoiceStatisticsDataStatsInner) GetOutbound() ViewVoiceStatisticsDataStatsInnerOutbound`

GetOutbound returns the Outbound field if non-nil, zero value otherwise.

### GetOutboundOk

`func (o *ViewVoiceStatisticsDataStatsInner) GetOutboundOk() (*ViewVoiceStatisticsDataStatsInnerOutbound, bool)`

GetOutboundOk returns a tuple with the Outbound field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetOutbound

`func (o *ViewVoiceStatisticsDataStatsInner) SetOutbound(v ViewVoiceStatisticsDataStatsInnerOutbound)`

SetOutbound sets Outbound field to given value.

### HasOutbound

`func (o *ViewVoiceStatisticsDataStatsInner) HasOutbound() bool`

HasOutbound returns a boolean if a field has been set.

### GetBounced

`func (o *ViewVoiceStatisticsDataStatsInner) GetBounced() CancelAllSmsData`

GetBounced returns the Bounced field if non-nil, zero value otherwise.

### GetBouncedOk

`func (o *ViewVoiceStatisticsDataStatsInner) GetBouncedOk() (*CancelAllSmsData, bool)`

GetBouncedOk returns a tuple with the Bounced field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetBounced

`func (o *ViewVoiceStatisticsDataStatsInner) SetBounced(v CancelAllSmsData)`

SetBounced sets Bounced field to given value.

### HasBounced

`func (o *ViewVoiceStatisticsDataStatsInner) HasBounced() bool`

HasBounced returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


