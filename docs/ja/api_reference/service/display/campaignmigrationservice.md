# CampaignMigrationService


## Table of contents

### Methods

- [download](campaignmigrationservice.md#download)
- [downloadErrorFile](campaignmigrationservice.md#downloaderrorfile)
- [downloadOriginalFile](campaignmigrationservice.md#downloadoriginalfile)
- [get](campaignmigrationservice.md#get)
- [upload](campaignmigrationservice.md#upload)

## Methods

### download

▸ **download**(`campaignMigrationServiceDownloadSelector?`: [*CampaignMigrationServiceDownloadSelector*](../../data/display/campaignmigrationservicedownloadselector.md)): *Uint8Array*

<div lang=\"ja\">マイグレーション対象のキャンペーン一覧をダウンロードします。</div> 

#### Parameters

| Name | Type |
| :------ | :------ |
| `campaignMigrationServiceDownloadSelector?` | [*CampaignMigrationServiceDownloadSelector*](../../data/display/campaignmigrationservicedownloadselector.md) |

**Returns:** *Uint8Array*

___

### downloadErrorFile

▸ **downloadErrorFile**(`campaignMigrationServiceDownloadFileSelector?`: [*CampaignMigrationServiceDownloadFileSelector*](../../data/display/campaignmigrationservicedownloadfileselector.md)): *Uint8Array*

<div lang=\"ja\">エラーが発生したキャンペーン一覧のcsvファイルをダウンロードします。</div> 

#### Parameters

| Name | Type |
| :------ | :------ |
| `campaignMigrationServiceDownloadFileSelector?` | [*CampaignMigrationServiceDownloadFileSelector*](../../data/display/campaignmigrationservicedownloadfileselector.md) |

**Returns:** *Uint8Array*

___

### downloadOriginalFile

▸ **downloadOriginalFile**(`campaignMigrationServiceDownloadFileSelector?`: [*CampaignMigrationServiceDownloadFileSelector*](../../data/display/campaignmigrationservicedownloadfileselector.md)): *Uint8Array*

<div lang=\"ja\">アップロードしたオリジナルcsvファイルをダウンロードします。</div> 

#### Parameters

| Name | Type |
| :------ | :------ |
| `campaignMigrationServiceDownloadFileSelector?` | [*CampaignMigrationServiceDownloadFileSelector*](../../data/display/campaignmigrationservicedownloadfileselector.md) |

**Returns:** *Uint8Array*

___

### get

▸ **get**(`campaignMigrationServiceSelector?`: [*CampaignMigrationServiceSelector*](../../data/display/campaignmigrationserviceselector.md)): [*CampaignMigrationServiceGetResponse*](../../data/display/campaignmigrationservicegetresponse.md)

<div lang=\"ja\">マイグレーション状況を取得します。</div> 

#### Parameters

| Name | Type |
| :------ | :------ |
| `campaignMigrationServiceSelector?` | [*CampaignMigrationServiceSelector*](../../data/display/campaignmigrationserviceselector.md) |

**Returns:** [*CampaignMigrationServiceGetResponse*](../../data/display/campaignmigrationservicegetresponse.md)

___

### upload

▸ **upload**(`accountId`: *number*, `file?`: *any*): [*CampaignMigrationServiceUploadResponse*](../../data/display/campaignmigrationserviceuploadresponse.md)

<div lang=\"ja\">マイグレーション用csvファイルのアップロード処理を実施します。</div> 

#### Parameters

| Name | Type |
| :------ | :------ |
| `accountId` | *number* |
| `file?` | *any* |

**Returns:** [*CampaignMigrationServiceUploadResponse*](../../data/display/campaignmigrationserviceuploadresponse.md)
