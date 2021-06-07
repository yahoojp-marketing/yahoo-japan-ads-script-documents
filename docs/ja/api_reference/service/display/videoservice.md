# VideoService


## Table of contents

### Methods

- [download](videoservice.md#download)
- [get](videoservice.md#get)
- [remove](videoservice.md#remove)
- [set](videoservice.md#set)
- [upload](videoservice.md#upload)

## Methods

### download

▸ **download**(`videoServiceDownloadSelector?`: [*VideoServiceDownloadSelector*](../../data/display/videoservicedownloadselector.md)): *Uint8Array*

<div lang=\"ja\">入稿済の動画をダウンロードします。</div> 

#### Parameters

| Name | Type |
| :------ | :------ |
| `videoServiceDownloadSelector?` | [*VideoServiceDownloadSelector*](../../data/display/videoservicedownloadselector.md) |

**Returns:** *Uint8Array*

___

### get

▸ **get**(`videoServiceSelector?`: [*VideoServiceSelector*](../../data/display/videoserviceselector.md)): [*VideoServiceGetResponse*](../../data/display/videoservicegetresponse.md)

<div lang=\"ja\">入稿済の動画の情報を取得します。</div> 

#### Parameters

| Name | Type |
| :------ | :------ |
| `videoServiceSelector?` | [*VideoServiceSelector*](../../data/display/videoserviceselector.md) |

**Returns:** [*VideoServiceGetResponse*](../../data/display/videoservicegetresponse.md)

___

### remove

▸ **remove**(`videoServiceOperation?`: [*VideoServiceOperation*](../../data/display/videoserviceoperation.md)): [*VideoServiceMutateResponse*](../../data/display/videoservicemutateresponse.md)

<div lang=\"ja\">入稿済みの動画を削除します。</div> 

#### Parameters

| Name | Type |
| :------ | :------ |
| `videoServiceOperation?` | [*VideoServiceOperation*](../../data/display/videoserviceoperation.md) |

**Returns:** [*VideoServiceMutateResponse*](../../data/display/videoservicemutateresponse.md)

___

### set

▸ **set**(`videoServiceOperation?`: [*VideoServiceOperation*](../../data/display/videoserviceoperation.md)): [*VideoServiceMutateResponse*](../../data/display/videoservicemutateresponse.md)

<div lang=\"ja\">入稿済の動画の情報（動画名、配信状況）を変更します。</div> 

#### Parameters

| Name | Type |
| :------ | :------ |
| `videoServiceOperation?` | [*VideoServiceOperation*](../../data/display/videoserviceoperation.md) |

**Returns:** [*VideoServiceMutateResponse*](../../data/display/videoservicemutateresponse.md)

___

### upload

▸ **upload**(`accountId`: *number*, `videoName`: *string*, `videoTitle`: *string*, `userStatus`: [*VideoServiceUserStatus*](../../data/display/enums/videoserviceuserstatus.md), `file?`: *any*): [*VideoServiceUploadResponse*](../../data/display/videoserviceuploadresponse.md)

<div lang=\"ja\">動画ファイルのアップロード処理を実施します。</div> 

#### Parameters

| Name | Type |
| :------ | :------ |
| `accountId` | *number* |
| `videoName` | *string* |
| `videoTitle` | *string* |
| `userStatus` | [*VideoServiceUserStatus*](../../data/display/enums/videoserviceuserstatus.md) |
| `file?` | *any* |

**Returns:** [*VideoServiceUploadResponse*](../../data/display/videoserviceuploadresponse.md)
