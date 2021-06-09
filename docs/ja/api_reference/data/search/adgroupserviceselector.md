# AdGroupServiceSelector


<div lang=\"ja\">AdGroupServiceSelectorオブジェクトは、指定された広告グループを表します。</div> 

## Table of contents

### Properties

- [accountId](adgroupserviceselector.md#accountid)
- [adGroupIds](adgroupserviceselector.md#adgroupids)
- [biddingKeywordCpcRange](adgroupserviceselector.md#biddingkeywordcpcrange)
- [biddingStrategyIds](adgroupserviceselector.md#biddingstrategyids)
- [campaignIds](adgroupserviceselector.md#campaignids)
- [containsLabelId](adgroupserviceselector.md#containslabelid)
- [createdDateRange](adgroupserviceselector.md#createddaterange)
- [labelIds](adgroupserviceselector.md#labelids)
- [numberResults](adgroupserviceselector.md#numberresults)
- [startIndex](adgroupserviceselector.md#startindex)
- [userStatuses](adgroupserviceselector.md#userstatuses)

## Properties

### accountId

• **accountId**: *number*

<div lang=\"ja\">検索条件：アカウントID</div> 

**`memberof`** AdGroupServiceSelector

___

### adGroupIds

• `Optional` **adGroupIds**: ``null`` \| *number*[]

<div lang=\"ja\">検索条件：広告グループID</div> 

**`memberof`** AdGroupServiceSelector

___

### biddingKeywordCpcRange

• `Optional` **biddingKeywordCpcRange**: ``null`` \| [*AdGroupServiceBiddingKeywordCpcRange*](adgroupservicebiddingkeywordcpcrange.md)

**`memberof`** AdGroupServiceSelector

___

### biddingStrategyIds

• `Optional` **biddingStrategyIds**: ``null`` \| *number*[]

<div lang=\"ja\">検索条件：自動入札ID</div> 

**`memberof`** AdGroupServiceSelector

___

### campaignIds

• `Optional` **campaignIds**: ``null`` \| *number*[]

<div lang=\"ja\">検索条件：キャンペーンID</div> 

**`memberof`** AdGroupServiceSelector

___

### containsLabelId

• `Optional` **containsLabelId**: ``null`` \| [*True*](./enums/adgroupservicecontainslabelid.md#true) \| [*False*](./enums/adgroupservicecontainslabelid.md#false) \| [*Unknown*](./enums/adgroupservicecontainslabelid.md#unknown)

**`memberof`** AdGroupServiceSelector

___

### createdDateRange

• `Optional` **createdDateRange**: ``null`` \| [*AdGroupServiceCreatedDateRange*](adgroupservicecreateddaterange.md)

**`memberof`** AdGroupServiceSelector

___

### labelIds

• `Optional` **labelIds**: ``null`` \| *number*[]

<div lang=\"ja\">検索条件：ラベルID</div> 

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
