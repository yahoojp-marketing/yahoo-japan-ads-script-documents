# FeedDataServiceSelector


<div lang=\"ja\">get操作の検索条件を保持するオブジェクト</div> 

## Table of contents

### Properties

- [accountId](feeddataserviceselector.md#accountid)
- [feedIds](feeddataserviceselector.md#feedids)
- [fileUploadDateRange](feeddataserviceselector.md#fileuploaddaterange)
- [itemListUploadIds](feeddataserviceselector.md#itemlistuploadids)
- [numberResults](feeddataserviceselector.md#numberresults)
- [startIndex](feeddataserviceselector.md#startindex)
- [uploadStatuses](feeddataserviceselector.md#uploadstatuses)

## Properties

### accountId

• **accountId**: *number*

<div lang=\"ja\">アカウントID</div> 

**`memberof`** FeedDataServiceSelector

___

### feedIds

• `Optional` **feedIds**: ``null`` \| *number*[]

<div lang=\"ja\">フィードID</div> 

**`memberof`** FeedDataServiceSelector

___

### fileUploadDateRange

• `Optional` **fileUploadDateRange**: ``null`` \| [*FeedDataServiceFileUploadDateRange*](feeddataservicefileuploaddaterange.md)

**`memberof`** FeedDataServiceSelector

___

### itemListUploadIds

• `Optional` **itemListUploadIds**: ``null`` \| *number*[]

<div lang=\"ja\">アップロードした商品情報ID</div> 

**`memberof`** FeedDataServiceSelector

___

### numberResults

• `Optional` **numberResults**: ``null`` \| *number*

<div lang=\"ja\">ページの最大件数です。このフィールドは、1以上を指定する必要があります。</div> 

**`memberof`** FeedDataServiceSelector

___

### startIndex

• `Optional` **startIndex**: ``null`` \| *number*

<div lang=\"ja\">ページの先頭のインデックスです。このフィールドは、1以上を指定する必要があります。</div> 

**`memberof`** FeedDataServiceSelector

___

### uploadStatuses

• `Optional` **uploadStatuses**: ``null`` \| [*FeedDataServiceFileUploadStatus*](./enums/feeddataservicefileuploadstatus.md)[]

**`memberof`** FeedDataServiceSelector
