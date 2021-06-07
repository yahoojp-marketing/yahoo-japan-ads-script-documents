# OfflineConversionService


## Table of contents

### Methods

- [download](offlineconversionservice.md#download)
- [downloadErrorFile](offlineconversionservice.md#downloaderrorfile)
- [get](offlineconversionservice.md#get)
- [upload](offlineconversionservice.md#upload)

## Methods

### download

▸ **download**(`offlineConversionServiceDownloadSelector?`: [*OfflineConversionServiceDownloadSelector*](../../data/search/offlineconversionservicedownloadselector.md)): *Uint8Array*

<div lang=\"ja\">ファイルの一括ダウンロードを実施します。</div> 

#### Parameters

| Name | Type |
| :------ | :------ |
| `offlineConversionServiceDownloadSelector?` | [*OfflineConversionServiceDownloadSelector*](../../data/search/offlineconversionservicedownloadselector.md) |

**Returns:** *Uint8Array*

___

### downloadErrorFile

▸ **downloadErrorFile**(`offlineConversionServiceDownloadSelector?`: [*OfflineConversionServiceDownloadSelector*](../../data/search/offlineconversionservicedownloadselector.md)): *Uint8Array*

<div lang=\"ja\">エラーファイルのダウンロードを実施します。</div> 

#### Parameters

| Name | Type |
| :------ | :------ |
| `offlineConversionServiceDownloadSelector?` | [*OfflineConversionServiceDownloadSelector*](../../data/search/offlineconversionservicedownloadselector.md) |

**Returns:** *Uint8Array*

___

### get

▸ **get**(`offlineConversionServiceSelector?`: [*OfflineConversionServiceSelector*](../../data/search/offlineconversionserviceselector.md)): [*OfflineConversionServiceGetResponse*](../../data/search/offlineconversionservicegetresponse.md)

<div lang=\"ja\">登録したオフラインコンバージョンデータの情報を取得します。</div> 

#### Parameters

| Name | Type |
| :------ | :------ |
| `offlineConversionServiceSelector?` | [*OfflineConversionServiceSelector*](../../data/search/offlineconversionserviceselector.md) |

**Returns:** [*OfflineConversionServiceGetResponse*](../../data/search/offlineconversionservicegetresponse.md)

___

### upload

▸ **upload**(`accountId`: *number*, `uploadType`: [*OfflineConversionServiceUploadType*](../../data/search/enums/offlineconversionserviceuploadtype.md), `uploadFileName`: *string*, `file?`: *any*): [*OfflineConversionServiceUploadResponse*](../../data/search/offlineconversionserviceuploadresponse.md)

<div lang=\"ja\"> オフラインコンバージョンデータのアップロード処理を実施します。<br> ・ファイルサイズ上限20Mbyte(20,971,520 byte) </div> 

#### Parameters

| Name | Type |
| :------ | :------ |
| `accountId` | *number* |
| `uploadType` | [*OfflineConversionServiceUploadType*](../../data/search/enums/offlineconversionserviceuploadtype.md) |
| `uploadFileName` | *string* |
| `file?` | *any* |

**Returns:** [*OfflineConversionServiceUploadResponse*](../../data/search/offlineconversionserviceuploadresponse.md)
