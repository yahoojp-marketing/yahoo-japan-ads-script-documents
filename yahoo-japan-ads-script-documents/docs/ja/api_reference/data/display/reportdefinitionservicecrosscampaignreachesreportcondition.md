# ReportDefinitionServiceCrossCampaignReachesReportCondition


<div lang=\"ja\">   ReportDefinitionServiceCrossCampaignReachesReportConditionオブジェクトは、横断リーチレポートの作成条件を表します。<br>   このフィールドは、ADD時に省略可能となり、REMOVE時に無視されます。<br>   ※ADD時、reportTypeが<code>CROSS_CAMPAIGN_REACHES</code>の場合は必須です。   ※crossCampaignIds、crossCampaignGoals、crossCampaignBuyingTypesには少なくとも2件の要素が必要です。   ※crossCampaignIds、crossCampaignGoals、crossCampaignBuyingTypesには最大で3件の要素を指定できます。 </div> 

## Table of contents

### Properties

- [crossCampaignBuyingTypes](reportdefinitionservicecrosscampaignreachesreportcondition.md#crosscampaignbuyingtypes)
- [crossCampaignGoals](reportdefinitionservicecrosscampaignreachesreportcondition.md#crosscampaigngoals)
- [crossCampaignIds](reportdefinitionservicecrosscampaignreachesreportcondition.md#crosscampaignids)
- [crossCampaignType](reportdefinitionservicecrosscampaignreachesreportcondition.md#crosscampaigntype)

## Properties

### crossCampaignBuyingTypes

• `Optional` **crossCampaignBuyingTypes**: ``null`` \| [*ReportDefinitionServiceCrossCampaignBuying*](reportdefinitionservicecrosscampaignbuying.md)[]

**`memberof`** ReportDefinitionServiceCrossCampaignReachesReportCondition

___

### crossCampaignGoals

• `Optional` **crossCampaignGoals**: ``null`` \| [*ReportDefinitionServiceCrossCampaignGoal*](reportdefinitionservicecrosscampaigngoal.md)[]

**`memberof`** ReportDefinitionServiceCrossCampaignReachesReportCondition

___

### crossCampaignIds

• `Optional` **crossCampaignIds**: ``null`` \| [*ReportDefinitionServiceCrossCampaignId*](reportdefinitionservicecrosscampaignid.md)[]

**`memberof`** ReportDefinitionServiceCrossCampaignReachesReportCondition

___

### crossCampaignType

• `Optional` **crossCampaignType**: ``null`` \| [*CampaignId*](./enums/reportdefinitionservicecrosscampaigntype.md#campaignid) \| [*CampaignGoal*](./enums/reportdefinitionservicecrosscampaigntype.md#campaigngoal) \| [*CampaignBuyingType*](./enums/reportdefinitionservicecrosscampaigntype.md#campaignbuyingtype) \| [*Unknown*](./enums/reportdefinitionservicecrosscampaigntype.md#unknown)

**`memberof`** ReportDefinitionServiceCrossCampaignReachesReportCondition
