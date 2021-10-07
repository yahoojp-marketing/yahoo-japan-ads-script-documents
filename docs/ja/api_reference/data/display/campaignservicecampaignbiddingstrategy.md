# CampaignServiceCampaignBiddingStrategy


<div lang=\"ja\"> CampaignServiceCampaignBiddingStrategyオブジェクトは、キャンペーン入札戦略です。<br> ADDおよびSET時、このフィールドは目的なしの場合は設定不可となり、目的ありの場合は必須となります。<br> REMOVE時、このフィールドは無視されます。 </div> 

## Table of contents

### Properties

- [campaignBiddingStrategyType](campaignservicecampaignbiddingstrategy.md#campaignbiddingstrategytype)
- [maxCpcBidValue](campaignservicecampaignbiddingstrategy.md#maxcpcbidvalue)
- [maxCpvBidValue](campaignservicecampaignbiddingstrategy.md#maxcpvbidvalue)
- [maxVcpmBidValue](campaignservicecampaignbiddingstrategy.md#maxvcpmbidvalue)
- [targetCpaBidValue](campaignservicecampaignbiddingstrategy.md#targetcpabidvalue)

## Properties

### campaignBiddingStrategyType

• `Optional` **campaignBiddingStrategyType**: ``null`` \| [*Auto*](./enums/campaignservicecampaignbiddingstrategytype.md#auto) \| [*MaximizeConversions*](./enums/campaignservicecampaignbiddingstrategytype.md#maximizeconversions) \| [*MaximizeClicks*](./enums/campaignservicecampaignbiddingstrategytype.md#maximizeclicks) \| [*MaximizeView*](./enums/campaignservicecampaignbiddingstrategytype.md#maximizeview) \| [*MaximizeVieableimpressions*](./enums/campaignservicecampaignbiddingstrategytype.md#maximizevieableimpressions) \| [*MaxVcpm*](./enums/campaignservicecampaignbiddingstrategytype.md#maxvcpm) \| [*MaxCpc*](./enums/campaignservicecampaignbiddingstrategytype.md#maxcpc) \| [*MaxCpv*](./enums/campaignservicecampaignbiddingstrategytype.md#maxcpv) \| [*TargetCpa*](./enums/campaignservicecampaignbiddingstrategytype.md#targetcpa) \| [*None*](./enums/campaignservicecampaignbiddingstrategytype.md#none) \| [*Unknown*](./enums/campaignservicecampaignbiddingstrategytype.md#unknown)

**`memberof`** CampaignServiceCampaignBiddingStrategy

___

### maxCpcBidValue

• `Optional` **maxCpcBidValue**: ``null`` \| *number*

<div lang=\"ja\"> キャンペーン最大入札価格(CPC)です。<br> このフィールドは、ADDおよびSET時に省略可能となり、REMOVE時に無視されます。 </div> 

**`memberof`** CampaignServiceCampaignBiddingStrategy

___

### maxCpvBidValue

• `Optional` **maxCpvBidValue**: ``null`` \| *number*

<div lang=\"ja\"> キャンペーン最大入札価格(CPV)です。<br> このフィールドは、ADDおよびSET時に省略可能となり、REMOVE時に無視されます。 </div> 

**`memberof`** CampaignServiceCampaignBiddingStrategy

___

### maxVcpmBidValue

• `Optional` **maxVcpmBidValue**: ``null`` \| *number*

<div lang=\"ja\"> キャンペーン最大入札価格(vCPM)です。<br> このフィールドは、ADDおよびSET時に省略可能となり、REMOVE時に無視されます。 </div> 

**`memberof`** CampaignServiceCampaignBiddingStrategy

___

### targetCpaBidValue

• `Optional` **targetCpaBidValue**: ``null`` \| *number*

<div lang=\"ja\"> キャンペーン目標単価(tCPA)です。<br> このフィールドは、ADDおよびSET時に省略可能となり、REMOVE時に無視されます。 </div> 

**`memberof`** CampaignServiceCampaignBiddingStrategy
