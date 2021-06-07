# CampaignServiceSelector


<div lang=\"ja\">CampaignServiceSelectorオブジェクトは、getメソッドの検索条件（実行パラメータ）を保持します。</div> 

## Table of contents

### Properties

- [accountId](campaignserviceselector.md#accountid)
- [campaignGoalFilterType](campaignserviceselector.md#campaigngoalfiltertype)
- [campaignIds](campaignserviceselector.md#campaignids)
- [campaignType](campaignserviceselector.md#campaigntype)
- [containsLabelIdFlg](campaignserviceselector.md#containslabelidflg)
- [createdDateRange](campaignserviceselector.md#createddaterange)
- [feedIds](campaignserviceselector.md#feedids)
- [labelIds](campaignserviceselector.md#labelids)
- [numberResults](campaignserviceselector.md#numberresults)
- [startIndex](campaignserviceselector.md#startindex)
- [userStatuses](campaignserviceselector.md#userstatuses)

## Properties

### accountId

• **accountId**: *number*

<div lang=\"ja\">検索条件 : アカウントID</div> 

**`memberof`** CampaignServiceSelector

___

### campaignGoalFilterType

• `Optional` **campaignGoalFilterType**: ``null`` \| [*All*](./enums/campaignservicegoalfiltertype.md#all) \| [*NonGoal*](./enums/campaignservicegoalfiltertype.md#nongoal) \| [*Goal*](./enums/campaignservicegoalfiltertype.md#goal) \| [*Unknown*](./enums/campaignservicegoalfiltertype.md#unknown)

**`memberof`** CampaignServiceSelector

___

### campaignIds

• `Optional` **campaignIds**: ``null`` \| *number*[]

<div lang=\"ja\">検索条件 : キャンペーンID</div> 

**`memberof`** CampaignServiceSelector

___

### campaignType

• `Optional` **campaignType**: ``null`` \| [*Standard*](./enums/campaignservicetype.md#standard) \| [*App*](./enums/campaignservicetype.md#app) \| [*Unknown*](./enums/campaignservicetype.md#unknown)

**`memberof`** CampaignServiceSelector

___

### containsLabelIdFlg

• `Optional` **containsLabelIdFlg**: ``null`` \| *boolean*

<div lang=\"ja\">ラベルID取得フラグ</div> 

**`memberof`** CampaignServiceSelector

___

### createdDateRange

• `Optional` **createdDateRange**: ``null`` \| [*CampaignServiceCreatedDateRange*](campaignservicecreateddaterange.md)

**`memberof`** CampaignServiceSelector

___

### feedIds

• `Optional` **feedIds**: ``null`` \| *number*[]

<div lang=\"ja\">検索条件 : フィードID</div> 

**`memberof`** CampaignServiceSelector

___

### labelIds

• `Optional` **labelIds**: ``null`` \| *number*[]

<div lang=\"ja\">検索条件 : ラベルID</div> 

**`memberof`** CampaignServiceSelector

___

### numberResults

• `Optional` **numberResults**: ``null`` \| *number*

<div lang=\"ja\">ページの最大件数です。このフィールドは、1以上を指定する必要があります。</div> 

**`memberof`** CampaignServiceSelector

___

### startIndex

• `Optional` **startIndex**: ``null`` \| *number*

<div lang=\"ja\">ページの先頭のインデックスです。このフィールドは、1以上を指定する必要があります。</div> 

**`memberof`** CampaignServiceSelector

___

### userStatuses

• `Optional` **userStatuses**: ``null`` \| [*CampaignServiceUserStatus*](./enums/campaignserviceuserstatus.md)[]

<div lang=\"ja\">検索条件 : 取得範囲</div> 

**`memberof`** CampaignServiceSelector
