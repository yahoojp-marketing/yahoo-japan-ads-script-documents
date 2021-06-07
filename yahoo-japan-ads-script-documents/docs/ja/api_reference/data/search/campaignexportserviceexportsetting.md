# CampaignExportServiceExportSetting


<div lang=\"ja\">CampaignExportServiceExportSetting オブジェクトは、エクスポートする条件を表します。</div> 

## Table of contents

### Properties

- [accountId](campaignexportserviceexportsetting.md#accountid)
- [adGroupAdApprovalStatuses](campaignexportserviceexportsetting.md#adgroupadapprovalstatuses)
- [adGroupAdUserStatuses](campaignexportserviceexportsetting.md#adgroupaduserstatuses)
- [adGroupCriterionApprovalStatuses](campaignexportserviceexportsetting.md#adgroupcriterionapprovalstatuses)
- [adGroupCriterionIds](campaignexportserviceexportsetting.md#adgroupcriterionids)
- [adGroupCriterionUserStatuses](campaignexportserviceexportsetting.md#adgroupcriterionuserstatuses)
- [adGroupIds](campaignexportserviceexportsetting.md#adgroupids)
- [adGroupUserStatuses](campaignexportserviceexportsetting.md#adgroupuserstatuses)
- [adIds](campaignexportserviceexportsetting.md#adids)
- [campaignCriterionIds](campaignexportserviceexportsetting.md#campaigncriterionids)
- [campaignIds](campaignexportserviceexportsetting.md#campaignids)
- [campaignUserStatuses](campaignexportserviceexportsetting.md#campaignuserstatuses)
- [encoding](campaignexportserviceexportsetting.md#encoding)
- [entityTypes](campaignexportserviceexportsetting.md#entitytypes)
- [exportFields](campaignexportserviceexportsetting.md#exportfields)
- [jobName](campaignexportserviceexportsetting.md#jobname)
- [lang](campaignexportserviceexportsetting.md#lang)
- [output](campaignexportserviceexportsetting.md#output)

## Properties

### accountId

• **accountId**: *number*

<div lang=\"ja\">アカウントIDです。<br>このフィールドは、必須です。</div> 

**`memberof`** CampaignExportServiceExportSetting

___

### adGroupAdApprovalStatuses

• `Optional` **adGroupAdApprovalStatuses**: ``null`` \| [*CampaignExportServiceApprovalStatus*](./enums/campaignexportserviceapprovalstatus.md)[]

**`memberof`** CampaignExportServiceExportSetting

___

### adGroupAdUserStatuses

• `Optional` **adGroupAdUserStatuses**: ``null`` \| [*CampaignExportServiceUserStatus*](./enums/campaignexportserviceuserstatus.md)[]

**`memberof`** CampaignExportServiceExportSetting

___

### adGroupCriterionApprovalStatuses

• `Optional` **adGroupCriterionApprovalStatuses**: ``null`` \| [*CampaignExportServiceApprovalStatus*](./enums/campaignexportserviceapprovalstatus.md)[]

**`memberof`** CampaignExportServiceExportSetting

___

### adGroupCriterionIds

• `Optional` **adGroupCriterionIds**: ``null`` \| *number*[]

<div lang=\"ja\">広告グループクライテリアIDです。<br>このフィールドは、省略可能となります。</div> 

**`memberof`** CampaignExportServiceExportSetting

___

### adGroupCriterionUserStatuses

• `Optional` **adGroupCriterionUserStatuses**: ``null`` \| [*CampaignExportServiceUserStatus*](./enums/campaignexportserviceuserstatus.md)[]

**`memberof`** CampaignExportServiceExportSetting

___

### adGroupIds

• `Optional` **adGroupIds**: ``null`` \| *number*[]

<div lang=\"ja\">ダウンロード対象の広告グループIDです。<br> このフィールドは、省略可能となります。</div> 

**`memberof`** CampaignExportServiceExportSetting

___

### adGroupUserStatuses

• `Optional` **adGroupUserStatuses**: ``null`` \| [*CampaignExportServiceUserStatus*](./enums/campaignexportserviceuserstatus.md)[]

**`memberof`** CampaignExportServiceExportSetting

___

### adIds

• `Optional` **adIds**: ``null`` \| *number*[]

<div lang=\"ja\">ダウンロード対象の広告IDです。<br> このフィールドは、省略可能となります。</div> 

**`memberof`** CampaignExportServiceExportSetting

___

### campaignCriterionIds

• `Optional` **campaignCriterionIds**: ``null`` \| *number*[]

<div lang=\"ja\">キャンペーンクライテリアIDです。<br> このフィールドは、省略可能となります。</div> 

**`memberof`** CampaignExportServiceExportSetting

___

### campaignIds

• `Optional` **campaignIds**: ``null`` \| *number*[]

<div lang=\"ja\">ダウンロード対象のキャンペーンIDです。<br> このフィールドは、省略可能となります。</div> 

**`memberof`** CampaignExportServiceExportSetting

___

### campaignUserStatuses

• `Optional` **campaignUserStatuses**: ``null`` \| [*CampaignExportServiceUserStatus*](./enums/campaignexportserviceuserstatus.md)[]

**`memberof`** CampaignExportServiceExportSetting

___

### encoding

• `Optional` **encoding**: ``null`` \| [*Utf8*](./enums/campaignexportserviceencoding.md#utf8) \| [*Sjis*](./enums/campaignexportserviceencoding.md#sjis) \| [*Unknown*](./enums/campaignexportserviceencoding.md#unknown)

**`memberof`** CampaignExportServiceExportSetting

___

### entityTypes

• `Optional` **entityTypes**: ``null`` \| [*CampaignExportServiceEntityType*](./enums/campaignexportserviceentitytype.md)[]

**`memberof`** CampaignExportServiceExportSetting

___

### exportFields

• `Optional` **exportFields**: ``null`` \| *string*[]

<div lang=\"ja\">エクスポートするフィールドを指定します。<br> このフィールドは、省略可能となります。</div> 

**`memberof`** CampaignExportServiceExportSetting

___

### jobName

• `Optional` **jobName**: ``null`` \| *string*

<div lang=\"ja\">ダウンロードするジョブの名称です。<br> このフィールドは、省略可能となります。</div> 

**`memberof`** CampaignExportServiceExportSetting

___

### lang

• `Optional` **lang**: ``null`` \| [*Ja*](./enums/campaignexportservicelang.md#ja) \| [*En*](./enums/campaignexportservicelang.md#en) \| [*Unknown*](./enums/campaignexportservicelang.md#unknown)

**`memberof`** CampaignExportServiceExportSetting

___

### output

• `Optional` **output**: ``null`` \| [*Csv*](./enums/campaignexportserviceoutput.md#csv) \| [*ZippedCsv*](./enums/campaignexportserviceoutput.md#zippedcsv) \| [*Unknown*](./enums/campaignexportserviceoutput.md#unknown)

**`memberof`** CampaignExportServiceExportSetting
