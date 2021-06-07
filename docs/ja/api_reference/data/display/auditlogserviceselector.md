# AuditLogServiceSelector


<div lang=\"ja\">getメソッドの検索条件（実行パラメータ）を保持するオブジェクトです。</div> 

## Table of contents

### Properties

- [accountId](auditlogserviceselector.md#accountid)
- [auditLogJobIds](auditlogserviceselector.md#auditlogjobids)
- [jobStatuses](auditlogserviceselector.md#jobstatuses)
- [numberResults](auditlogserviceselector.md#numberresults)
- [startIndex](auditlogserviceselector.md#startindex)

## Properties

### accountId

• **accountId**: *number*

<div lang=\"ja\">アカウントIDです。</div> 

**`memberof`** AuditLogServiceSelector

___

### auditLogJobIds

• `Optional` **auditLogJobIds**: ``null`` \| *number*[]

<div lang=\"ja\">ジョブIDです。</div> 

**`memberof`** AuditLogServiceSelector

___

### jobStatuses

• `Optional` **jobStatuses**: ``null`` \| [*AuditLogServiceJobStatus*](./enums/auditlogservicejobstatus.md)[]

<div lang=\"ja\">ジョブステータスです。</div> 

**`memberof`** AuditLogServiceSelector

___

### numberResults

• `Optional` **numberResults**: ``null`` \| *number*

<div lang=\"ja\">ページの最大件数です。このフィールドは、1以上を指定する必要があります。</div> 

**`memberof`** AuditLogServiceSelector

___

### startIndex

• `Optional` **startIndex**: ``null`` \| *number*

<div lang=\"ja\">ページの先頭のインデックスです。このフィールドは、1以上を指定する必要があります。</div> 

**`memberof`** AuditLogServiceSelector
