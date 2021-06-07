# PageFeedItemServiceUploadJob


<div lang=\"ja\">PageFeedItemServiceUploadJobオブジェクトは、ページフィードアイテム情報をダウンロードする処理内容を格納します。</div> 

## Table of contents

### Properties

- [accountId](pagefeeditemserviceuploadjob.md#accountid)
- [endDate](pagefeeditemserviceuploadjob.md#enddate)
- [errorCount](pagefeeditemserviceuploadjob.md#errorcount)
- [feedIds](pagefeeditemserviceuploadjob.md#feedids)
- [jobId](pagefeeditemserviceuploadjob.md#jobid)
- [progress](pagefeeditemserviceuploadjob.md#progress)
- [startDate](pagefeeditemserviceuploadjob.md#startdate)
- [uploadJobStatus](pagefeeditemserviceuploadjob.md#uploadjobstatus)

## Properties

### accountId

• `Optional` **accountId**: ``null`` \| *number*

<div lang=\"ja\">アカウントID</div> 

**`memberof`** PageFeedItemServiceUploadJob

___

### endDate

• `Optional` **endDate**: ``null`` \| *string*

<div lang=\"ja\">ジョブの終了日<br> 形式：yyyyMMddHHmmss</div> 

**`memberof`** PageFeedItemServiceUploadJob

___

### errorCount

• `Optional` **errorCount**: ``null`` \| *number*

<div lang=\"ja\">エラーの件数</div> 

**`memberof`** PageFeedItemServiceUploadJob

___

### feedIds

• `Optional` **feedIds**: ``null`` \| *number*[]

**`memberof`** PageFeedItemServiceUploadJob

___

### jobId

• `Optional` **jobId**: ``null`` \| *number*

<div lang=\"ja\">ジョブID</div> 

**`memberof`** PageFeedItemServiceUploadJob

___

### progress

• `Optional` **progress**: ``null`` \| *number*

<div lang=\"ja\">ジョブの進捗状況</div> 

**`memberof`** PageFeedItemServiceUploadJob

___

### startDate

• `Optional` **startDate**: ``null`` \| *string*

<div lang=\"ja\">ジョブの開始日<br> 形式：yyyyMMddHHmmss</div> 

**`memberof`** PageFeedItemServiceUploadJob

___

### uploadJobStatus

• `Optional` **uploadJobStatus**: ``null`` \| [*InProgress*](./enums/pagefeeditemserviceuploadjobstatus.md#inprogress) \| [*Completed*](./enums/pagefeeditemserviceuploadjobstatus.md#completed) \| [*CompletedWithValidationError*](./enums/pagefeeditemserviceuploadjobstatus.md#completedwithvalidationerror) \| [*FileFormatError*](./enums/pagefeeditemserviceuploadjobstatus.md#fileformaterror) \| [*FileEncodingError*](./enums/pagefeeditemserviceuploadjobstatus.md#fileencodingerror) \| [*ColumnHeaderError*](./enums/pagefeeditemserviceuploadjobstatus.md#columnheadererror) \| [*ExceedRowLines*](./enums/pagefeeditemserviceuploadjobstatus.md#exceedrowlines) \| [*ExceedFileCounts*](./enums/pagefeeditemserviceuploadjobstatus.md#exceedfilecounts) \| [*InvalidFeedId*](./enums/pagefeeditemserviceuploadjobstatus.md#invalidfeedid) \| [*Timeout*](./enums/pagefeeditemserviceuploadjobstatus.md#timeout) \| [*SystemError*](./enums/pagefeeditemserviceuploadjobstatus.md#systemerror) \| [*Unknown*](./enums/pagefeeditemserviceuploadjobstatus.md#unknown)

**`memberof`** PageFeedItemServiceUploadJob
