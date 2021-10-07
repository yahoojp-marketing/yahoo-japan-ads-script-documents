# AdGroupAdServiceSelector


<div lang=\"ja\">AdGroupAdServiceSelectorオブジェクトは、操作の対象とする広告およびフィルタ条件を表します。</div> 

## Table of contents

### Properties

- [accountId](adgroupadserviceselector.md#accountid)
- [adGroupIds](adgroupadserviceselector.md#adgroupids)
- [adIds](adgroupadserviceselector.md#adids)
- [approvalStatuses](adgroupadserviceselector.md#approvalstatuses)
- [campaignIds](adgroupadserviceselector.md#campaignids)
- [containsLabelIdFlg](adgroupadserviceselector.md#containslabelidflg)
- [createdDateRange](adgroupadserviceselector.md#createddaterange)
- [labelIds](adgroupadserviceselector.md#labelids)
- [mediaIds](adgroupadserviceselector.md#mediaids)
- [numberResults](adgroupadserviceselector.md#numberresults)
- [startIndex](adgroupadserviceselector.md#startindex)
- [userStatuses](adgroupadserviceselector.md#userstatuses)

## Properties

### accountId

• **accountId**: *number*

<div lang=\"ja\">検索条件 : アカウント情報</div> 

**`memberof`** AdGroupAdServiceSelector

___

### adGroupIds

• `Optional` **adGroupIds**: ``null`` \| *number*[]

<div lang=\"ja\">検索条件 : 広告グループID</div> 

**`memberof`** AdGroupAdServiceSelector

___

### adIds

• `Optional` **adIds**: ``null`` \| *number*[]

<div lang=\"ja\">検索条件 : 広告ID</div> 

**`memberof`** AdGroupAdServiceSelector

___

### approvalStatuses

• `Optional` **approvalStatuses**: ``null`` \| [*AdGroupAdServiceApprovalStatus*](./enums/adgroupadserviceapprovalstatus.md)[]

**`memberof`** AdGroupAdServiceSelector

___

### campaignIds

• `Optional` **campaignIds**: ``null`` \| *number*[]

<div lang=\"ja\">検索条件 : キャンペーンID</div> 

**`memberof`** AdGroupAdServiceSelector

___

### containsLabelIdFlg

• `Optional` **containsLabelIdFlg**: ``null`` \| *boolean*

<div lang=\"ja\">ラベルID取得フラグ</div> 

**`memberof`** AdGroupAdServiceSelector

___

### createdDateRange

• `Optional` **createdDateRange**: ``null`` \| [*AdGroupAdServiceCreatedDateRange*](adgroupadservicecreateddaterange.md)

**`memberof`** AdGroupAdServiceSelector

___

### labelIds

• `Optional` **labelIds**: ``null`` \| *number*[]

<div lang=\"ja\">検索条件 : ラベルID</div> 

**`memberof`** AdGroupAdServiceSelector

___

### mediaIds

• `Optional` **mediaIds**: ``null`` \| *number*[]

<div lang=\"ja\">検索条件 : 画像ID</div> 

**`memberof`** AdGroupAdServiceSelector

___

### numberResults

• `Optional` **numberResults**: ``null`` \| *number*

<div lang=\"ja\">ページの最大件数です。このフィールドは、1以上を指定する必要があります。</div> 

**`memberof`** AdGroupAdServiceSelector

___

### startIndex

• `Optional` **startIndex**: ``null`` \| *number*

<div lang=\"ja\">ページの先頭のインデックスです。このフィールドは、1以上を指定する必要があります。</div> 

**`memberof`** AdGroupAdServiceSelector

___

### userStatuses

• `Optional` **userStatuses**: ``null`` \| [*AdGroupAdServiceUserStatus*](./enums/adgroupadserviceuserstatus.md)[]

**`memberof`** AdGroupAdServiceSelector
