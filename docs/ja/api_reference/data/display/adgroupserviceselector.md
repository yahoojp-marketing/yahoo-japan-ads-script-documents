# AdGroupServiceSelector


<div lang=\"ja\">AdGroupServiceSelectorオブジェクトは、指定された広告グループを表します。</div> 

## Table of contents

### Properties

- [accountId](adgroupserviceselector.md#accountid)
- [adGroupIds](adgroupserviceselector.md#adgroupids)
- [campaignGoalFilterType](adgroupserviceselector.md#campaigngoalfiltertype)
- [campaignIds](adgroupserviceselector.md#campaignids)
- [containsLabelIdFlg](adgroupserviceselector.md#containslabelidflg)
- [createdDateRange](adgroupserviceselector.md#createddaterange)
- [feedSetIds](adgroupserviceselector.md#feedsetids)
- [labelIds](adgroupserviceselector.md#labelids)
- [numberResults](adgroupserviceselector.md#numberresults)
- [startIndex](adgroupserviceselector.md#startindex)
- [userStatuses](adgroupserviceselector.md#userstatuses)

## Properties

### accountId

• **accountId**: ``null`` \| *number*

<div lang=\"ja\">検索条件：アカウントID</div> 

**`memberof`** AdGroupServiceSelector

___

### adGroupIds

• `Optional` **adGroupIds**: ``null`` \| *number*[]

<div lang=\"ja\">検索条件：広告グループID</div> 

**`memberof`** AdGroupServiceSelector

___

### campaignGoalFilterType

• `Optional` **campaignGoalFilterType**: ``null`` \| [*All*](./enums/adgroupservicecampaigngoalfiltertype.md#all) \| [*NonGoal*](./enums/adgroupservicecampaigngoalfiltertype.md#nongoal) \| [*Goal*](./enums/adgroupservicecampaigngoalfiltertype.md#goal) \| [*Unknown*](./enums/adgroupservicecampaigngoalfiltertype.md#unknown)

**`memberof`** AdGroupServiceSelector

___

### campaignIds

• `Optional` **campaignIds**: ``null`` \| *number*[]

<div lang=\"ja\">検索条件：キャンペーンID</div> 

**`memberof`** AdGroupServiceSelector

___

### containsLabelIdFlg

• `Optional` **containsLabelIdFlg**: ``null`` \| *boolean*

<div lang=\"ja\">ラベルID取得フラグ</div> 

**`memberof`** AdGroupServiceSelector

___

### createdDateRange

• `Optional` **createdDateRange**: ``null`` \| [*AdGroupServiceCreatedDateRange*](adgroupservicecreateddaterange.md)

**`memberof`** AdGroupServiceSelector

___

### feedSetIds

• `Optional` **feedSetIds**: ``null`` \| *number*[]

<div lang=\"ja\">検索条件：フィードセットID</div> 

**`memberof`** AdGroupServiceSelector

___

### labelIds

• `Optional` **labelIds**: ``null`` \| *number*[]

<div lang=\"ja\">検索条件 : ラベルID</div> 

**`memberof`** AdGroupServiceSelector

___

### numberResults

• `Optional` **numberResults**: ``null`` \| *number*

<div lang=\"ja\">ページの最大件数です。このフィールドは、1以上を指定する必要があります。</div> 

**`memberof`** AdGroupServiceSelector

___

### startIndex

• `Optional` **startIndex**: ``null`` \| *number*

<div lang=\"ja\">ページの先頭のインデックスです。このフィールドは、1以上を指定する必要があります。</div> 

**`memberof`** AdGroupServiceSelector

___

### userStatuses

• `Optional` **userStatuses**: ``null`` \| [*AdGroupServiceUserStatus*](./enums/adgroupserviceuserstatus.md)[]

**`memberof`** AdGroupServiceSelector
