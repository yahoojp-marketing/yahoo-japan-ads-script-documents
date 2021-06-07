# BiddingStrategyServiceTargetImpressionShareScheme


<div lang=\"ja\">BiddingStrategyServiceTargetImpressionShareSchemeオブジェクトは、広告費用対効果の目標値の自動入札設定情報を表します。<br> このフィールドは、省略可能となります。※ADD時、typeがTARGET_IMPRESSION_SHAREの場合は必須です。</div> 

## Table of contents

### Properties

- [bidCeiling](biddingstrategyservicetargetimpressionsharescheme.md#bidceiling)
- [location](biddingstrategyservicetargetimpressionsharescheme.md#location)
- [targetImpressionShare](biddingstrategyservicetargetimpressionsharescheme.md#targetimpressionshare)

## Properties

### bidCeiling

• `Optional` **bidCeiling**: ``null`` \| *number*

<div lang=\"ja\">入札価格の上限です。（0〜50000）<br> ※「0」が設定された場合、上限設定はありません。<br> このフィールドは、いずれの場合でも省略可能となります。</div> 

**`memberof`** BiddingStrategyServiceTargetImpressionShareScheme

___

### location

• `Optional` **location**: ``null`` \| [*AnywhereOnPage*](./enums/biddingstrategyservicetargetimpressionsharelocation.md#anywhereonpage) \| [*TopOfPage*](./enums/biddingstrategyservicetargetimpressionsharelocation.md#topofpage) \| [*AbsoluteTopOfPage*](./enums/biddingstrategyservicetargetimpressionsharelocation.md#absolutetopofpage) \| [*Unknown*](./enums/biddingstrategyservicetargetimpressionsharelocation.md#unknown)

**`memberof`** BiddingStrategyServiceTargetImpressionShareScheme

___

### targetImpressionShare

• `Optional` **targetImpressionShare**: ``null`` \| *number*

<div lang=\"ja\">目標のインプレッションシェアです。<br> ADD時およびSET時、このフィールドは必須となります。</div> 

**`memberof`** BiddingStrategyServiceTargetImpressionShareScheme
