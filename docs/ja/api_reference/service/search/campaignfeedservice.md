# CampaignFeedService


## Table of contents

### Methods

- [get](campaignfeedservice.md#get)
- [set](campaignfeedservice.md#set)

## Methods

### get

▸ **get**(`campaignFeedServiceSelector?`: [*CampaignFeedServiceSelector*](../../data/search/campaignfeedserviceselector.md)): [*CampaignFeedServiceGetResponse*](../../data/search/campaignfeedservicegetresponse.md)

<div lang=\"ja\">キャンペーンのFeedItem情報を取得します。</div> 

#### Parameters

| Name | Type |
| :------ | :------ |
| `campaignFeedServiceSelector?` | [*CampaignFeedServiceSelector*](../../data/search/campaignfeedserviceselector.md) |

**Returns:** [*CampaignFeedServiceGetResponse*](../../data/search/campaignfeedservicegetresponse.md)

___

### set

▸ **set**(`campaignFeedServiceOperation?`: [*CampaignFeedServiceOperation*](../../data/search/campaignfeedserviceoperation.md)): [*CampaignFeedServiceMutateResponse*](../../data/search/campaignfeedservicemutateresponse.md)

<div lang=\"ja\">キャンペーンにFeedItem情報を追加・更新・解除（削除）します。<br> ・FeedItem情報を解除するときは空の情報で更新します。<br> ・1つのキャンペーンに設定できるFeedItem情報は、QUICKLINKS、CALLEXTENSIONでそれぞれ20件までです。<br> ・CALLEXTENSIONについて1キャンペーンあたり1件の設定をお薦めします。<br> ・1リクエスト内で同一のcampaignIdに複数のFeedItem情報は設定できません。<br> ※現在、こちらのサービスは利用できません。 </div>

#### Parameters

| Name | Type |
| :------ | :------ |
| `campaignFeedServiceOperation?` | [*CampaignFeedServiceOperation*](../../data/search/campaignfeedserviceoperation.md) |

**Returns:** [*CampaignFeedServiceMutateResponse*](../../data/search/campaignfeedservicemutateresponse.md)
