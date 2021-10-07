# CampaignServiceSelector


<div lang=\"ja\">CampaignServiceSelectorオブジェクトは、getメソッドの検索条件（実行パラメータ）を保持します。</div> 

## Table of contents

### Properties

- [accountId](campaignserviceselector.md#accountid)
- [budgetAmountRange](campaignserviceselector.md#budgetamountrange)
- [campaignIds](campaignserviceselector.md#campaignids)
- [containsLabelIdFlg](campaignserviceselector.md#containslabelidflg)
- [conversionGroupIds](campaignserviceselector.md#conversiongroupids)
- [conversionTrackerIds](campaignserviceselector.md#conversiontrackerids)
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

### budgetAmountRange

• `Optional` **budgetAmountRange**: ``null`` \| [*CampaignServiceBudgetAmountRange*](campaignservicebudgetamountrange.md)

**`memberof`** CampaignServiceSelector

___

### campaignIds

• `Optional` **campaignIds**: ``null`` \| *number*[]

<div lang=\"ja\">検索条件 : キャンペーンID</div> 

**`memberof`** CampaignServiceSelector

___

### containsLabelIdFlg

• `Optional` **containsLabelIdFlg**: ``null`` \| *boolean*

<div lang=\"ja\">ラベルID取得フラグ</div> 

**`memberof`** CampaignServiceSelector

___

### conversionGroupIds

• `Optional` **conversionGroupIds**: ``null`` \| *number*[]

<div lang=\"ja\">検索条件 : コンバージョングループID</div> 

**`memberof`** CampaignServiceSelector

___

### conversionTrackerIds

• `Optional` **conversionTrackerIds**: ``null`` \| *number*[]

<div lang=\"ja\">検索条件 : コンバージョントラッカーID</div> 

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
