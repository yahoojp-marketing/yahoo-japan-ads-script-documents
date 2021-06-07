# CampaignExportServiceSelector


<div lang=\"ja\">CampaignExportServiceSelector オブジェクトは、登録したジョブを検索する条件を表します。</div> 

## Table of contents

### Properties

- [accountId](campaignexportserviceselector.md#accountid)
- [jobIds](campaignexportserviceselector.md#jobids)
- [jobStatuses](campaignexportserviceselector.md#jobstatuses)
- [numberResults](campaignexportserviceselector.md#numberresults)
- [startIndex](campaignexportserviceselector.md#startindex)

## Properties

### accountId

• **accountId**: *number*

<div lang=\"ja\">検索条件：アカウントIDです。</div> 

**`memberof`** CampaignExportServiceSelector

___

### jobIds

• `Optional` **jobIds**: ``null`` \| *number*[]

<div lang=\"ja\">検索条件：ジョブIDです。</div> 

**`memberof`** CampaignExportServiceSelector

___

### jobStatuses

• `Optional` **jobStatuses**: ``null`` \| [*CampaignExportServiceJobStatus*](./enums/campaignexportservicejobstatus.md)[]

**`memberof`** CampaignExportServiceSelector

___

### numberResults

• `Optional` **numberResults**: ``null`` \| *number*

<div lang=\"ja\">ページの最大件数です。このフィールドは、1以上を指定する必要があります。</div> 

**`memberof`** CampaignExportServiceSelector

___

### startIndex

• `Optional` **startIndex**: ``null`` \| *number*

<div lang=\"ja\">ページの先頭のインデックスです。このフィールドは、1以上を指定する必要があります。</div> 

**`memberof`** CampaignExportServiceSelector
