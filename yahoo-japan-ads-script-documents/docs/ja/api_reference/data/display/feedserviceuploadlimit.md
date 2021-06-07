# FeedServiceUploadLimit


<div lang=\"ja\">FeedServiceUploadLimitオブジェクトは、Feedファイルの制限情報を保持します。</div> 

## Table of contents

### Properties

- [controlType](feedserviceuploadlimit.md#controltype)
- [limitValue](feedserviceuploadlimit.md#limitvalue)
- [sourceType](feedserviceuploadlimit.md#sourcetype)

## Properties

### controlType

• `Optional` **controlType**: ``null`` \| [*UploadCountLimit*](./enums/feedservicecontroltype.md#uploadcountlimit) \| [*FileRowsLimit*](./enums/feedservicecontroltype.md#filerowslimit) \| [*FileSizeLimitCompress*](./enums/feedservicecontroltype.md#filesizelimitcompress) \| [*FileSizeLimitUncompress*](./enums/feedservicecontroltype.md#filesizelimituncompress) \| [*Unknown*](./enums/feedservicecontroltype.md#unknown)

**`memberof`** FeedServiceUploadLimit

___

### limitValue

• `Optional` **limitValue**: ``null`` \| *number*

<div lang=\"ja\">上限数です。</div> 

**`memberof`** FeedServiceUploadLimit

___

### sourceType

• `Optional` **sourceType**: ``null`` \| [*FtpSchedule*](./enums/feedservicesourcetype.md#ftpschedule) \| [*FtpDirect*](./enums/feedservicesourcetype.md#ftpdirect) \| [*Api*](./enums/feedservicesourcetype.md#api) \| [*FtpAndApi*](./enums/feedservicesourcetype.md#ftpandapi) \| [*CampaignManagementTool*](./enums/feedservicesourcetype.md#campaignmanagementtool) \| [*Unknown*](./enums/feedservicesourcetype.md#unknown)

**`memberof`** FeedServiceUploadLimit
