# CampaignServiceBiddingStrategy


<div lang=\"ja\">CampaignServiceBiddingStrategyオブジェクトは、自動入札設定方法を表します。<br> ADD時、biddingStrategyConfigurationは必須となります。また、failedBiddingStrategyConfigurationはレスポンスの際に返却されますが、リクエストの際には無視されます。</div> 

## Table of contents

### Properties

- [biddingScheme](campaignservicebiddingstrategy.md#biddingscheme)
- [biddingStrategyId](campaignservicebiddingstrategy.md#biddingstrategyid)
- [biddingStrategyName](campaignservicebiddingstrategy.md#biddingstrategyname)
- [biddingStrategySource](campaignservicebiddingstrategy.md#biddingstrategysource)
- [biddingStrategyType](campaignservicebiddingstrategy.md#biddingstrategytype)

## Properties

### biddingScheme

• `Optional` **biddingScheme**: ``null`` \| [*CampaignServiceBiddingScheme*](campaignservicebiddingscheme.md)

**`memberof`** CampaignServiceBiddingStrategy

___

### biddingStrategyId

• `Optional` **biddingStrategyId**: ``null`` \| *number*

<div lang=\"ja\">自動入札IDです。<br> ADD時、標準入札設定の場合、このフィールドは設定不可となり、ポートフォリオ入札設定の場合、必須となります。また、biddingSchemeと同時に設定することはできません。</div> 

**`memberof`** CampaignServiceBiddingStrategy

___

### biddingStrategyName

• `Optional` **biddingStrategyName**: ``null`` \| *string*

<div lang=\"ja\">自動入札名です。<br> ADD時、このフィールドは無視されます。<br> ※50文字以内になります。</div> 

**`memberof`** CampaignServiceBiddingStrategy

___

### biddingStrategySource

• `Optional` **biddingStrategySource**: ``null`` \| [*Campaign*](./enums/campaignservicebiddingstrategysource.md#campaign) \| [*Unknown*](./enums/campaignservicebiddingstrategysource.md#unknown)

**`memberof`** CampaignServiceBiddingStrategy

___

### biddingStrategyType

• `Optional` **biddingStrategyType**: ``null`` \| [*ManualCpc*](./enums/campaignservicebiddingstrategytype.md#manualcpc) \| [*TargetRoas*](./enums/campaignservicebiddingstrategytype.md#targetroas) \| [*TargetSpend*](./enums/campaignservicebiddingstrategytype.md#targetspend) \| [*TargetCpa*](./enums/campaignservicebiddingstrategytype.md#targetcpa) \| [*MaximizeConversions*](./enums/campaignservicebiddingstrategytype.md#maximizeconversions) \| [*TargetImpressionShare*](./enums/campaignservicebiddingstrategytype.md#targetimpressionshare) \| [*Unknown*](./enums/campaignservicebiddingstrategytype.md#unknown)

**`memberof`** CampaignServiceBiddingStrategy
