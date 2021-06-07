# AuditLogServiceJob


<div lang=\"ja\">AuditLogServiceJobは操作履歴のダウンロードジョブの情報を保持するオブジェクトです。</div> 

## Table of contents

### Properties

- [accountId](auditlogservicejob.md#accountid)
- [auditLogJobEndDate](auditlogservicejob.md#auditlogjobenddate)
- [auditLogJobId](auditlogservicejob.md#auditlogjobid)
- [auditLogJobName](auditlogservicejob.md#auditlogjobname)
- [auditLogJobStartDate](auditlogservicejob.md#auditlogjobstartdate)
- [auditLogJobUserName](auditlogservicejob.md#auditlogjobusername)
- [campaignIds](auditlogservicejob.md#campaignids)
- [dateRange](auditlogservicejob.md#daterange)
- [jobStatus](auditlogservicejob.md#jobstatus)
- [lang](auditlogservicejob.md#lang)
- [progress](auditlogservicejob.md#progress)
- [updateSource](auditlogservicejob.md#updatesource)

## Properties

### accountId

• `Optional` **accountId**: ``null`` \| *number*

<div lang=\"ja\"> アカウントIDです。<br> このフィールドは、レスポンスの際に返却されますが、リクエストの際には無視されます。 </div> 

**`memberof`** AuditLogServiceJob

___

### auditLogJobEndDate

• `Optional` **auditLogJobEndDate**: ``null`` \| *string*

<div lang=\"ja\"> 操作履歴ダウンロードジョブの終了日時です。<br> このフィールドは、レスポンスの際に返却されますが、リクエストの際には無視されます。 </div> 

**`memberof`** AuditLogServiceJob

___

### auditLogJobId

• `Optional` **auditLogJobId**: ``null`` \| *number*

<div lang=\"ja\"> 操作履歴のダウンロードジョブIDです。<br> このフィールドは、レスポンスの際に返却されますが、リクエストの際には無視されます。 </div> 

**`memberof`** AuditLogServiceJob

___

### auditLogJobName

• `Optional` **auditLogJobName**: ``null`` \| *string*

<div lang=\"ja\"> 操作履歴のダウンロードジョブ名です。<br> このフィールドは、リクエストの場合は省略可能となります。 </div> 

**`memberof`** AuditLogServiceJob

___

### auditLogJobStartDate

• `Optional` **auditLogJobStartDate**: ``null`` \| *string*

<div lang=\"ja\"> 操作履歴ダウンロードジョブの開始日時です。<br> このフィールドは、レスポンスの際に返却されますが、リクエストの際には無視されます。 </div> 

**`memberof`** AuditLogServiceJob

___

### auditLogJobUserName

• `Optional` **auditLogJobUserName**: ``null`` \| *string*

<div lang=\"ja\"> 操作履歴ダウンロードジョブの実行ユーザー名です。<br> このフィールドは、レスポンスの際に返却されますが、リクエストの際には無視されます。 </div> 

**`memberof`** AuditLogServiceJob

___

### campaignIds

• `Optional` **campaignIds**: ``null`` \| *number*[]

<div lang=\"ja\"> ダウンロード対象のキャンペーンIDです。<br> このフィールドは、リクエストの場合は省略可能となります。 </div> 

**`memberof`** AuditLogServiceJob

___

### dateRange

• `Optional` **dateRange**: ``null`` \| [*AuditLogServiceDateRange*](auditlogservicedaterange.md)

**`memberof`** AuditLogServiceJob

___

### jobStatus

• `Optional` **jobStatus**: ``null`` \| [*InProgress*](./enums/auditlogservicejobstatus.md#inprogress) \| [*Completed*](./enums/auditlogservicejobstatus.md#completed) \| [*SystemError*](./enums/auditlogservicejobstatus.md#systemerror) \| [*Unknown*](./enums/auditlogservicejobstatus.md#unknown)

**`memberof`** AuditLogServiceJob

___

### lang

• `Optional` **lang**: ``null`` \| [*Ja*](./enums/auditlogservicelang.md#ja) \| [*En*](./enums/auditlogservicelang.md#en) \| [*Unknown*](./enums/auditlogservicelang.md#unknown)

**`memberof`** AuditLogServiceJob

___

### progress

• `Optional` **progress**: ``null`` \| *number*

<div lang=\"ja\"> 処理進捗です。<br> このフィールドは、レスポンスの際に返却されますが、リクエストの際には無視されます。 </div> 

**`memberof`** AuditLogServiceJob

___

### updateSource

• `Optional` **updateSource**: ``null`` \| [*CampaignManagementTool*](./enums/auditlogserviceupdatesource.md#campaignmanagementtool) \| [*Api*](./enums/auditlogserviceupdatesource.md#api) \| [*All*](./enums/auditlogserviceupdatesource.md#all) \| [*Unknown*](./enums/auditlogserviceupdatesource.md#unknown)

**`memberof`** AuditLogServiceJob
