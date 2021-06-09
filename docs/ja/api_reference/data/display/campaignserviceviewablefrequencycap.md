# CampaignServiceViewableFrequencyCap


<div lang=\"ja\"> CampaignServiceViewableFrequencyCapは、ビューアブルフリークエンシー制御を表します。<br> ADDおよびSET時、このフィールドは目的なしの場合は設定不可となり、目的ありの場合は省略可能となります。<br> REMOVE時は無視されます。<br> ※ADD時は全ての項目の指定が必須です。<br> ※SET時は更新する項目のみのリクエストが可能です。<br> ※ビューアブルフリークエンシーキャップの解除方法は、以下の通りです： </div>  <code> {     \"viewableFrequencyCap\": {         \"vImps\": 0     } } </code>

## Table of contents

### Properties

- [frequencyLevel](campaignserviceviewablefrequencycap.md#frequencylevel)
- [frequencyTimeUnit](campaignserviceviewablefrequencycap.md#frequencytimeunit)
- [vImps](campaignserviceviewablefrequencycap.md#vimps)

## Properties

### frequencyLevel

• `Optional` **frequencyLevel**: ``null`` \| [*Campaign*](./enums/campaignservicefrequencylevel.md#campaign) \| [*AdGroup*](./enums/campaignservicefrequencylevel.md#adgroup) \| [*Ad*](./enums/campaignservicefrequencylevel.md#ad) \| [*Unknown*](./enums/campaignservicefrequencylevel.md#unknown)

**`memberof`** CampaignServiceViewableFrequencyCap

___

### frequencyTimeUnit

• `Optional` **frequencyTimeUnit**: ``null`` \| [*Day*](./enums/campaignservicefrequencytimeunit.md#day) \| [*Week*](./enums/campaignservicefrequencytimeunit.md#week) \| [*Month*](./enums/campaignservicefrequencytimeunit.md#month) \| [*Unknown*](./enums/campaignservicefrequencytimeunit.md#unknown)

**`memberof`** CampaignServiceViewableFrequencyCap

___

### vImps

• `Optional` **vImps**: ``null`` \| *number*

<div lang=\"ja\"> 同一ユーザに対する広告の最大ビューアブルインプレッション数です。<br> このフィールドは、ADDおよびSET時に省略可能となります。 </div> 

**`memberof`** CampaignServiceViewableFrequencyCap
