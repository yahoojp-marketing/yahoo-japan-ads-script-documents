# VideoServiceSelector


<div lang=\"ja\">VideoServiceSelectorオブジェクトは、入稿済みの動画の情報を取得します。</div> 

## Table of contents

### Properties

- [accountId](videoserviceselector.md#accountid)
- [approvalStatuses](videoserviceselector.md#approvalstatuses)
- [createdDateRange](videoserviceselector.md#createddaterange)
- [mediaIds](videoserviceselector.md#mediaids)
- [numberResults](videoserviceselector.md#numberresults)
- [processStatuses](videoserviceselector.md#processstatuses)
- [startIndex](videoserviceselector.md#startindex)
- [userStatuses](videoserviceselector.md#userstatuses)

## Properties

### accountId

• **accountId**: *number*

<div lang=\"ja\">アカウントIDです。</div> 

**`memberof`** VideoServiceSelector

___

### approvalStatuses

• `Optional` **approvalStatuses**: ``null`` \| [*VideoServiceApprovalStatus*](./enums/videoserviceapprovalstatus.md)[]

**`memberof`** VideoServiceSelector

___

### createdDateRange

• `Optional` **createdDateRange**: ``null`` \| [*VideoServiceCreatedDateRange*](videoservicecreateddaterange.md)

**`memberof`** VideoServiceSelector

___

### mediaIds

• `Optional` **mediaIds**: ``null`` \| *number*[]

<div lang=\"ja\">メディアIDです。</div> 

**`memberof`** VideoServiceSelector

___

### numberResults

• `Optional` **numberResults**: ``null`` \| *number*

<div lang=\"ja\">ページの最大件数です。このフィールドは、1以上を指定する必要があります。</div> 

**`memberof`** VideoServiceSelector

___

### processStatuses

• `Optional` **processStatuses**: ``null`` \| [*VideoServiceProcessStatus*](./enums/videoserviceprocessstatus.md)[]

**`memberof`** VideoServiceSelector

___

### startIndex

• `Optional` **startIndex**: ``null`` \| *number*

<div lang=\"ja\">ページの先頭のインデックスです。このフィールドは、1以上を指定する必要があります。</div> 

**`memberof`** VideoServiceSelector

___

### userStatuses

• `Optional` **userStatuses**: ``null`` \| [*VideoServiceUserStatus*](./enums/videoserviceuserstatus.md)[]

**`memberof`** VideoServiceSelector
