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

<div lang=\"ja\">入札価格の上限です。<br>このフィールドの追加と編集は廃止され、現在設定できません。</div> 

**`memberof`** CampaignServiceTargetRoasBiddingScheme

___

### bidFloor

• `Optional` **bidFloor**: ``null`` \| *number*

<div lang=\"ja\">入札価格の下限です。<br>このフィールドの追加と編集は廃止され、現在設定できません。</div> 

**`memberof`** CampaignServiceTargetRoasBiddingScheme

___

### targetRoas

• `Optional` **targetRoas**: ``null`` \| *number*

<div lang=\"ja\">広告費用対効果の目標値です。<br> 0.01 ～ 1000.00（1% ～ 100000%）の範囲内のみ 許容します。<br> ADD時およびSET時、このフィールドは必須となります。<br> ※ROAS:Return On Advertising Spend</div> 

**`memberof`** CampaignServiceTargetRoasBiddingScheme
