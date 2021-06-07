# FeedServiceAttribute


<div lang=\"ja\">FeedServiceAttributeオブジェクトは、自動データ挿入のリストの属性を格納します。<br> このフィールドは、ADDおよびSET時に省略可能となり、REMOVE時に無視されます。</div> 

## Table of contents

### Properties

- [feedAttributeId](feedserviceattribute.md#feedattributeid)
- [feedAttributeName](feedserviceattribute.md#feedattributename)
- [placeholderField](feedserviceattribute.md#placeholderfield)

## Properties

### feedAttributeId

• `Optional` **feedAttributeId**: ``null`` \| *number*

<div lang=\"ja\">自動データ挿入のリストの属性（カラム）IDです。<br> このフィールドは、レスポンスの際に返却されますが、リクエストの際には無視されます。</div> 

**`memberof`** FeedServiceAttribute

___

### feedAttributeName

• `Optional` **feedAttributeName**: ``null`` \| *string*

<div lang=\"ja\">自動データ挿入のリストの属性（カラム）名です。<br> このフィールドはADDおよびSET時に必須となり、REMOVE時に無視されます。</div> 

**`memberof`** FeedServiceAttribute

___

### placeholderField

• `Optional` **placeholderField**: ``null`` \| [*AdCustomizerInteger*](./enums/feedserviceplaceholderfield.md#adcustomizerinteger) \| [*AdCustomizerPrice*](./enums/feedserviceplaceholderfield.md#adcustomizerprice) \| [*AdCustomizerDate*](./enums/feedserviceplaceholderfield.md#adcustomizerdate) \| [*AdCustomizerString*](./enums/feedserviceplaceholderfield.md#adcustomizerstring) \| [*DynamicAdForSearchPageFeedsPageUrl*](./enums/feedserviceplaceholderfield.md#dynamicadforsearchpagefeedspageurl) \| [*DynamicAdForSearchPageFeedsLabel*](./enums/feedserviceplaceholderfield.md#dynamicadforsearchpagefeedslabel) \| [*Unknown*](./enums/feedserviceplaceholderfield.md#unknown)

**`memberof`** FeedServiceAttribute
