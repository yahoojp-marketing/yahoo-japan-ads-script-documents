# CampaignServiceTargetRoasBiddingScheme


<div lang=\"ja\">CampaignServiceTargetRoasBiddingSchemeオブジェクトは、広告費用対効果の目標値の自動入札設定情報を表します。 （BiddingStrategyService以外用のオブジェクトです。）<br> ADD時、BiddingStrategyTypeがTARGET_ROASの場合、必須となり、それ以外では省略可能となります。</div> 

## Table of contents

### Properties

- [bidCeiling](campaignservicetargetroasbiddingscheme.md#bidceiling)
- [bidFloor](campaignservicetargetroasbiddingscheme.md#bidfloor)
- [targetRoas](campaignservicetargetroasbiddingscheme.md#targetroas)

## Properties

### bidCeiling

• `Optional` **bidCeiling**: ``null`` \| *number*

<div lang=\"ja\">入札価格の上限です。<br>このフィールドは省略可能となります。その際、デフォルト設定値は0となります。<br> ※「0」が設定された場合、上限設定はありません。</div> 

**`memberof`** CampaignServiceTargetRoasBiddingScheme

___

### bidFloor

• `Optional` **bidFloor**: ``null`` \| *number*

<div lang=\"ja\">入札価格の下限です。<br>このフィールドは省略可能となります。その際、デフォルト設定値は0となります。<br> ※ 設定を解除する場合は「0」を指定します。</div> 

**`memberof`** CampaignServiceTargetRoasBiddingScheme

___

### targetRoas

• `Optional` **targetRoas**: ``null`` \| *number*

<div lang=\"ja\">広告費用対効果の目標値です。<br> 0.01 ～ 1000.00（1% ～ 100000%）の範囲内のみ 許容します。<br> ADD時およびSET時、このフィールドは必須となります。<br> ※ROAS:Return On Advertising Spend</div> 

**`memberof`** CampaignServiceTargetRoasBiddingScheme
