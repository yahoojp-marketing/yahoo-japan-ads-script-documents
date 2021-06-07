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

<div lang=\"ja\">入札価格の上限です。<br> このフィールドは省略可能となります。その際、デフォルト設定値は0となります。<br> ※「0」が設定された場合、上限設定はありません。</div> 

**`memberof`** CampaignServiceTargetCpaBiddingScheme

___

### bidFloor

• `Optional` **bidFloor**: ``null`` \| *number*

<div lang=\"ja\">入札価格の下限です。<br> このフィールドは省略可能となります。その際、デフォルト設定値は0となります。<br> ※ 設定を解除する場合は「0」を指定します。</div> 

**`memberof`** CampaignServiceTargetCpaBiddingScheme

___

### targetCpa

• `Optional` **targetCpa**: ``null`` \| *number*

<div lang=\"ja\">コンバージョン単価の目標値です。<br> ADD時およびSET時、このフィールドは必須となります。<br> ※制限値：0 ～ 99999999<br>※日本円のみの設定です。</div> 

**`memberof`** CampaignServiceTargetCpaBiddingScheme
