# BiddingStrategyServiceTargetCpaBiddingScheme


<div lang=\"ja\">BiddingStrategyServiceTargetCpaBiddingSchemeオブジェクトは、コンバージョン単価の目標値の自動入札設定情報を表します。<br> このフィールドは、省略可能となります。※ADD時、typeがTARGET_CPAの場合は必須です。</div> 

## Table of contents

### Properties

- [bidCeiling](biddingstrategyservicetargetcpabiddingscheme.md#bidceiling)
- [bidFloor](biddingstrategyservicetargetcpabiddingscheme.md#bidfloor)
- [targetCpa](biddingstrategyservicetargetcpabiddingscheme.md#targetcpa)

## Properties

### bidCeiling

• `Optional` **bidCeiling**: ``null`` \| *number*

<div lang=\"ja\">入札価格の上限です。<br>※「0」が設定された場合、上限設定はありません。<br> このフィールドは、いずれの場合でも省略可能となります。</div> 

**`memberof`** BiddingStrategyServiceTargetCpaBiddingScheme

___

### bidFloor

• `Optional` **bidFloor**: ``null`` \| *number*

<div lang=\"ja\">入札価格の下限です。<br>※ 設定を解除する場合は「0」を指定します。<br> このフィールドは、いずれの場合でも省略可能となります。</div> 

**`memberof`** BiddingStrategyServiceTargetCpaBiddingScheme

___

### targetCpa

• `Optional` **targetCpa**: ``null`` \| *number*

<div lang=\"ja\">コンバージョン単価の目標値です（日本円です）。<br> このフィールドは、ADD時は必須となり、SET時は省略可能となります。</div> 

**`memberof`** BiddingStrategyServiceTargetCpaBiddingScheme
