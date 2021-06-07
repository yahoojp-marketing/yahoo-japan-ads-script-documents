# CampaignCriterionServiceCriterion


<div lang=\"ja\">CampaignCriterionServiceCriterionオブジェクトは、クライテリアを表します。※キャンペーン用クライテリアです。<br> ADD時およびREMOVE時、このフィールドは必須です。</div> 

## Table of contents

### Properties

- [criterionId](campaigncriterionservicecriterion.md#criterionid)
- [criterionTrackId](campaigncriterionservicecriterion.md#criteriontrackid)
- [criterionType](campaigncriterionservicecriterion.md#criteriontype)
- [keyword](campaigncriterionservicecriterion.md#keyword)

## Properties

### criterionId

• `Optional` **criterionId**: ``null`` \| *number*

<div lang=\"ja\">クライテリアIDです。<br> REMOVE時、このフィールドは必須です。</div> 

**`memberof`** CampaignCriterionServiceCriterion

___

### criterionTrackId

• `Optional` **criterionTrackId**: ``null`` \| *number*

<div lang=\"ja\">クライテリオントラックIDです。<br> 対象外キーワードでは返却されません。</div> 

**`memberof`** CampaignCriterionServiceCriterion

___

### criterionType

• `Optional` **criterionType**: ``null`` \| [*Keyword*](./enums/campaigncriterionservicecriteriontype.md#keyword) \| [*Unknown*](./enums/campaigncriterionservicecriteriontype.md#unknown)

**`memberof`** CampaignCriterionServiceCriterion

___

### keyword

• `Optional` **keyword**: ``null`` \| [*CampaignCriterionServiceKeyword*](campaigncriterionservicekeyword.md)

**`memberof`** CampaignCriterionServiceCriterion
