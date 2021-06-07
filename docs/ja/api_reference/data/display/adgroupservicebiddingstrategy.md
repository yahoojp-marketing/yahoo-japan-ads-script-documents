# AdGroupServiceBiddingStrategy


<div lang=\"ja\"> AdGroupServiceBiddingStrategyは、広告グループ入札戦略を表します。<br> ADDおよびSET時、このフィールドは省略可能となります。<br> ※目的ありのキャンペーンの場合のみ設定可能です。 </div> 

## Table of contents

### Properties

- [campaignBiddingStrategyType](adgroupservicebiddingstrategy.md#campaignbiddingstrategytype)
- [maxCpcBidValue](adgroupservicebiddingstrategy.md#maxcpcbidvalue)
- [maxCpvBidValue](adgroupservicebiddingstrategy.md#maxcpvbidvalue)
- [maxVcpmBidValue](adgroupservicebiddingstrategy.md#maxvcpmbidvalue)
- [targetCpaBidValue](adgroupservicebiddingstrategy.md#targetcpabidvalue)

## Properties

### campaignBiddingStrategyType

• `Optional` **campaignBiddingStrategyType**: ``null`` \| [*Auto*](./enums/adgroupservicecampaignbiddingstrategytype.md#auto) \| [*MaxVcpm*](./enums/adgroupservicecampaignbiddingstrategytype.md#maxvcpm) \| [*MaxCpc*](./enums/adgroupservicecampaignbiddingstrategytype.md#maxcpc) \| [*MaxCpv*](./enums/adgroupservicecampaignbiddingstrategytype.md#maxcpv) \| [*TargetCpa*](./enums/adgroupservicecampaignbiddingstrategytype.md#targetcpa) \| [*None*](./enums/adgroupservicecampaignbiddingstrategytype.md#none) \| [*Unknown*](./enums/adgroupservicecampaignbiddingstrategytype.md#unknown)

**`memberof`** AdGroupServiceBiddingStrategy

___

### maxCpcBidValue

• `Optional` **maxCpcBidValue**: ``null`` \| *number*

<div lang=\"ja\"> 広告グループ最大入札価格（CPC）です。<br> ADDおよびSET時、このフィールドは省略可能となります。<br> ※campaignBiddingStrategyTypeがMAX_CPCの場合のみ指定可能です。 </div> 

**`memberof`** AdGroupServiceBiddingStrategy

___

### maxCpvBidValue

• `Optional` **maxCpvBidValue**: ``null`` \| *number*

<div lang=\"ja\"> 広告グループ最大入札価格（CPV）です。<br> ADDおよびSET時、このフィールドは省略可能となります。<br> ※campaignBiddingStrategyTypeがMAX_CPVの場合のみ指定可能です。 </div> 

**`memberof`** AdGroupServiceBiddingStrategy

___

### maxVcpmBidValue

• `Optional` **maxVcpmBidValue**: ``null`` \| *number*

<div lang=\"ja\"> 広告グループ最大入札価格（vCPM）です。<br> ADDおよびSET時、このフィールドは省略可能となります。<br> ※campaignBiddingStrategyTypeがMAX_VCPMの場合のみ指定可能です。 </div> 

**`memberof`** AdGroupServiceBiddingStrategy

___

### targetCpaBidValue

• `Optional` **targetCpaBidValue**: ``null`` \| *number*

<div lang=\"ja\"> 広告グループ目標単価（tCPA）です。<br> ADDおよびSET時、このフィールドは省略可能となります。<br> ※campaignBiddingStrategyTypeがTARGET_CPAの場合のみ指定可能です。 </div> 

**`memberof`** AdGroupServiceBiddingStrategy
