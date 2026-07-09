# ViewSmsStatisticsDataStatInner

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Date** | Pointer to **float32** | The date. | [optional] 
**Outbound** | Pointer to [**ViewVoiceStatisticsDataStatsInnerOutbound**](ViewVoiceStatisticsDataStatsInnerOutbound.md) |  | [optional] 
**Inbound** | Pointer to [**CancelAllSmsData**](CancelAllSmsData.md) |  | [optional] 
**Bounced** | Pointer to [**CancelAllSmsData**](CancelAllSmsData.md) |  | [optional] 

## Methods

### NewViewSmsStatisticsDataStatInner

`func NewViewSmsStatisticsDataStatInner() *ViewSmsStatisticsDataStatInner`

NewViewSmsStatisticsDataStatInner instantiates a new ViewSmsStatisticsDataStatInner object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewViewSmsStatisticsDataStatInnerWithDefaults

`func NewViewSmsStatisticsDataStatInnerWithDefaults() *ViewSmsStatisticsDataStatInner`

NewViewSmsStatisticsDataStatInnerWithDefaults instantiates a new ViewSmsStatisticsDataStatInner object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetDate

`func (o *ViewSmsStatisticsDataStatInner) GetDate() float32`

GetDate returns the Date field if non-nil, zero value otherwise.

### GetDateOk

`func (o *ViewSmsStatisticsDataStatInner) GetDateOk() (*float32, bool)`

GetDateOk returns a tuple with the Date field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDate

`func (o *ViewSmsStatisticsDataStatInner) SetDate(v float32)`

SetDate sets Date field to given value.

### HasDate

`func (o *ViewSmsStatisticsDataStatInner) HasDate() bool`

HasDate returns a boolean if a field has been set.

### GetOutbound

`func (o *ViewSmsStatisticsDataStatInner) GetOutbound() ViewVoiceStatisticsDataStatsInnerOutbound`

GetOutbound returns the Outbound field if non-nil, zero value otherwise.

### GetOutboundOk

`func (o *ViewSmsStatisticsDataStatInner) GetOutboundOk() (*ViewVoiceStatisticsDataStatsInnerOutbound, bool)`

GetOutboundOk returns a tuple with the Outbound field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetOutbound

`func (o *ViewSmsStatisticsDataStatInner) SetOutbound(v ViewVoiceStatisticsDataStatsInnerOutbound)`

SetOutbound sets Outbound field to given value.

### HasOutbound

`func (o *ViewSmsStatisticsDataStatInner) HasOutbound() bool`

HasOutbound returns a boolean if a field has been set.

### GetInbound

`func (o *ViewSmsStatisticsDataStatInner) GetInbound() CancelAllSmsData`

GetInbound returns the Inbound field if non-nil, zero value otherwise.

### GetInboundOk

`func (o *ViewSmsStatisticsDataStatInner) GetInboundOk() (*CancelAllSmsData, bool)`

GetInboundOk returns a tuple with the Inbound field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetInbound

`func (o *ViewSmsStatisticsDataStatInner) SetInbound(v CancelAllSmsData)`

SetInbound sets Inbound field to given value.

### HasInbound

`func (o *ViewSmsStatisticsDataStatInner) HasInbound() bool`

HasInbound returns a boolean if a field has been set.

### GetBounced

`func (o *ViewSmsStatisticsDataStatInner) GetBounced() CancelAllSmsData`

GetBounced returns the Bounced field if non-nil, zero value otherwise.

### GetBouncedOk

`func (o *ViewSmsStatisticsDataStatInner) GetBouncedOk() (*CancelAllSmsData, bool)`

GetBouncedOk returns a tuple with the Bounced field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetBounced

`func (o *ViewSmsStatisticsDataStatInner) SetBounced(v CancelAllSmsData)`

SetBounced sets Bounced field to given value.

### HasBounced

`func (o *ViewSmsStatisticsDataStatInner) HasBounced() bool`

HasBounced returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


