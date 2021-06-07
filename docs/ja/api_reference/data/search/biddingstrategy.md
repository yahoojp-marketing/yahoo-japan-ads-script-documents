# BiddingStrategy


<div lang=\"ja\">BiddingStrategyオブジェクトは、入札方法を表します。</div> 

## Table of contents

### Properties

- [accountId](biddingstrategy.md#accountid)
- [biddingScheme](biddingstrategy.md#biddingscheme)
- [biddingStrategyId](biddingstrategy.md#biddingstrategyid)
- [biddingStrategyName](biddingstrategy.md#biddingstrategyname)
- [type](biddingstrategy.md#type)

## Properties

### accountId

• `Optional` **accountId**: ``null`` \| *number*

<div lang=\"ja\">アカウントIDです。<br> このフィールドは、いずれの場合でも必須です。</div> 

**`memberof`** BiddingStrategy

___

### biddingScheme

• `Optional` **biddingScheme**: ``null`` \| [*BiddingStrategyServiceBiddingScheme*](biddingstrategyservicebiddingscheme.md)

**`memberof`** BiddingStrategy

___

### biddingStrategyId

• `Optional` **biddingStrategyId**: ``null`` \| *number*

<div lang=\"ja\">自動入札IDです。<br> SET時およびREMOVE時、このフィールドは必須となります。</div> 

**`memberof`** BiddingStrategy

___

### biddingStrategyName

• `Optional` **biddingStrategyName**: ``null`` \| *string*

<div lang=\"ja\">自動入札名です（50文字以内になります）。<br> このフィールドは、ADD時は必須となり、SET時は省略可能となります。</div> 

**`memberof`** BiddingStrategy

___

### type

• `Optional` **type**: ``null`` \| [*TargetRoas*](./enums/biddingstrategyservicetype.md#targetroas) \| [*TargetSpend*](./enums/biddingstrategyservicetype.md#targetspend) \| [*TargetCpa*](./enums/biddingstrategyservicetype.md#targetcpa) \| [*TargetImpressionShare*](./enums/biddingstrategyservicetype.md#targetimpressionshare) \| [*Unknown*](./enums/biddingstrategyservicetype.md#unknown)

**`memberof`** BiddingStrategy
