# CampaignServiceTargetCpaBiddingScheme


<div lang=\"ja\">CampaignServiceTargetCpaBiddingSchemeオブジェクトは、コンバージョン単価の目標値の自動入札設定情報を表します。 （BiddingStrategyService以外用のオブジェクトです。）<br> ADD時、BiddingStrategyTypeがTARGET_CPAの場合、必須となり、それ以外では省略可能となります。</div> 

## Table of contents

### Properties

- [bidCeiling](campaignservicetargetcpabiddingscheme.md#bidceiling)
- [bidFloor](campaignservicetargetcpabiddingscheme.md#bidfloor)
- [targetCpa](campaignservicetargetcpabiddingscheme.md#targetcpa)

## Properties

### bidCeiling

• `Optional` **bidCeiling**: ``null`` \| *number*

<div lang=\"ja\">入札価格の上限です。<br> このフィールドの追加と編集は廃止され、現在設定できません。</div> 

**`memberof`** CampaignServiceTargetCpaBiddingScheme

___

### bidFloor

• `Optional` **bidFloor**: ``null`` \| *number*

<div lang=\"ja\">入札価格の下限です。<br> このフィールドの追加と編集は廃止され、現在設定できません。</div> 

**`memberof`** CampaignServiceTargetCpaBiddingScheme

___

### targetCpa

• `Optional` **targetCpa**: ``null`` \| *number*

<div lang=\"ja\">コンバージョン単価の目標値です。<br> ADD時およびSET時、このフィールドは必須となります。<br> ※制限値：1 ～ 800000<br>※日本円のみの設定です。</div> 

**`memberof`** CampaignServiceTargetCpaBiddingScheme
