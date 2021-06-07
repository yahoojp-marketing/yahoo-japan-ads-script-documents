# PageFeedItemServiceJobStatusSelector


<div lang=\"ja\">PageFeedItemServiceJobStatusSelectorオブジェクトは、upload、downloadの処理状況を取得するための検索条件を格納します。</div> 

## Table of contents

### Properties

- [accountId](pagefeeditemservicejobstatusselector.md#accountid)
- [jobIds](pagefeeditemservicejobstatusselector.md#jobids)
- [jobType](pagefeeditemservicejobstatusselector.md#jobtype)
- [numberResults](pagefeeditemservicejobstatusselector.md#numberresults)
- [startIndex](pagefeeditemservicejobstatusselector.md#startindex)

## Properties

### accountId

• **accountId**: *number*

<div lang=\"ja\">アカウントID</div> 

**`memberof`** PageFeedItemServiceJobStatusSelector

___

### jobIds

• `Optional` **jobIds**: ``null`` \| *number*[]

<div lang=\"ja\">登録したジョブのID</div> 

**`memberof`** PageFeedItemServiceJobStatusSelector

___

### jobType

• **jobType**: ``null`` \| [*Upload*](./enums/pagefeeditemservicejobtype.md#upload) \| [*Download*](./enums/pagefeeditemservicejobtype.md#download) \| [*Unknown*](./enums/pagefeeditemservicejobtype.md#unknown)

**`memberof`** PageFeedItemServiceJobStatusSelector

___

### numberResults

• `Optional` **numberResults**: ``null`` \| *number*

<div lang=\"ja\">ページの最大件数です。このフィールドは、1以上を指定する必要があります。</div> 

**`memberof`** PageFeedItemServiceJobStatusSelector

___

### startIndex

• `Optional` **startIndex**: ``null`` \| *number*

<div lang=\"ja\">ページの先頭のインデックスです。このフィールドは、1以上を指定する必要があります。</div> 

**`memberof`** PageFeedItemServiceJobStatusSelector
