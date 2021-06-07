# Enumeration: AuditLogServiceJobStatus


<div lang=\"ja\">AuditLogServiceJobStatusは、操作履歴取得ジョブの実行状況を表します。<br> このフィールドは、job配下ではレスポンスの際に返却されますが、リクエストの際には無視されます。</div>  <dl class=term>   <dt class=\"term__item\">SYSTEM_ERROR</dt>   <dd class=\"term__desc\"><span lang=\"ja\">エラーです。</span></dd>   <dt class=\"term__item\">IN_PROGRESS</dt>   <dd class=\"term__desc\"><span lang=\"ja\">処理中です。</span></dd>   <dt class=\"term__item\">COMPLETED</dt>   <dd class=\"term__desc\"><span lang=\"ja\">処理完了です。</span></dd>   <dt class=\"term__item\">TIMEOUT</dt>   <dd class=\"term__desc\"><span lang=\"ja\">タイムアウトです。</span></dd>   <dt class=\"term__item\">UNKNOWN</dt>   <dd class=\"term__desc\"><span lang=\"ja\">未知の値です。</span></dd> </dl>

## Table of contents

### Enumeration members

- [Completed](auditlogservicejobstatus.md#completed)
- [InProgress](auditlogservicejobstatus.md#inprogress)
- [SystemError](auditlogservicejobstatus.md#systemerror)
- [Timeout](auditlogservicejobstatus.md#timeout)
- [Unknown](auditlogservicejobstatus.md#unknown)

## Enumeration members

### Completed

• **Completed**: = "COMPLETED"

___

### InProgress

• **InProgress**: = "IN\_PROGRESS"

___

### SystemError

• **SystemError**: = "SYSTEM\_ERROR"

___

### Timeout

• **Timeout**: = "TIMEOUT"

___

### Unknown

• **Unknown**: = "UNKNOWN"
