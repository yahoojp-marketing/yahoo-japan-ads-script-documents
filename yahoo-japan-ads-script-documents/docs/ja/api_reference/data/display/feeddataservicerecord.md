# FeedDataServiceRecord


<div lang=\"ja\">FeedDataServiceRecordオブジェクトは、アップロードした商品情報(ファイル形式)の状態を保持する。</div> 

## Table of contents

### Properties

- [accountId](feeddataservicerecord.md#accountid)
- [completeDate](feeddataservicerecord.md#completedate)
- [errorCount](feeddataservicerecord.md#errorcount)
- [errorRate](feeddataservicerecord.md#errorrate)
- [feedId](feeddataservicerecord.md#feedid)
- [fileUploadSrc](feeddataservicerecord.md#fileuploadsrc)
- [fileUploadStatus](feeddataservicerecord.md#fileuploadstatus)
- [isDebug](feeddataservicerecord.md#isdebug)
- [itemListUploadId](feeddataservicerecord.md#itemlistuploadid)
- [itemListUploadType](feeddataservicerecord.md#itemlistuploadtype)
- [uploadDate](feeddataservicerecord.md#uploaddate)

## Properties

### accountId

• `Optional` **accountId**: ``null`` \| *number*

<div lang=\"ja\">アカウントID</div> 

**`memberof`** FeedDataServiceRecord

___

### completeDate

• `Optional` **completeDate**: ``null`` \| *string*

<div lang=\"ja\">取り込み完了日(yyyyMMdd)</div> 

**`memberof`** FeedDataServiceRecord

___

### errorCount

• `Optional` **errorCount**: ``null`` \| *number*

<div lang=\"ja\">不備がある商品情報の件数</div> 

**`memberof`** FeedDataServiceRecord

___

### errorRate

• `Optional` **errorRate**: ``null`` \| *number*

<div lang=\"ja\">エラー率</div> 

**`memberof`** FeedDataServiceRecord

___

### feedId

• `Optional` **feedId**: ``null`` \| *number*

<div lang=\"ja\">Feedを識別するId</div> 

**`memberof`** FeedDataServiceRecord

___

### fileUploadSrc

• `Optional` **fileUploadSrc**: ``null`` \| [*CampaignManagementTool*](./enums/feeddataservicefileuploadsrc.md#campaignmanagementtool) \| [*Api*](./enums/feeddataservicefileuploadsrc.md#api) \| [*FtpSchedule*](./enums/feeddataservicefileuploadsrc.md#ftpschedule) \| [*FtpDirect*](./enums/feeddataservicefileuploadsrc.md#ftpdirect) \| [*Unknown*](./enums/feeddataservicefileuploadsrc.md#unknown)

**`memberof`** FeedDataServiceRecord

___

### fileUploadStatus

• `Optional` **fileUploadStatus**: ``null`` \| [*Uploaded*](./enums/feeddataservicefileuploadstatus.md#uploaded) \| [*Completed*](./enums/feeddataservicefileuploadstatus.md#completed) \| [*FileFormatError*](./enums/feeddataservicefileuploadstatus.md#fileformaterror) \| [*SystemError*](./enums/feeddataservicefileuploadstatus.md#systemerror) \| [*NetworkError*](./enums/feeddataservicefileuploadstatus.md#networkerror) \| [*FileNotFoundError*](./enums/feeddataservicefileuploadstatus.md#filenotfounderror) \| [*FileSizeOverError*](./enums/feeddataservicefileuploadstatus.md#filesizeovererror) \| [*AuthError*](./enums/feeddataservicefileuploadstatus.md#autherror) \| [*UploadCountOverError*](./enums/feeddataservicefileuploadstatus.md#uploadcountovererror) \| [*NotModified*](./enums/feeddataservicefileuploadstatus.md#notmodified) \| [*Unknown*](./enums/feeddataservicefileuploadstatus.md#unknown)

**`memberof`** FeedDataServiceRecord

___

### isDebug

• `Optional` **isDebug**: ``null`` \| *boolean*

<div lang=\"ja\">trueはデバッグモードでの実行を意味します。</div> 

**`memberof`** FeedDataServiceRecord

___

### itemListUploadId

• `Optional` **itemListUploadId**: ``null`` \| *number*

<div lang=\"ja\">アップロードした商品情報を識別するID</div> 

**`memberof`** FeedDataServiceRecord

___

### itemListUploadType

• `Optional` **itemListUploadType**: ``null`` \| [*UpdatePart*](./enums/feeddataserviceitemlistuploadtype.md#updatepart) \| [*UpdateAll*](./enums/feeddataserviceitemlistuploadtype.md#updateall) \| [*Unknown*](./enums/feeddataserviceitemlistuploadtype.md#unknown)

**`memberof`** FeedDataServiceRecord

___

### uploadDate

• `Optional` **uploadDate**: ``null`` \| *string*

<div lang=\"ja\">アップロード日(yyyyMMdd)</div> 

**`memberof`** FeedDataServiceRecord
