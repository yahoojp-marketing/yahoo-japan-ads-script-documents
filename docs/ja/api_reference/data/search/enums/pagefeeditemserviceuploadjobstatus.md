# Enumeration: PageFeedItemServiceUploadJobStatus


<div lang=\"ja\">PageFeedItemServiceUploadJobStatusは、ページフィードアイテムアップロードジョブの実行状況を表します。</div>  <dl class=term>   <dt class=\"term__item\">IN_PROGRESS</dt>   <dd class=\"term__desc\"><span lang=\"ja\">処理中</span></dd>   <dt class=\"term__item\">COMPLETED</dt>   <dd class=\"term__desc\"><span lang=\"ja\">処理完了</span></dd>   <dt class=\"term__item\">COMPLETED_WITH_VALIDATION_ERROR</dt>   <dd class=\"term__desc\"><span lang=\"ja\">ファイル内の入力値が不正</span></dd>   <dt class=\"term__item\">FILE_FORMAT_ERROR</dt>   <dd class=\"term__desc\"><span lang=\"ja\">ファイルのフォーマットが不正</span></dd>   <dt class=\"term__item\">FILE_ENCODING_ERROR</dt>   <dd class=\"term__desc\"><span lang=\"ja\">ファイルのエンコードが不正</span></dd>   <dt class=\"term__item\">COLUMN_HEADER_ERROR</dt>   <dd class=\"term__desc\"><span lang=\"ja\">ファイルのヘッダーが不正</span></dd>   <dt class=\"term__item\">EXCEED_ROW_LINES</dt>   <dd class=\"term__desc\"><span lang=\"ja\">ファイルの最大行数が超過しています。</span></dd>   <dt class=\"term__item\">EXCEED_FILE_COUNTS</dt>   <dd class=\"term__desc\"><span lang=\"ja\">複数のファイルを圧縮しているためエラー</span></dd>   <dt class=\"term__item\">INVALID_FEED_ID</dt>   <dd class=\"term__desc\"><span lang=\"ja\">フィードIDが不正</span></dd>   <dt class=\"term__item\">TIMEOUT</dt>   <dd class=\"term__desc\"><span lang=\"ja\">タイムアウト</span></dd>   <dt class=\"term__item\">SYSTEM_ERROR</dt>   <dd class=\"term__desc\"><span lang=\"ja\">エラー</span></dd>   <dt class=\"term__item\">UNKNOWN</dt>   <dd class=\"term__desc\"><span lang=\"ja\">未知の値です。</span></dd> </dl>

## Table of contents

### Enumeration members

- [ColumnHeaderError](pagefeeditemserviceuploadjobstatus.md#columnheadererror)
- [Completed](pagefeeditemserviceuploadjobstatus.md#completed)
- [CompletedWithValidationError](pagefeeditemserviceuploadjobstatus.md#completedwithvalidationerror)
- [ExceedFileCounts](pagefeeditemserviceuploadjobstatus.md#exceedfilecounts)
- [ExceedRowLines](pagefeeditemserviceuploadjobstatus.md#exceedrowlines)
- [FileEncodingError](pagefeeditemserviceuploadjobstatus.md#fileencodingerror)
- [FileFormatError](pagefeeditemserviceuploadjobstatus.md#fileformaterror)
- [InProgress](pagefeeditemserviceuploadjobstatus.md#inprogress)
- [InvalidFeedId](pagefeeditemserviceuploadjobstatus.md#invalidfeedid)
- [SystemError](pagefeeditemserviceuploadjobstatus.md#systemerror)
- [Timeout](pagefeeditemserviceuploadjobstatus.md#timeout)
- [Unknown](pagefeeditemserviceuploadjobstatus.md#unknown)

## Enumeration members

### ColumnHeaderError

• **ColumnHeaderError**: = "COLUMN\_HEADER\_ERROR"

___

### Completed

• **Completed**: = "COMPLETED"

___

### CompletedWithValidationError

• **CompletedWithValidationError**: = "COMPLETED\_WITH\_VALIDATION\_ERROR"

___

### ExceedFileCounts

• **ExceedFileCounts**: = "EXCEED\_FILE\_COUNTS"

___

### ExceedRowLines

• **ExceedRowLines**: = "EXCEED\_ROW\_LINES"

___

### FileEncodingError

• **FileEncodingError**: = "FILE\_ENCODING\_ERROR"

___

### FileFormatError

• **FileFormatError**: = "FILE\_FORMAT\_ERROR"

___

### InProgress

• **InProgress**: = "IN\_PROGRESS"

___

### InvalidFeedId

• **InvalidFeedId**: = "INVALID\_FEED\_ID"

___

### SystemError

• **SystemError**: = "SYSTEM\_ERROR"

___

### Timeout

• **Timeout**: = "TIMEOUT"

___

### Unknown

• **Unknown**: = "UNKNOWN"
