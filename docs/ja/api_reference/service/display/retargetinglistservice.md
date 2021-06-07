# RetargetingListService


## Table of contents

### Methods

- [add](retargetinglistservice.md#add)
- [get](retargetinglistservice.md#get)
- [getUploadUserListStatus](retargetinglistservice.md#getuploaduserliststatus)
- [remove](retargetinglistservice.md#remove)
- [set](retargetinglistservice.md#set)
- [uploadUserList](retargetinglistservice.md#uploaduserlist)

## Methods

### add

▸ **add**(`retargetingListServiceOperation?`: [*RetargetingListServiceOperation*](../../data/display/retargetinglistserviceoperation.md)): [*RetargetingListServiceMutateResponse*](../../data/display/retargetinglistservicemutateresponse.md)

<div lang=\"ja\">サイトリターゲティングのターゲットリストを作成します。</div> 

#### Parameters

| Name | Type |
| :------ | :------ |
| `retargetingListServiceOperation?` | [*RetargetingListServiceOperation*](../../data/display/retargetinglistserviceoperation.md) |

**Returns:** [*RetargetingListServiceMutateResponse*](../../data/display/retargetinglistservicemutateresponse.md)

___

### get

▸ **get**(`retargetingListServiceSelector?`: [*RetargetingListServiceSelector*](../../data/display/retargetinglistserviceselector.md)): [*RetargetingListServiceGetResponse*](../../data/display/retargetinglistservicegetresponse.md)

<div lang=\"ja\">サイトリターゲティングのターゲットリストを取得します。</div> 

#### Parameters

| Name | Type |
| :------ | :------ |
| `retargetingListServiceSelector?` | [*RetargetingListServiceSelector*](../../data/display/retargetinglistserviceselector.md) |

**Returns:** [*RetargetingListServiceGetResponse*](../../data/display/retargetinglistservicegetresponse.md)

___

### getUploadUserListStatus

▸ **getUploadUserListStatus**(`retargetingListServiceUploadUserListStatusSelector?`: [*RetargetingListServiceUploadUserListStatusSelector*](../../data/display/retargetinglistserviceuploaduserliststatusselector.md)): [*RetargetingListServiceGetUploadUserListResponse*](../../data/display/retargetinglistservicegetuploaduserlistresponse.md)

<div lang=\"ja\">ユーザリストのアップロード状況を取得します。</div> 

#### Parameters

| Name | Type |
| :------ | :------ |
| `retargetingListServiceUploadUserListStatusSelector?` | [*RetargetingListServiceUploadUserListStatusSelector*](../../data/display/retargetinglistserviceuploaduserliststatusselector.md) |

**Returns:** [*RetargetingListServiceGetUploadUserListResponse*](../../data/display/retargetinglistservicegetuploaduserlistresponse.md)

___

### remove

▸ **remove**(`retargetingListServiceOperation?`: [*RetargetingListServiceOperation*](../../data/display/retargetinglistserviceoperation.md)): [*RetargetingListServiceMutateResponse*](../../data/display/retargetinglistservicemutateresponse.md)

<div lang=\"ja\">サイトリターゲティングのターゲットリストを削除します。</div> 

#### Parameters

| Name | Type |
| :------ | :------ |
| `retargetingListServiceOperation?` | [*RetargetingListServiceOperation*](../../data/display/retargetinglistserviceoperation.md) |

**Returns:** [*RetargetingListServiceMutateResponse*](../../data/display/retargetinglistservicemutateresponse.md)

___

### set

▸ **set**(`retargetingListServiceOperation?`: [*RetargetingListServiceOperation*](../../data/display/retargetinglistserviceoperation.md)): [*RetargetingListServiceMutateResponse*](../../data/display/retargetinglistservicemutateresponse.md)

<div lang=\"ja\">サイトリターゲティングのターゲットリストを更新します。</div> 

#### Parameters

| Name | Type |
| :------ | :------ |
| `retargetingListServiceOperation?` | [*RetargetingListServiceOperation*](../../data/display/retargetinglistserviceoperation.md) |

**Returns:** [*RetargetingListServiceMutateResponse*](../../data/display/retargetinglistservicemutateresponse.md)

___

### uploadUserList

▸ **uploadUserList**(`accountId`: *number*, `retargetingTagId`: *string*, `targetListId`: *number*, `uploadType`: [*RetargetingListServiceUploadUserListUploadType*](../../data/display/enums/retargetinglistserviceuploaduserlistuploadtype.md), `compressType`: [*RetargetingListServiceUploadUserListCompressType*](../../data/display/enums/retargetinglistserviceuploaduserlistcompresstype.md), `customUserId?`: *string*, `body?`: *any*): [*RetargetingListServiceUploadUserListResponse*](../../data/display/retargetinglistserviceuploaduserlistresponse.md)

<div lang=\"ja\">   カスタムリストのユーザリストファイルをアップロードします。<br/>   アップロードリクエストでは以下を指定します。   <ul>     <li>・Content-Type: application/octet-stream（非圧縮形式の場合はtext/plain指定も可能）</li>     <li>・Content-Length: アップロード対象のファイルのバイト数</li>     <li>・Request body: アップロードするユーザーリストのファイル本体</li>   </ul>   Transfer-encoding: chunkedを指定してのアップロードには対応していません。<br/>   また、アップロードするファイルの制限は下記の通りです。   <ul>     <li>・UTF8、BOMなし、正規化形式</li>     <li>・ユーザーIDごとに改行</li>     <li>・改行コードLF</li>     <li>・ファイルサイズ上限1GB(1,073,741,824 byte)</li>   </ul> </div> 

#### Parameters

| Name | Type |
| :------ | :------ |
| `accountId` | *number* |
| `retargetingTagId` | *string* |
| `targetListId` | *number* |
| `uploadType` | [*RetargetingListServiceUploadUserListUploadType*](../../data/display/enums/retargetinglistserviceuploaduserlistuploadtype.md) |
| `compressType` | [*RetargetingListServiceUploadUserListCompressType*](../../data/display/enums/retargetinglistserviceuploaduserlistcompresstype.md) |
| `customUserId?` | *string* |
| `body?` | *any* |

**Returns:** [*RetargetingListServiceUploadUserListResponse*](../../data/display/retargetinglistserviceuploaduserlistresponse.md)
