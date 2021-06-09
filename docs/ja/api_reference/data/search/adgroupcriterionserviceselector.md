# AdGroupCriterionServiceSelector


<div lang=\"ja\">AdGroupCriterionServiceSelectorオブジェクトは、操作の対象となる広告グループのクライテリアを表します。</div> 

## Table of contents

### Properties

- [accountId](adgroupcriterionserviceselector.md#accountid)
- [adGroupIds](adgroupcriterionserviceselector.md#adgroupids)
- [approvalStatuses](adgroupcriterionserviceselector.md#approvalstatuses)
- [biddingKeywordCpcRange](adgroupcriterionserviceselector.md#biddingkeywordcpcrange)
- [biddingStrategyIds](adgroupcriterionserviceselector.md#biddingstrategyids)
- [campaignIds](adgroupcriterionserviceselector.md#campaignids)
- [containsLabelId](adgroupcriterionserviceselector.md#containslabelid)
- [criterionIds](adgroupcriterionserviceselector.md#criterionids)
- [keyword](adgroupcriterionserviceselector.md#keyword)
- [labelIds](adgroupcriterionserviceselector.md#labelids)
- [numberResults](adgroupcriterionserviceselector.md#numberresults)
- [startIndex](adgroupcriterionserviceselector.md#startindex)
- [use](adgroupcriterionserviceselector.md#use)
- [userStatuses](adgroupcriterionserviceselector.md#userstatuses)

## Properties

### accountId

• **accountId**: *number*

<div lang=\"ja\">検索条件：アカウントID</div> 

**`memberof`** AdGroupCriterionServiceSelector

___

### adGroupIds

• `Optional` **adGroupIds**: ``null`` \| *number*[]

<div lang=\"ja\">検索条件：広告グループID</div> 

**`memberof`** AdGroupCriterionServiceSelector

___

### approvalStatuses

• `Optional` **approvalStatuses**: ``null`` \| [*AdGroupCriterionServiceApprovalStatus*](./enums/adgroupcriterionserviceapprovalstatus.md)[]

**`memberof`** AdGroupCriterionServiceSelector

___

### biddingKeywordCpcRange

• `Optional` **biddingKeywordCpcRange**: ``null`` \| [*AdGroupCriterionServiceBiddingKeywordCpcRange*](adgroupcriterionservicebiddingkeywordcpcrange.md)

**`memberof`** AdGroupCriterionServiceSelector

___

### biddingStrategyIds

• `Optional` **biddingStrategyIds**: ``null`` \| *number*[]

<div lang=\"ja\">検索条件：自動入札ID</div> 

**`memberof`** AdGroupCriterionServiceSelector

___

### campaignIds

• `Optional` **campaignIds**: ``null`` \| *number*[]

<div lang=\"ja\">検索条件：キャンペーンID</div> 

**`memberof`** AdGroupCriterionServiceSelector

___

### containsLabelId

• `Optional` **containsLabelId**: ``null`` \| [*True*](./enums/adgroupcriterionservicecontainslabelid.md#true) \| [*False*](./enums/adgroupcriterionservicecontainslabelid.md#false) \| [*Unknown*](./enums/adgroupcriterionservicecontainslabelid.md#unknown)

**`memberof`** AdGroupCriterionServiceSelector

___

### criterionIds

• `Optional` **criterionIds**: ``null`` \| *number*[]

<div lang=\"ja\">検索条件：クライテリオンID<br>指定しない場合は、広告グループID以下のすべてのクライ テリアが含まれます。</div> 

**`memberof`** AdGroupCriterionServiceSelector

___

### keyword

• `Optional` **keyword**: ``null`` \| [*AdGroupCriterionServiceKeyword*](adgroupcriterionservicekeyword.md)

**`memberof`** AdGroupCriterionServiceSelector

___

### labelIds

• `Optional` **labelIds**: ``null`` \| *number*[]

<div lang=\"ja\">検索条件：ラベルID</div> 

**`memberof`** AdGroupCriterionServiceSelector

___

### numberResults

• `Optional` **numberResults**: ``null`` \| *number*

<div lang=\"ja\">ページの最大件数です。このフィールドは、1以上を指定する必要があります。</div> 

**`memberof`** AdGroupCriterionServiceSelector

___

### startIndex

• `Optional` **startIndex**: ``null`` \| *number*

<div lang=\"ja\">ページの先頭のインデックスです。このフィールドは、1以上を指定する必要があります。</div> 

**`memberof`** AdGroupCriterionServiceSelector

___

### use

• **use**: ``null`` \| [*Biddable*](./enums/adgroupcriterionserviceuse.md#biddable) \| [*Negative*](./enums/adgroupcriterionserviceuse.md#negative) \| [*Unknown*](./enums/adgroupcriterionserviceuse.md#unknown)

**`memberof`** AdGroupCriterionServiceSelector

___

### userStatuses

• `Optional` **userStatuses**: ``null`` \| [*AdGroupCriterionServiceUserStatus*](./enums/adgroupcriterionserviceuserstatus.md)[]

**`memberof`** AdGroupCriterionServiceSelector
