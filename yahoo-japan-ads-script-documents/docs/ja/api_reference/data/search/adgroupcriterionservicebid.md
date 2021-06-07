# AdGroupCriterionServiceBid


<div lang=\"ja\">AdGroupCriterionServiceBidオブジェクトは、入札価格を表示します。 （AdGroupCriterionService用のオブジェクトです。）<br> ADDおよびSET時、このフィールドは省略可能となります。</div> 

## Table of contents

### Properties

- [adGroupMaxCpc](adgroupcriterionservicebid.md#adgroupmaxcpc)
- [bidSource](adgroupcriterionservicebid.md#bidsource)
- [keywordMaxCpc](adgroupcriterionservicebid.md#keywordmaxcpc)
- [maxCpc](adgroupcriterionservicebid.md#maxcpc)

## Properties

### adGroupMaxCpc

• `Optional` **adGroupMaxCpc**: ``null`` \| *number*

<div lang=\"ja\">広告グループ入札価格です。</div> 

**`memberof`** AdGroupCriterionServiceBid

___

### bidSource

• `Optional` **bidSource**: ``null`` \| [*Adgroup*](./enums/adgroupcriterionservicebidsource.md#adgroup) \| [*Criterion*](./enums/adgroupcriterionservicebidsource.md#criterion) \| [*Unknown*](./enums/adgroupcriterionservicebidsource.md#unknown)

**`memberof`** AdGroupCriterionServiceBid

___

### keywordMaxCpc

• `Optional` **keywordMaxCpc**: ``null`` \| *number*

<div lang=\"ja\">キーワード入札価格です。</div> 

**`memberof`** AdGroupCriterionServiceBid

___

### maxCpc

• `Optional` **maxCpc**: ``null`` \| *number*

<div lang=\"ja\">キーワード入札価格です。<br> このフィールドは、省略可能となります。その際、ADD時のデフォルト設定値は1となります。<br> ※maxCpcが0の場合は、設定なしと同様です。</div> 

**`memberof`** AdGroupCriterionServiceBid
