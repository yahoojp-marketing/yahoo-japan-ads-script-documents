# FeedService


## Table of contents

### Methods

- [add](feedservice.md#add)
- [downloadDisApprovalReasonList](feedservice.md#downloaddisapprovalreasonlist)
- [get](feedservice.md#get)
- [remove](feedservice.md#remove)
- [set](feedservice.md#set)

## Methods

### add

▸ **add**(`feedServiceOperation?`: [*FeedServiceOperation*](../../data/display/feedserviceoperation.md)): [*FeedServiceMutateResponse*](../../data/display/feedservicemutateresponse.md)

<div lang=\"ja\">Feed情報を新規登録します</div> 

#### Parameters

| Name | Type |
| :------ | :------ |
| `feedServiceOperation?` | [*FeedServiceOperation*](../../data/display/feedserviceoperation.md) |

**Returns:** [*FeedServiceMutateResponse*](../../data/display/feedservicemutateresponse.md)

___

### downloadDisApprovalReasonList

▸ **downloadDisApprovalReasonList**(`feedServiceDownloadDisApprovalReasonListSelector?`: [*FeedServiceDownloadDisApprovalReasonListSelector*](../../data/display/feedservicedownloaddisapprovalreasonlistselector.md)): *Uint8Array*

<div lang=\"ja\">Feed情報の審査否認理由をダウンロードします。</div> 

#### Parameters

| Name | Type |
| :------ | :------ |
| `feedServiceDownloadDisApprovalReasonListSelector?` | [*FeedServiceDownloadDisApprovalReasonListSelector*](../../data/display/feedservicedownloaddisapprovalreasonlistselector.md) |

**Returns:** *Uint8Array*

___

### get

▸ **get**(`feedServiceSelector?`: [*FeedServiceSelector*](../../data/display/feedserviceselector.md)): [*FeedServiceGetResponse*](../../data/display/feedservicegetresponse.md)

<div lang=\"ja\">Feed情報を取得します。</div> 

#### Parameters

| Name | Type |
| :------ | :------ |
| `feedServiceSelector?` | [*FeedServiceSelector*](../../data/display/feedserviceselector.md) |

**Returns:** [*FeedServiceGetResponse*](../../data/display/feedservicegetresponse.md)

___

### remove

▸ **remove**(`feedServiceOperation?`: [*FeedServiceOperation*](../../data/display/feedserviceoperation.md)): [*FeedServiceMutateResponse*](../../data/display/feedservicemutateresponse.md)

<div lang=\"ja\">Feed情報を削除します</div> 

#### Parameters

| Name | Type |
| :------ | :------ |
| `feedServiceOperation?` | [*FeedServiceOperation*](../../data/display/feedserviceoperation.md) |

**Returns:** [*FeedServiceMutateResponse*](../../data/display/feedservicemutateresponse.md)

___

### set

▸ **set**(`feedServiceOperation?`: [*FeedServiceOperation*](../../data/display/feedserviceoperation.md)): [*FeedServiceMutateResponse*](../../data/display/feedservicemutateresponse.md)

<div lang=\"ja\">Feed情報を更新します</div> 

#### Parameters

| Name | Type |
| :------ | :------ |
| `feedServiceOperation?` | [*FeedServiceOperation*](../../data/display/feedserviceoperation.md) |

**Returns:** [*FeedServiceMutateResponse*](../../data/display/feedservicemutateresponse.md)
