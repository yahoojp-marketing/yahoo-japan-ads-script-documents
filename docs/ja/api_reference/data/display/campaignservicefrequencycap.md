# CampaignServiceFrequencyCap


<div lang=\"ja\"> CampaignServiceFrequencyCapは、フリークエンシー制御を表します。<br> このフィールドは、ADDおよびSET時に省略可能となり、REMOVE時に無視されます。<br> ※ADDおよびSET時、目的ありの場合は設定不可となります。<br> ※ADD時、このフィールドは指定できません。<br> ※SET時は更新する項目のみのリクエストが可能です。<br> ※フリークエンシーキャップの解除方法は、以下の通りです： </div>  <code> {   \"frequencyCap\": {     \"impression\": 0   } } </code>

## Table of contents

### Properties

- [frequencyLevel](campaignservicefrequencycap.md#frequencylevel)
- [frequencyTimeUnit](campaignservicefrequencycap.md#frequencytimeunit)
- [impression](campaignservicefrequencycap.md#impression)

## Properties

### frequencyLevel

• `Optional` **frequencyLevel**: ``null`` \| [*Campaign*](./enums/campaignservicefrequencylevel.md#campaign) \| [*AdGroup*](./enums/campaignservicefrequencylevel.md#adgroup) \| [*Ad*](./enums/campaignservicefrequencylevel.md#ad) \| [*Unknown*](./enums/campaignservicefrequencylevel.md#unknown)

**`memberof`** CampaignServiceFrequencyCap

___

### frequencyTimeUnit

• `Optional` **frequencyTimeUnit**: ``null`` \| [*Day*](./enums/campaignservicefrequencytimeunit.md#day) \| [*Week*](./enums/campaignservicefrequencytimeunit.md#week) \| [*Month*](./enums/campaignservicefrequencytimeunit.md#month) \| [*Unknown*](./enums/campaignservicefrequencytimeunit.md#unknown)

**`memberof`** CampaignServiceFrequencyCap

___

### impression

• `Optional` **impression**: ``null`` \| *number*

<div lang=\"ja\"> 同一ユーザに対する広告の最大インプレッション数です。<br> このフィールドは、ADDおよびSET時に省略可能となります。 </div> 

**`memberof`** CampaignServiceFrequencyCap
