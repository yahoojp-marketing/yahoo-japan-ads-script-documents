# MediaService


## Table of contents

### Methods

- [add](mediaservice.md#add)
- [download](mediaservice.md#download)
- [get](mediaservice.md#get)
- [remove](mediaservice.md#remove)
- [set](mediaservice.md#set)

## Methods

### add

▸ **add**(`mediaServiceOperation?`: [*MediaServiceOperation*](../../data/display/mediaserviceoperation.md)): [*MediaServiceMutateResponse*](../../data/display/mediaservicemutateresponse.md)

<div lang=\"ja\">画像のアップロードを行います（最大1件）。</div> 

#### Parameters

| Name | Type |
| :------ | :------ |
| `mediaServiceOperation?` | [*MediaServiceOperation*](../../data/display/mediaserviceoperation.md) |

**Returns:** [*MediaServiceMutateResponse*](../../data/display/mediaservicemutateresponse.md)

___

### download

▸ **download**(`mediaServiceDownloadSelector?`: [*MediaServiceDownloadSelector*](../../data/display/mediaservicedownloadselector.md)): *Uint8Array*

<div lang=\"ja\">入稿済みのメディアファイルをダウンロードします。</div> 

#### Parameters

| Name | Type |
| :------ | :------ |
| `mediaServiceDownloadSelector?` | [*MediaServiceDownloadSelector*](../../data/display/mediaservicedownloadselector.md) |

**Returns:** *Uint8Array*

___

### get

▸ **get**(`mediaServiceSelector?`: [*MediaServiceSelector*](../../data/display/mediaserviceselector.md)): [*MediaServiceGetResponse*](../../data/display/mediaservicegetresponse.md)

<div lang=\"ja\">入稿済の画像の一覧を条件を指定して取得します。</div> 

#### Parameters

| Name | Type |
| :------ | :------ |
| `mediaServiceSelector?` | [*MediaServiceSelector*](../../data/display/mediaserviceselector.md) |

**Returns:** [*MediaServiceGetResponse*](../../data/display/mediaservicegetresponse.md)

___

### remove

▸ **remove**(`mediaServiceOperation?`: [*MediaServiceOperation*](../../data/display/mediaserviceoperation.md)): [*MediaServiceMutateResponse*](../../data/display/mediaservicemutateresponse.md)

<div lang=\"ja\">入稿済みの画像を削除します。</div> 

#### Parameters

| Name | Type |
| :------ | :------ |
| `mediaServiceOperation?` | [*MediaServiceOperation*](../../data/display/mediaserviceoperation.md) |

**Returns:** [*MediaServiceMutateResponse*](../../data/display/mediaservicemutateresponse.md)

___

### set

▸ **set**(`mediaServiceOperation?`: [*MediaServiceOperation*](../../data/display/mediaserviceoperation.md)): [*MediaServiceMutateResponse*](../../data/display/mediaservicemutateresponse.md)

<div lang=\"ja\">入稿済の画像のステータス（配信設定）の変更を行います。</div> 

#### Parameters

| Name | Type |
| :------ | :------ |
| `mediaServiceOperation?` | [*MediaServiceOperation*](../../data/display/mediaserviceoperation.md) |

**Returns:** [*MediaServiceMutateResponse*](../../data/display/mediaservicemutateresponse.md)
