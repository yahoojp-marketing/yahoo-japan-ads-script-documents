# CampaignTargetService


## Table of contents

### Methods

- [add](campaigntargetservice.md#add)
- [get](campaigntargetservice.md#get)
- [remove](campaigntargetservice.md#remove)
- [set](campaigntargetservice.md#set)

## Methods

### add

▸ **add**(`campaignTargetServiceOperation?`: [*CampaignTargetServiceOperation*](../../data/search/campaigntargetserviceoperation.md)): [*CampaignTargetServiceMutateResponse*](../../data/search/campaigntargetservicemutateresponse.md)

<div lang=\"ja\">キャンペーンのターゲティング設定に関する情報を追加します。</div> 

#### Parameters

| Name | Type |
| :------ | :------ |
| `campaignTargetServiceOperation?` | [*CampaignTargetServiceOperation*](../../data/search/campaigntargetserviceoperation.md) |

**Returns:** [*CampaignTargetServiceMutateResponse*](../../data/search/campaigntargetservicemutateresponse.md)

___

### get

▸ **get**(`campaignTargetServiceSelector?`: [*CampaignTargetServiceSelector*](../../data/search/campaigntargetserviceselector.md)): [*CampaignTargetServiceGetResponse*](../../data/search/campaigntargetservicegetresponse.md)

<div lang=\"ja\">キャンペーンのターゲティング設定に関する情報を取得します。</div> 

#### Parameters

| Name | Type |
| :------ | :------ |
| `campaignTargetServiceSelector?` | [*CampaignTargetServiceSelector*](../../data/search/campaigntargetserviceselector.md) |

**Returns:** [*CampaignTargetServiceGetResponse*](../../data/search/campaigntargetservicegetresponse.md)

___

### remove

▸ **remove**(`campaignTargetServiceOperation?`: [*CampaignTargetServiceOperation*](../../data/search/campaigntargetserviceoperation.md)): [*CampaignTargetServiceMutateResponse*](../../data/search/campaigntargetservicemutateresponse.md)

<div lang=\"ja\">キャンペーンのターゲティング設定に関する情報を削除します。</div> 

#### Parameters

| Name | Type |
| :------ | :------ |
| `campaignTargetServiceOperation?` | [*CampaignTargetServiceOperation*](../../data/search/campaigntargetserviceoperation.md) |

**Returns:** [*CampaignTargetServiceMutateResponse*](../../data/search/campaigntargetservicemutateresponse.md)

___

### set

▸ **set**(`campaignTargetServiceOperation?`: [*CampaignTargetServiceOperation*](../../data/search/campaigntargetserviceoperation.md)): [*CampaignTargetServiceMutateResponse*](../../data/search/campaigntargetservicemutateresponse.md)

<div lang=\"ja\">キャンペーンのターゲティング設定に関する情報を変更します。※入札調整率（bidmultiplier）のみ変更可能です。</div> 

#### Parameters

| Name | Type |
| :------ | :------ |
| `campaignTargetServiceOperation?` | [*CampaignTargetServiceOperation*](../../data/search/campaigntargetserviceoperation.md) |

**Returns:** [*CampaignTargetServiceMutateResponse*](../../data/search/campaigntargetservicemutateresponse.md)
