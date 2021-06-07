# CampaignCriterionServiceSelector


<div lang=\"ja\">CampaignCriterionServiceSelectorオブジェクトは、操作の対象となるキャンペーンのクライテリアを表します。</div> 

## Table of contents

### Properties

- [accountId](campaigncriterionserviceselector.md#accountid)
- [campaignIds](campaigncriterionserviceselector.md#campaignids)
- [criterionIds](campaigncriterionserviceselector.md#criterionids)
- [numberResults](campaigncriterionserviceselector.md#numberresults)
- [startIndex](campaigncriterionserviceselector.md#startindex)
- [use](campaigncriterionserviceselector.md#use)

## Properties

### accountId

• **accountId**: *number*

<div lang=\"ja\">アカウントIDです。</div> 

**`memberof`** CampaignCriterionServiceSelector

___

### campaignIds

• `Optional` **campaignIds**: ``null`` \| *number*[]

<div lang=\"ja\">キャンペーンIDの配列です。</div> 

**`memberof`** CampaignCriterionServiceSelector

___

### criterionIds

• `Optional` **criterionIds**: ``null`` \| *number*[]

<div lang=\"ja\">クライテリオンIDの配列です。<br> 指定しない場合は、キャンペーンID以下のすべてのクライテリアが含まれます。</div> 

**`memberof`** CampaignCriterionServiceSelector

___

### numberResults

• `Optional` **numberResults**: ``null`` \| *number*

<div lang=\"ja\">ページの最大件数です。このフィールドは、1以上を指定する必要があります。</div> 

**`memberof`** CampaignCriterionServiceSelector

___

### startIndex

• `Optional` **startIndex**: ``null`` \| *number*

<div lang=\"ja\">ページの先頭のインデックスです。このフィールドは、1以上を指定する必要があります。</div> 

**`memberof`** CampaignCriterionServiceSelector

___

### use

• `Optional` **use**: ``null`` \| [*Negative*](./enums/campaigncriterionserviceuse.md#negative) \| [*Unknown*](./enums/campaigncriterionserviceuse.md#unknown)

**`memberof`** CampaignCriterionServiceSelector
