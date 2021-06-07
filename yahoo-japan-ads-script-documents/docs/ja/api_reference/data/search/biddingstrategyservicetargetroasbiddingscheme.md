# BiddingStrategyServiceTargetRoasBiddingScheme


<div lang=\"ja\">BiddingStrategyServiceTargetRoasBiddingSchemeオブジェクトは、広告費用対効果の目標値の自動入札設定情報を表します。<br> このフィールドは、省略可能となります。※ADD時、typeがTARGET_ROASの場合は必須です。</div> 

## Table of contents

### Properties

- [bidCeiling](biddingstrategyservicetargetroasbiddingscheme.md#bidceiling)
- [bidFloor](biddingstrategyservicetargetroasbiddingscheme.md#bidfloor)
- [targetRoas](biddingstrategyservicetargetroasbiddingscheme.md#targetroas)

## Properties

### bidCeiling

• `Optional` **bidCeiling**: ``null`` \| *number*

<div lang=\"ja\">入札価格の上限です。（0〜50000）<br> ※「0」が設定された場合、上限設定はありません。<br> このフィールドは、いずれの場合でも省略可能となります。</div> 

**`memberof`** BiddingStrategyServiceTargetRoasBiddingScheme

___

### bidFloor

• `Optional` **bidFloor**: ``null`` \| *number*

<div lang=\"ja\">入札価格の下限です。<br> ※ 設定を解除する場合は「0」を指定します。<br> このフィールドは、いずれの場合でも省略可能となります。</div> 

**`memberof`** BiddingStrategyServiceTargetRoasBiddingScheme

___

### targetRoas

• `Optional` **targetRoas**: ``null`` \| *number*

<div lang=\"ja\">広告費用対効果の目標値<br> ※0.01 〜1000.00（1%〜100000%）の範囲内のみ許容します。<br> このフィールドは、ADD時は必須となり、SET時は省略可能となります。※Return On Advertising Spend(ROAS)</div> 

**`memberof`** BiddingStrategyServiceTargetRoasBiddingScheme
