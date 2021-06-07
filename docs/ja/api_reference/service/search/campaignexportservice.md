# CampaignExportService


## Table of contents

### Methods

- [addJob](campaignexportservice.md#addjob)
- [download](campaignexportservice.md#download)
- [get](campaignexportservice.md#get)
- [getExportFields](campaignexportservice.md#getexportfields)

## Methods

### addJob

▸ **addJob**(`campaignExportServiceJobOperation?`: [*CampaignExportServiceJobOperation*](../../data/search/campaignexportservicejoboperation.md)): [*CampaignExportServiceAddJobResponse*](../../data/search/campaignexportserviceaddjobresponse.md)

<div lang=\"ja\">エクスポートの登録を実施します。</div> 

#### Parameters

| Name | Type |
| :------ | :------ |
| `campaignExportServiceJobOperation?` | [*CampaignExportServiceJobOperation*](../../data/search/campaignexportservicejoboperation.md) |

**Returns:** [*CampaignExportServiceAddJobResponse*](../../data/search/campaignexportserviceaddjobresponse.md)

___

### download

▸ **download**(`campaignExportServiceDownloadSelector?`: [*CampaignExportServiceDownloadSelector*](../../data/search/campaignexportservicedownloadselector.md)): *Uint8Array*

<div lang=\"ja\">エクスポート結果をダウンロードします。</div> 

#### Parameters

| Name | Type |
| :------ | :------ |
| `campaignExportServiceDownloadSelector?` | [*CampaignExportServiceDownloadSelector*](../../data/search/campaignexportservicedownloadselector.md) |

**Returns:** *Uint8Array*

___

### get

▸ **get**(`campaignExportServiceSelector?`: [*CampaignExportServiceSelector*](../../data/search/campaignexportserviceselector.md)): [*CampaignExportServiceGetResponse*](../../data/search/campaignexportservicegetresponse.md)

<div lang=\"ja\">登録したジョブに関するステータス情報を取得します。</div> 

#### Parameters

| Name | Type |
| :------ | :------ |
| `campaignExportServiceSelector?` | [*CampaignExportServiceSelector*](../../data/search/campaignexportserviceselector.md) |

**Returns:** [*CampaignExportServiceGetResponse*](../../data/search/campaignexportservicegetresponse.md)

___

### getExportFields

▸ **getExportFields**(`body?`: *object*): [*CampaignExportServiceGetExportFieldsResponse*](../../data/search/campaignexportservicegetexportfieldsresponse.md)

<div lang=\"ja\">エクスポートできるフィールドを照会します。</div> 

#### Parameters

| Name | Type |
| :------ | :------ |
| `body?` | *object* |

**Returns:** [*CampaignExportServiceGetExportFieldsResponse*](../../data/search/campaignexportservicegetexportfieldsresponse.md)
