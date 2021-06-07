# CampaignServiceSelector


<div lang=\"ja\">CampaignServiceSelectorオブジェクトは、操作の対象とするキャンペーンの情報およびフィルタ条件を表します。</div> 

## Table of contents

### Properties

- [accountId](campaignserviceselector.md#accountid)
- [biddingStrategyIds](campaignserviceselector.md#biddingstrategyids)
- [campaignIds](campaignserviceselector.md#campaignids)
- [containsLabelId](campaignserviceselector.md#containslabelid)
- [createdDateRange](campaignserviceselector.md#createddaterange)
- [labelIds](campaignserviceselector.md#labelids)
- [numberResults](campaignserviceselector.md#numberresults)
- [startIndex](campaignserviceselector.md#startindex)
- [userStatuses](campaignserviceselector.md#userstatuses)

## Properties

### accountId

• **accountId**: *number*

<div lang=\"ja\">検索条件：アカウントIDです。</div> 

**`memberof`** CampaignServiceSelector

___

### biddingStrategyIds

• `Optional` **biddingStrategyIds**: ``null`` \| *number*[]

<div lang=\"ja\">検索条件：自動入札IDです。</div> 

**`memberof`** CampaignServiceSelector

___

### campaignIds

• `Optional` **campaignIds**: ``null`` \| *number*[]

<div lang=\"ja\">検索条件：キャンペーンIDです。<br> ※指定しない場合は、フィルタ条件に すべてのキャンペーンが含まれます。</div> 

**`memberof`** CampaignServiceSelector

___

### containsLabelId

• `Optional` **containsLabelId**: ``null`` \| [*True*](./enums/campaignservicecontainslabelid.md#true) \| [*False*](./enums/campaignservicecontainslabelid.md#false) \| [*Unknown*](./enums/campaignservicecontainslabelid.md#unknown)

**`memberof`** CampaignServiceSelector

___

### createdDateRange

• `Optional` **createdDateRange**: ``null`` \| [*CampaignServiceCreatedDateRange*](campaignservicecreateddaterange.md)

**`memberof`** CampaignServiceSelector

___

### labelIds

• `Optional` **labelIds**: ``null`` \| *number*[]

<div lang=\"ja\">検索条件：ラベルIDです。</div> 

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

**`memberof`** CampaignServiceSelector
