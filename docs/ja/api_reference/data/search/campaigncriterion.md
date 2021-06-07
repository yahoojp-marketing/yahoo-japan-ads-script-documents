# CampaignCriterion


<div lang=\"ja\">CampaignCriterionオブジェクトは、キャンペーンのクライテリアを表します。</div> 

## Table of contents

### Properties

- [accountId](campaigncriterion.md#accountid)
- [campaignId](campaigncriterion.md#campaignid)
- [campaignName](campaigncriterion.md#campaignname)
- [criterion](campaigncriterion.md#criterion)
- [use](campaigncriterion.md#use)

## Properties

### accountId

• `Optional` **accountId**: ``null`` \| *number*

<div lang=\"ja\">アカウントIDです。<br> ADD時およびREMOVE時、このフィールドは必須です。</div> 

**`memberof`** CampaignCriterion

___

### campaignId

• `Optional` **campaignId**: ``null`` \| *number*

<div lang=\"ja\">キャンペーンIDです。<br> ADD時およびREMOVE時、このフィールドは必須です。</div> 

**`memberof`** CampaignCriterion

___

### campaignName

• `Optional` **campaignName**: ``null`` \| *string*

<div lang=\"ja\">キャンペーン名です。<br> このフィールドは、レスポンスの際に返却されますが、リクエストの際には無視されます。</div> 

**`memberof`** CampaignCriterion

___

### criterion

• `Optional` **criterion**: ``null`` \| [*CampaignCriterionServiceCriterion*](campaigncriterionservicecriterion.md)

**`memberof`** CampaignCriterion

___

### use

• `Optional` **use**: ``null`` \| [*Negative*](./enums/campaigncriterionserviceuse.md#negative) \| [*Unknown*](./enums/campaigncriterionserviceuse.md#unknown)

**`memberof`** CampaignCriterion
