# FeedDataService


## Table of contents

### Methods

- [downloadErrorFile](feeddataservice.md#downloaderrorfile)
- [get](feeddataservice.md#get)
- [upload](feeddataservice.md#upload)

## Methods

### downloadErrorFile

▸ **downloadErrorFile**(`feedDataServiceDownloadErrorFileSelector?`: [*FeedDataServiceDownloadErrorFileSelector*](../../data/display/feeddataservicedownloaderrorfileselector.md)): *Uint8Array*

<div lang=\"ja\">商品情報のエラーファイルダウンロード処理を実施します。</div> 

#### Parameters

| Name | Type |
| :------ | :------ |
| `feedDataServiceDownloadErrorFileSelector?` | [*FeedDataServiceDownloadErrorFileSelector*](../../data/display/feeddataservicedownloaderrorfileselector.md) |

**Returns:** *Uint8Array*

___

### get

▸ **get**(`feedDataServiceSelector?`: [*FeedDataServiceSelector*](../../data/display/feeddataserviceselector.md)): [*FeedDataServiceGetResponse*](../../data/display/feeddataservicegetresponse.md)

<div lang=\"ja\">アップロードした商品情報の処理状況を照会します。</div> 

#### Parameters

| Name | Type |
| :------ | :------ |
| `feedDataServiceSelector?` | [*FeedDataServiceSelector*](../../data/display/feeddataserviceselector.md) |

**Returns:** [*FeedDataServiceGetResponse*](../../data/display/feeddataservicegetresponse.md)

___

### upload

▸ **upload**(`accountId`: *number*, `feedId`: *number*, `uploadType`: [*FeedDataServiceItemListUploadType*](../../data/display/enums/feeddataserviceitemlistuploadtype.md), `isDebug`: *boolean*, `file?`: *any*): [*FeedDataServiceUploadResponse*](../../data/display/feeddataserviceuploadresponse.md)

<div lang=\"ja\">商品情報のアップロード処理を実施します。</div> 

#### Parameters

| Name | Type |
| :------ | :------ |
| `accountId` | *number* |
| `feedId` | *number* |
| `uploadType` | [*FeedDataServiceItemListUploadType*](../../data/display/enums/feeddataserviceitemlistuploadtype.md) |
| `isDebug` | *boolean* |
| `file?` | *any* |

**Returns:** [*FeedDataServiceUploadResponse*](../../data/display/feeddataserviceuploadresponse.md)
