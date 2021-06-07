# CampaignSharedSetService


## Table of contents

### Methods

- [add](campaignsharedsetservice.md#add)
- [get](campaignsharedsetservice.md#get)
- [remove](campaignsharedsetservice.md#remove)

## Methods

### add

▸ **add**(`campaignSharedSetServiceOperation?`: [*CampaignSharedSetServiceOperation*](../../data/search/campaignsharedsetserviceoperation.md)): [*CampaignSharedSetServiceMutateResponse*](../../data/search/campaignsharedsetservicemutateresponse.md)

<div lang=\"ja\">キャンペーンに対象外キーワードリストの関連付け設定を行います。</div> 

#### Parameters

| Name | Type |
| :------ | :------ |
| `campaignSharedSetServiceOperation?` | [*CampaignSharedSetServiceOperation*](../../data/search/campaignsharedsetserviceoperation.md) |

**Returns:** [*CampaignSharedSetServiceMutateResponse*](../../data/search/campaignsharedsetservicemutateresponse.md)

___

### get

▸ **get**(`campaignSharedSetServiceSelector?`: [*CampaignSharedSetServiceSelector*](../../data/search/campaignsharedsetserviceselector.md)): [*CampaignSharedSetServiceGetResponse*](../../data/search/campaignsharedsetservicegetresponse.md)

<div lang=\"ja\">キャンペーンと対象外キーワードリストの関連付け情報を取得します。</div> 

#### Parameters

| Name | Type |
| :------ | :------ |
| `campaignSharedSetServiceSelector?` | [*CampaignSharedSetServiceSelector*](../../data/search/campaignsharedsetserviceselector.md) |

**Returns:** [*CampaignSharedSetServiceGetResponse*](../../data/search/campaignsharedsetservicegetresponse.md)

___

### remove

▸ **remove**(`campaignSharedSetServiceOperation?`: [*CampaignSharedSetServiceOperation*](../../data/search/campaignsharedsetserviceoperation.md)): [*CampaignSharedSetServiceMutateResponse*](../../data/search/campaignsharedsetservicemutateresponse.md)

<div lang=\"ja\">キャンペーンと対象外キーワードリストの関連付け設定を削除します。</div> 

#### Parameters

| Name | Type |
| :------ | :------ |
| `campaignSharedSetServiceOperation?` | [*CampaignSharedSetServiceOperation*](../../data/search/campaignsharedsetserviceoperation.md) |

**Returns:** [*CampaignSharedSetServiceMutateResponse*](../../data/search/campaignsharedsetservicemutateresponse.md)
