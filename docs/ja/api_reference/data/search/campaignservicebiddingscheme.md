# CampaignServiceBiddingScheme


<div lang=\"ja\">CampaignServiceBiddingSchemeオブジェクトは、自動入札設定の詳細情報を表します。 （BiddingStrategyService以外用のオブジェクトです。）<br> ADD時、標準入札設定の場合、このフィールドは必須となり、ポートフォリオ入札設定の場合、設定不可となります。また、biddingStrategyIdと同時に設定することはできません。</div> 

## Table of contents

### Properties

- [biddingStrategyType](campaignservicebiddingscheme.md#biddingstrategytype)
- [manualCpcBiddingScheme](campaignservicebiddingscheme.md#manualcpcbiddingscheme)
- [maximizeConversionValueBiddingScheme](campaignservicebiddingscheme.md#maximizeconversionvaluebiddingscheme)
- [maximizeConversionsBiddingScheme](campaignservicebiddingscheme.md#maximizeconversionsbiddingscheme)
- [targetCpaBiddingScheme](campaignservicebiddingscheme.md#targetcpabiddingscheme)
- [targetImpressionShareScheme](campaignservicebiddingscheme.md#targetimpressionsharescheme)
- [targetRoasBiddingScheme](campaignservicebiddingscheme.md#targetroasbiddingscheme)
- [targetSpendBiddingScheme](campaignservicebiddingscheme.md#targetspendbiddingscheme)

## Properties

### biddingStrategyType

• `Optional` **biddingStrategyType**: ``null`` \| [*ManualCpc*](./enums/campaignservicebiddingstrategytype.md#manualcpc) \| [*TargetRoas*](./enums/campaignservicebiddingstrategytype.md#targetroas) \| [*TargetSpend*](./enums/campaignservicebiddingstrategytype.md#targetspend) \| [*TargetCpa*](./enums/campaignservicebiddingstrategytype.md#targetcpa) \| [*MaximizeConversions*](./enums/campaignservicebiddingstrategytype.md#maximizeconversions) \| [*MaximizeConversionValue*](./enums/campaignservicebiddingstrategytype.md#maximizeconversionvalue) \| [*TargetImpressionShare*](./enums/campaignservicebiddingstrategytype.md#targetimpressionshare) \| [*Unknown*](./enums/campaignservicebiddingstrategytype.md#unknown)

**`memberof`** CampaignServiceBiddingScheme

___

### manualCpcBiddingScheme

• `Optional` **manualCpcBiddingScheme**: ``null`` \| [*CampaignServiceManualCpcBiddingScheme*](campaignservicemanualcpcbiddingscheme.md)

**`memberof`** CampaignServiceBiddingScheme

___

### maximizeConversionValueBiddingScheme

• `Optional` **maximizeConversionValueBiddingScheme**: ``null`` \| [*CampaignServiceMaximizeConversionValueBiddingScheme*](campaignservicemaximizeconversionvaluebiddingscheme.md)

**`memberof`** CampaignServiceBiddingScheme

___

### maximizeConversionsBiddingScheme

• `Optional` **maximizeConversionsBiddingScheme**: ``null`` \| [*CampaignServiceMaximizeConversionsBiddingScheme*](campaignservicemaximizeconversionsbiddingscheme.md)

**`memberof`** CampaignServiceBiddingScheme

___

### targetCpaBiddingScheme

• `Optional` **targetCpaBiddingScheme**: ``null`` \| [*CampaignServiceTargetCpaBiddingScheme*](campaignservicetargetcpabiddingscheme.md)

**`memberof`** CampaignServiceBiddingScheme

___

### targetImpressionShareScheme

• `Optional` **targetImpressionShareScheme**: ``null`` \| [*CampaignServiceTargetImpressionShareScheme*](campaignservicetargetimpressionsharescheme.md)

**`memberof`** CampaignServiceBiddingScheme

___

### targetRoasBiddingScheme

• `Optional` **targetRoasBiddingScheme**: ``null`` \| [*CampaignServiceTargetRoasBiddingScheme*](campaignservicetargetroasbiddingscheme.md)

**`memberof`** CampaignServiceBiddingScheme

___

### targetSpendBiddingScheme

• `Optional` **targetSpendBiddingScheme**: ``null`` \| [*CampaignServiceTargetSpendBiddingScheme*](campaignservicetargetspendbiddingscheme.md)

**`memberof`** CampaignServiceBiddingScheme
