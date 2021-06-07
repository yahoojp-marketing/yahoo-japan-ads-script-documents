# CampaignMigrationServiceJob


<div lang=\"ja\">CampaignMigrationServiceJobオブジェクトは、マイグレーションジョブの処理状況を示すオブジェクトです。</div> 

## Table of contents

### Properties

- [accountId](campaignmigrationservicejob.md#accountid)
- [failedCount](campaignmigrationservicejob.md#failedcount)
- [inProgressCount](campaignmigrationservicejob.md#inprogresscount)
- [jobStatus](campaignmigrationservicejob.md#jobstatus)
- [migrationJobEndDate](campaignmigrationservicejob.md#migrationjobenddate)
- [migrationJobId](campaignmigrationservicejob.md#migrationjobid)
- [migrationJobSubmitDate](campaignmigrationservicejob.md#migrationjobsubmitdate)
- [scope](campaignmigrationservicejob.md#scope)
- [succeededCount](campaignmigrationservicejob.md#succeededcount)
- [totalCount](campaignmigrationservicejob.md#totalcount)

## Properties

### accountId

• `Optional` **accountId**: ``null`` \| *number*

<div lang=\"ja\">アカウントID</div> 

**`memberof`** CampaignMigrationServiceJob

___

### failedCount

• `Optional` **failedCount**: ``null`` \| *number*

<div lang=\"ja\">失敗キャンペーン数</div> 

**`memberof`** CampaignMigrationServiceJob

___

### inProgressCount

• `Optional` **inProgressCount**: ``null`` \| *number*

<div lang=\"ja\">進行中キャンペーン数</div> 

**`memberof`** CampaignMigrationServiceJob

___

### jobStatus

• `Optional` **jobStatus**: ``null`` \| [*NotStarted*](./enums/campaignmigrationservicejobstatus.md#notstarted) \| [*InProgress*](./enums/campaignmigrationservicejobstatus.md#inprogress) \| [*Completed*](./enums/campaignmigrationservicejobstatus.md#completed) \| [*FileFormatError*](./enums/campaignmigrationservicejobstatus.md#fileformaterror) \| [*InvalidCsvValueError*](./enums/campaignmigrationservicejobstatus.md#invalidcsvvalueerror) \| [*UnknownCsvFieldError*](./enums/campaignmigrationservicejobstatus.md#unknowncsvfielderror) \| [*SystemError*](./enums/campaignmigrationservicejobstatus.md#systemerror) \| [*Unknown*](./enums/campaignmigrationservicejobstatus.md#unknown)

**`memberof`** CampaignMigrationServiceJob

___

### migrationJobEndDate

• `Optional` **migrationJobEndDate**: ``null`` \| *string*

<div lang=\"ja\">マイグレーションジョブ終了日時</div> 

**`memberof`** CampaignMigrationServiceJob

___

### migrationJobId

• `Optional` **migrationJobId**: ``null`` \| *number*

<div lang=\"ja\">マイグレーションジョブID</div> 

**`memberof`** CampaignMigrationServiceJob

___

### migrationJobSubmitDate

• `Optional` **migrationJobSubmitDate**: ``null`` \| *string*

<div lang=\"ja\">マイグレーションジョブ登録日時</div> 

**`memberof`** CampaignMigrationServiceJob

___

### scope

• `Optional` **scope**: ``null`` \| [*SingleAccount*](./enums/campaignmigrationservicescope.md#singleaccount) \| [*AllAccount*](./enums/campaignmigrationservicescope.md#allaccount) \| [*Unknown*](./enums/campaignmigrationservicescope.md#unknown)

**`memberof`** CampaignMigrationServiceJob

___

### succeededCount

• `Optional` **succeededCount**: ``null`` \| *number*

<div lang=\"ja\">正常終了キャンペーン数</div> 

**`memberof`** CampaignMigrationServiceJob

___

### totalCount

• `Optional` **totalCount**: ``null`` \| *number*

<div lang=\"ja\">全キャンペーン数</div> 

**`memberof`** CampaignMigrationServiceJob
