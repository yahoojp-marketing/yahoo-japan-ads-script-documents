# CampaignTarget


<div lang=\"ja\">CampaignTargetオブジェクトは、キャンペーンの各種ターゲティング設定を表します。</div> 

## Table of contents

### Properties

- [accountId](campaigntarget.md#accountid)
- [bidMultiplier](campaigntarget.md#bidmultiplier)
- [campaignId](campaigntarget.md#campaignid)
- [campaignName](campaigntarget.md#campaignname)
- [target](campaigntarget.md#target)

## Properties

### accountId

• `Optional` **accountId**: ``null`` \| *number*

<div lang=\"ja\">アカウントIDです。<br> このフィールドは、いずれの場合でも必須となります。</div> 

**`memberof`** CampaignTarget

___

### bidMultiplier

• `Optional` **bidMultiplier**: ``null`` \| *number*

<div lang=\"ja\">   入札価格調整率です。0.10～10.00まで指定できます。<br>   0を指定した場合、広告は配信されません。<br>   また、入札価格調整率の値は小数点第二位まで指定可能です。<br>   このフィールドは省略可能となります。その際、デフォルト設定値は1.0となります。 </div> 

**`memberof`** CampaignTarget

___

### campaignId

• `Optional` **campaignId**: ``null`` \| *number*

<div lang=\"ja\">キャンペーンIDです。<br> このフィールドは、いずれの場合でも必須となります。</div> 

**`memberof`** CampaignTarget

___

### campaignName

• `Optional` **campaignName**: ``null`` \| *string*

<div lang=\"ja\">キャンペーン名です。</div> 

**`memberof`** CampaignTarget

___

### target

• `Optional` **target**: ``null`` \| [*CampaignTargetServiceTarget*](campaigntargetservicetarget.md)

**`memberof`** CampaignTarget
