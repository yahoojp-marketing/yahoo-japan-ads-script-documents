# AdGroupFeedService


## Table of contents

### Methods

- [get](adgroupfeedservice.md#get)
- [set](adgroupfeedservice.md#set)

## Methods

### get

▸ **get**(`adGroupFeedServiceSelector?`: [*AdGroupFeedServiceSelector*](../../data/search/adgroupfeedserviceselector.md)): [*AdGroupFeedServiceGetResponse*](../../data/search/adgroupfeedservicegetresponse.md)

<div lang=\"ja\">広告グループに設定されているFeedItem情報を取得します。</div> 

#### Parameters

| Name | Type |
| :------ | :------ |
| `adGroupFeedServiceSelector?` | [*AdGroupFeedServiceSelector*](../../data/search/adgroupfeedserviceselector.md) |

**Returns:** [*AdGroupFeedServiceGetResponse*](../../data/search/adgroupfeedservicegetresponse.md)

___

### set

▸ **set**(`adGroupFeedServiceOperation?`: [*AdGroupFeedServiceOperation*](../../data/search/adgroupfeedserviceoperation.md)): [*AdGroupFeedServiceMutateResponse*](../../data/search/adgroupfeedservicemutateresponse.md)

<div lang=\"ja\">広告グループにFeedItem情報を追加・更新・解除（削除）します。更新は常に上書きされるため追加分を含めて更新する必要があります。<br> ・FeedItem情報を解除するときは空の情報で更新します。<br> ・1リクエストで異なるキャンペーン配下の広告グループに対してFeedItem情報の設定が可能です。<br> ・1つの広告グループに設定できるFeedItem情報は、QUICKLINKS、CALLEXTENSIONでそれぞれ20件までです。<br> ・CALLEXTENSIONについては1広告グループあたり1件の設定をお薦めします。<br> ・1リクエスト内で同一のadGroupIdに複数のFeedItem情報を設定できません。<br> ※現在、こちらのサービスは利用できません。</div> 

#### Parameters

| Name | Type |
| :------ | :------ |
| `adGroupFeedServiceOperation?` | [*AdGroupFeedServiceOperation*](../../data/search/adgroupfeedserviceoperation.md) |

**Returns:** [*AdGroupFeedServiceMutateResponse*](../../data/search/adgroupfeedservicemutateresponse.md)
