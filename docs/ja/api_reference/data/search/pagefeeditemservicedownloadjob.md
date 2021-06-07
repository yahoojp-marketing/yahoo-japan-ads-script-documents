# PageFeedItemServiceDownloadJob


<div lang=\"ja\">PageFeedItemServiceDownloadJobオブジェクトは、ページフィードアイテム情報をダウンロードする処理内容を格納します。</div> 

## Table of contents

### Properties

- [accountId](pagefeeditemservicedownloadjob.md#accountid)
- [bulkEncoding](pagefeeditemservicedownloadjob.md#bulkencoding)
- [bulkLang](pagefeeditemservicedownloadjob.md#bulklang)
- [bulkOutput](pagefeeditemservicedownloadjob.md#bulkoutput)
- [downloadJobStatus](pagefeeditemservicedownloadjob.md#downloadjobstatus)
- [endDate](pagefeeditemservicedownloadjob.md#enddate)
- [feedId](pagefeeditemservicedownloadjob.md#feedid)
- [jobId](pagefeeditemservicedownloadjob.md#jobid)
- [progress](pagefeeditemservicedownloadjob.md#progress)
- [startDate](pagefeeditemservicedownloadjob.md#startdate)

## Properties

### accountId

• `Optional` **accountId**: ``null`` \| *number*

<div lang=\"ja\">アカウントIDです。<br> このフィールドは必須です。</div> 

**`memberof`** PageFeedItemServiceDownloadJob

___

### bulkEncoding

• `Optional` **bulkEncoding**: ``null`` \| [*Sjis*](./enums/pagefeeditemservicebulkencoding.md#sjis) \| [*Utf8*](./enums/pagefeeditemservicebulkencoding.md#utf8) \| [*Utf16Le*](./enums/pagefeeditemservicebulkencoding.md#utf16le) \| [*Unknown*](./enums/pagefeeditemservicebulkencoding.md#unknown)

**`memberof`** PageFeedItemServiceDownloadJob

___

### bulkLang

• `Optional` **bulkLang**: ``null`` \| [*Ja*](./enums/pagefeeditemservicebulklang.md#ja) \| [*En*](./enums/pagefeeditemservicebulklang.md#en) \| [*Unknown*](./enums/pagefeeditemservicebulklang.md#unknown)

**`memberof`** PageFeedItemServiceDownloadJob

___

### bulkOutput

• `Optional` **bulkOutput**: ``null`` \| [*Csv*](./enums/pagefeeditemservicebulkoutput.md#csv) \| [*Tsv*](./enums/pagefeeditemservicebulkoutput.md#tsv) \| [*ZippedCsv*](./enums/pagefeeditemservicebulkoutput.md#zippedcsv) \| [*ZippedTsv*](./enums/pagefeeditemservicebulkoutput.md#zippedtsv) \| [*Unknown*](./enums/pagefeeditemservicebulkoutput.md#unknown)

**`memberof`** PageFeedItemServiceDownloadJob

___

### downloadJobStatus

• `Optional` **downloadJobStatus**: ``null`` \| [*InProgress*](./enums/pagefeeditemservicedownloadjobstatus.md#inprogress) \| [*Completed*](./enums/pagefeeditemservicedownloadjobstatus.md#completed) \| [*FieldsError*](./enums/pagefeeditemservicedownloadjobstatus.md#fieldserror) \| [*Timeout*](./enums/pagefeeditemservicedownloadjobstatus.md#timeout) \| [*SystemError*](./enums/pagefeeditemservicedownloadjobstatus.md#systemerror) \| [*Unknown*](./enums/pagefeeditemservicedownloadjobstatus.md#unknown)

**`memberof`** PageFeedItemServiceDownloadJob

___

### endDate

• `Optional` **endDate**: ``null`` \| *string*

<div lang=\"ja\">ジョブの終了日です。<br> このフィールドは、レスポンスの際に返却されますが、リクエストの際には無視されます。<br> 形式：yyyyMMddHHmmss</div>

**`memberof`** PageFeedItemServiceDownloadJob

___

### feedId

• `Optional` **feedId**: ``null`` \| *number*

<div lang=\"ja\">フィードIDです。<br> このフィールドは必須です。</div> 

**`memberof`** PageFeedItemServiceDownloadJob

___

### jobId

• `Optional` **jobId**: ``null`` \| *number*

<div lang=\"ja\">ジョブIDです。<br> このフィールドは、レスポンスの際に返却されますが、リクエストの際には無視されます。</div> 

**`memberof`** PageFeedItemServiceDownloadJob

___

### progress

• `Optional` **progress**: ``null`` \| *number*

<div lang=\"ja\">ジョブの進捗状況です。<br> このフィールドは、レスポンスの際に返却されますが、リクエストの際には無視されます。</div> 

**`memberof`** PageFeedItemServiceDownloadJob

___

### startDate

• `Optional` **startDate**: ``null`` \| *string*

<div lang=\"ja\">ジョブの開始日です。<br>このフィールドは、レスポンスの際に返却されますが、リクエストの際には無視されます。 <br> 形式：yyyyMMddHHmmss </div> 

**`memberof`** PageFeedItemServiceDownloadJob
