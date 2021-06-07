# RetargetingListServiceUploadUserListJob


<div lang=\"ja\">RetargetingListServiceUploadUserListJobオブジェクトは、ユーザーリストのアップロードジョブの処理状況を示すオブジェクトです。</div> 

## Table of contents

### Properties

- [jobStatus](retargetinglistserviceuploaduserlistjob.md#jobstatus)
- [receivedDate](retargetinglistserviceuploaduserlistjob.md#receiveddate)
- [retargetingTagId](retargetinglistserviceuploaduserlistjob.md#retargetingtagid)
- [targetListId](retargetinglistserviceuploaduserlistjob.md#targetlistid)
- [uploadJobId](retargetinglistserviceuploaduserlistjob.md#uploadjobid)
- [uploadSubmitDate](retargetinglistserviceuploaduserlistjob.md#uploadsubmitdate)
- [uploadType](retargetinglistserviceuploaduserlistjob.md#uploadtype)

## Properties

### jobStatus

• `Optional` **jobStatus**: ``null`` \| [*Receiving*](./enums/retargetinglistservicejobstatus.md#receiving) \| [*Received*](./enums/retargetinglistservicejobstatus.md#received) \| [*InvalidFile*](./enums/retargetinglistservicejobstatus.md#invalidfile) \| [*Failed*](./enums/retargetinglistservicejobstatus.md#failed) \| [*Unknown*](./enums/retargetinglistservicejobstatus.md#unknown)

**`memberof`** RetargetingListServiceUploadUserListJob

___

### receivedDate

• `Optional` **receivedDate**: ``null`` \| *string*

<div lang=\"ja\">アップロード受付完了日時</div>  <br>Format: yyyyMMddHHmmss

**`memberof`** RetargetingListServiceUploadUserListJob

___

### retargetingTagId

• `Optional` **retargetingTagId**: ``null`` \| *string*

<div lang=\"ja\">サイトリターゲティングのタグIDです。</div> 

**`memberof`** RetargetingListServiceUploadUserListJob

___

### targetListId

• `Optional` **targetListId**: ``null`` \| *number*

<div lang=\"ja\">カスタムオーディエンスのターゲットリストIDです。</div> 

**`memberof`** RetargetingListServiceUploadUserListJob

___

### uploadJobId

• `Optional` **uploadJobId**: ``null`` \| *string*

<div lang=\"ja\">アップロードジョブIDです。</div> 

**`memberof`** RetargetingListServiceUploadUserListJob

___

### uploadSubmitDate

• `Optional` **uploadSubmitDate**: ``null`` \| *string*

<div lang=\"ja\">アップロード日時</div>  <br>Format: yyyyMMddHHmmss

**`memberof`** RetargetingListServiceUploadUserListJob

___

### uploadType

• `Optional` **uploadType**: ``null`` \| [*Idfa*](./enums/retargetinglistserviceuploaduserlistuploadtype.md#idfa) \| [*Aaid*](./enums/retargetinglistserviceuploaduserlistuploadtype.md#aaid) \| [*MailAddress*](./enums/retargetinglistserviceuploaduserlistuploadtype.md#mailaddress) \| [*Userid*](./enums/retargetinglistserviceuploaduserlistuploadtype.md#userid) \| [*Unknown*](./enums/retargetinglistserviceuploaduserlistuploadtype.md#unknown)

**`memberof`** RetargetingListServiceUploadUserListJob
