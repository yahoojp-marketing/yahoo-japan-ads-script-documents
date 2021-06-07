# AuditLogServiceSelector


<div lang=\"ja\">AuditLogServiceSelectorオブジェクトは、登録したジョブを照会するための検索条件を保持します。</div> 

## Table of contents

### Properties

- [accountId](auditlogserviceselector.md#accountid)
- [jobIds](auditlogserviceselector.md#jobids)
- [jobStatuses](auditlogserviceselector.md#jobstatuses)
- [numberResults](auditlogserviceselector.md#numberresults)
- [startIndex](auditlogserviceselector.md#startindex)

## Properties

### accountId

• **accountId**: *number*

<div lang=\"ja\">アカウントIDです。</div> 

**`memberof`** AuditLogServiceSelector

___

### jobIds

• `Optional` **jobIds**: ``null`` \| *number*[]

<div lang=\"ja\">登録したジョブのIDです。</div> 

**`memberof`** AuditLogServiceSelector

___

### jobStatuses

• `Optional` **jobStatuses**: ``null`` \| [*AuditLogServiceJobStatus*](./enums/auditlogservicejobstatus.md)[]

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
