# AdGroupWebpageServiceBid


<div lang=\"ja\">AdGroupWebpageServiceBidオブジェクトは、入札価格を表示します。 （AdGroupWebpageService用のオブジェクトです。）<br> ADD時およびSET時、このフィールドは省略可能となります。※ExcludedTypeがINCLUDEDのみ更新可能です。</div> 

## Table of contents

### Properties

- [adGroupMaxCpc](adgroupwebpageservicebid.md#adgroupmaxcpc)
- [bidSource](adgroupwebpageservicebid.md#bidsource)
- [keywordMaxCpc](adgroupwebpageservicebid.md#keywordmaxcpc)
- [maxCpc](adgroupwebpageservicebid.md#maxcpc)

## Properties

### adGroupMaxCpc

• `Optional` **adGroupMaxCpc**: ``null`` \| *number*

<div lang=\"ja\">広告グループの最大入札価格です。<br>このフィールドは、レスポンスの際に返却されますが、リクエストの際には無視されます。</div> 

**`memberof`** AdGroupWebpageServiceBid

___

### bidSource

• `Optional` **bidSource**: ``null`` \| [*Adgroup*](./enums/adgroupwebpageservicebidsource.md#adgroup) \| [*Criterion*](./enums/adgroupwebpageservicebidsource.md#criterion) \| [*Unknown*](./enums/adgroupwebpageservicebidsource.md#unknown)

**`memberof`** AdGroupWebpageServiceBid

___

### keywordMaxCpc

• `Optional` **keywordMaxCpc**: ``null`` \| *number*

<div lang=\"ja\">キーワードの最大入札価格です。<br>このフィールドは、レスポンスの際に返却されますが、リクエストの際には無視されます。</div> 

**`memberof`** AdGroupWebpageServiceBid

___

### maxCpc

• `Optional` **maxCpc**: ``null`` \| *number*

<div lang=\"ja\">最大入札価格です。<br>ADD時、このフィールドは省略可能となります。その際、デフォルト値は1となります。SET時、このフィールドは省略可能となります。</div> 

**`memberof`** AdGroupWebpageServiceBid
