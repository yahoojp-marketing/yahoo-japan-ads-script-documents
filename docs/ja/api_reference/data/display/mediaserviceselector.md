# MediaServiceSelector


<div lang=\"ja\">MediaServiceSelectorオブジェクトは、操作の対象とする画像およびフィルタ条件を表します。</div> 

## Table of contents

### Properties

- [accountId](mediaserviceselector.md#accountid)
- [approvalStatuses](mediaserviceselector.md#approvalstatuses)
- [createdDateRange](mediaserviceselector.md#createddaterange)
- [mediaIds](mediaserviceselector.md#mediaids)
- [numberResults](mediaserviceselector.md#numberresults)
- [startIndex](mediaserviceselector.md#startindex)
- [userStatuses](mediaserviceselector.md#userstatuses)

## Properties

### accountId

• **accountId**: *number*

<div lang=\"ja\">アカウントIDです。</div> 

**`memberof`** MediaServiceSelector

___

### approvalStatuses

• `Optional` **approvalStatuses**: ``null`` \| [*MediaServiceApprovalStatus*](./enums/mediaserviceapprovalstatus.md)[]

**`memberof`** MediaServiceSelector

___

### createdDateRange

• `Optional` **createdDateRange**: ``null`` \| [*MediaServiceCreatedDateRange*](mediaservicecreateddaterange.md)

**`memberof`** MediaServiceSelector

___

### mediaIds

• `Optional` **mediaIds**: ``null`` \| *number*[]

<div lang=\"ja\">画像IDです。</div> 

**`memberof`** MediaServiceSelector

___

### numberResults

• `Optional` **numberResults**: ``null`` \| *number*

<div lang=\"ja\">ページの最大件数です。このフィールドは、1以上を指定する必要があります。</div> 

**`memberof`** MediaServiceSelector

___

### startIndex

• `Optional` **startIndex**: ``null`` \| *number*

<div lang=\"ja\">ページの先頭のインデックスです。このフィールドは、1以上を指定する必要があります。</div> 

**`memberof`** MediaServiceSelector

___

### userStatuses

• `Optional` **userStatuses**: ``null`` \| [*MediaServiceUserStatus*](./enums/mediaserviceuserstatus.md)[]

**`memberof`** MediaServiceSelector
