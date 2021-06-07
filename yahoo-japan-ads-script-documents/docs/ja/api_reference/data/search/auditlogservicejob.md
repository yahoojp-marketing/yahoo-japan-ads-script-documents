# AuditLogServiceJob


<div lang=\"ja\">AuditLogServiceJobオブジェクトは、操作履歴取得で登録するジョブの情報を保持します。</div> 

## Table of contents

### Properties

- [accountId](auditlogservicejob.md#accountid)
- [dateRange](auditlogservicejob.md#daterange)
- [encoding](auditlogservicejob.md#encoding)
- [eventSelector](auditlogservicejob.md#eventselector)
- [jobId](auditlogservicejob.md#jobid)
- [jobName](auditlogservicejob.md#jobname)
- [jobStatus](auditlogservicejob.md#jobstatus)
- [lang](auditlogservicejob.md#lang)
- [output](auditlogservicejob.md#output)
- [sourceType](auditlogservicejob.md#sourcetype)

## Properties

### accountId

• `Optional` **accountId**: ``null`` \| *number*

<div lang=\"ja\">アカウントIDです。<br>このフィールドは、レスポンスの際に返却されますが、リクエストの際には無視されます。</div> 

**`memberof`** AuditLogServiceJob

___

### dateRange

• `Optional` **dateRange**: ``null`` \| [*AuditLogServiceDateRange*](auditlogservicedaterange.md)

**`memberof`** AuditLogServiceJob

___

### encoding

• `Optional` **encoding**: ``null`` \| [*Sjis*](./enums/auditlogserviceencoding.md#sjis) \| [*Utf8*](./enums/auditlogserviceencoding.md#utf8) \| [*Utf16Le*](./enums/auditlogserviceencoding.md#utf16le) \| [*Unknown*](./enums/auditlogserviceencoding.md#unknown)

**`memberof`** AuditLogServiceJob

___

### eventSelector

• **eventSelector**: ``null`` \| [*AuditLogServiceEventSelector*](auditlogserviceeventselector.md)[]

**`memberof`** AuditLogServiceJob

___

### jobId

• `Optional` **jobId**: ``null`` \| *number*

<div lang=\"ja\">ジョブIDです。<br>このフィールドは、レスポンスの際に返却されますが、リクエストの際には無視されます。</div> 

**`memberof`** AuditLogServiceJob

___

### jobName

• `Optional` **jobName**: ``null`` \| *string*

<div lang=\"ja\">ジョブ名です。<br>このフィールドは、省略可能となります。</div> 

**`memberof`** AuditLogServiceJob

___

### jobStatus

• `Optional` **jobStatus**: ``null`` \| [*InProgress*](./enums/auditlogservicejobstatus.md#inprogress) \| [*Completed*](./enums/auditlogservicejobstatus.md#completed) \| [*Timeout*](./enums/auditlogservicejobstatus.md#timeout) \| [*SystemError*](./enums/auditlogservicejobstatus.md#systemerror) \| [*Unknown*](./enums/auditlogservicejobstatus.md#unknown)

**`memberof`** AuditLogServiceJob

___

### lang

• `Optional` **lang**: ``null`` \| [*Ja*](./enums/auditlogservicelang.md#ja) \| [*En*](./enums/auditlogservicelang.md#en) \| [*Unknown*](./enums/auditlogservicelang.md#unknown)

**`memberof`** AuditLogServiceJob

___

### output

• `Optional` **output**: ``null`` \| [*Csv*](./enums/auditlogserviceoutput.md#csv) \| [*Tsv*](./enums/auditlogserviceoutput.md#tsv) \| [*ZippedCsv*](./enums/auditlogserviceoutput.md#zippedcsv) \| [*ZippedTsv*](./enums/auditlogserviceoutput.md#zippedtsv) \| [*Unknown*](./enums/auditlogserviceoutput.md#unknown)

**`memberof`** AuditLogServiceJob

___

### sourceType

• `Optional` **sourceType**: ``null`` \| [*Api*](./enums/auditlogservicesourcetype.md#api) \| [*YahooJapan*](./enums/auditlogservicesourcetype.md#yahoojapan) \| [*CampaignManagementTool*](./enums/auditlogservicesourcetype.md#campaignmanagementtool) \| [*All*](./enums/auditlogservicesourcetype.md#all) \| [*Unknown*](./enums/auditlogservicesourcetype.md#unknown)

**`memberof`** AuditLogServiceJob
