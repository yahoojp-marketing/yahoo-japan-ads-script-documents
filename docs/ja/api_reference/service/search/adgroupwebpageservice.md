# AdGroupWebpageService


## Table of contents

### Methods

- [add](adgroupwebpageservice.md#add)
- [get](adgroupwebpageservice.md#get)
- [remove](adgroupwebpageservice.md#remove)
- [set](adgroupwebpageservice.md#set)

## Methods

### add

▸ **add**(`adGroupWebpageServiceOperation?`: [*AdGroupWebpageServiceOperation*](../../data/search/adgroupwebpageserviceoperation.md)): [*AdGroupWebpageServiceMutateResponse*](../../data/search/adgroupwebpageservicemutateresponse.md)

<div lang=\"ja\">広告グループにPageFeedItemを配信、又は、除外として設定します。<br> ※1リクエストで異なるキャンペーン配下の広告グループに対してWebページ情報の設定が可能です。<br> ※1リクエスト内で同一のadGroupIdに同一組み合わせのWebpageParameterを設定できません。</div> 

#### Parameters

| Name | Type |
| :------ | :------ |
| `adGroupWebpageServiceOperation?` | [*AdGroupWebpageServiceOperation*](../../data/search/adgroupwebpageserviceoperation.md) |

**Returns:** [*AdGroupWebpageServiceMutateResponse*](../../data/search/adgroupwebpageservicemutateresponse.md)

___

### get

▸ **get**(`adGroupWebpageServiceSelector?`: [*AdGroupWebpageServiceSelector*](../../data/search/adgroupwebpageserviceselector.md)): [*AdGroupWebpageServiceGetResponse*](../../data/search/adgroupwebpageservicegetresponse.md)

<div lang=\"ja\">広告グループに設定されているPageFeedItemの配信/除外設定を取得します。</div> 

#### Parameters

| Name | Type |
| :------ | :------ |
| `adGroupWebpageServiceSelector?` | [*AdGroupWebpageServiceSelector*](../../data/search/adgroupwebpageserviceselector.md) |

**Returns:** [*AdGroupWebpageServiceGetResponse*](../../data/search/adgroupwebpageservicegetresponse.md)

___

### remove

▸ **remove**(`adGroupWebpageServiceOperation?`: [*AdGroupWebpageServiceOperation*](../../data/search/adgroupwebpageserviceoperation.md)): [*AdGroupWebpageServiceMutateResponse*](../../data/search/adgroupwebpageservicemutateresponse.md)

<div lang=\"ja\">広告グループに関連付けしているPageFeedItemを解除します。</div> 

#### Parameters

| Name | Type |
| :------ | :------ |
| `adGroupWebpageServiceOperation?` | [*AdGroupWebpageServiceOperation*](../../data/search/adgroupwebpageserviceoperation.md) |

**Returns:** [*AdGroupWebpageServiceMutateResponse*](../../data/search/adgroupwebpageservicemutateresponse.md)

___

### set

▸ **set**(`adGroupWebpageServiceOperation?`: [*AdGroupWebpageServiceOperation*](../../data/search/adgroupwebpageserviceoperation.md)): [*AdGroupWebpageServiceMutateResponse*](../../data/search/adgroupwebpageservicemutateresponse.md)

<div lang=\"ja\">広告グループにPageFeedItemを配信、又は、除外として設定します。<br> ※1リクエストで異なるキャンペーン配下の広告グループに対してWebページ情報の設定が可能です。<br> ※1リクエスト内で同一のadGroupIdに同一組み合わせのWebpageParameterを設定できません。</div> 

#### Parameters

| Name | Type |
| :------ | :------ |
| `adGroupWebpageServiceOperation?` | [*AdGroupWebpageServiceOperation*](../../data/search/adgroupwebpageserviceoperation.md) |

**Returns:** [*AdGroupWebpageServiceMutateResponse*](../../data/search/adgroupwebpageservicemutateresponse.md)
