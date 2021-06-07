# FeedSet


<div lang=\"ja\">FeedSetオブジェクトは、商品セット情報を保持します。</div> 

## Table of contents

### Properties

- [accountId](feedset.md#accountid)
- [conditionSets](feedset.md#conditionsets)
- [feedId](feedset.md#feedid)
- [feedSetId](feedset.md#feedsetid)
- [feedSetName](feedset.md#feedsetname)
- [isDefaultSet](feedset.md#isdefaultset)
- [itemCount](feedset.md#itemcount)

## Properties

### accountId

• `Optional` **accountId**: ``null`` \| *number*

<div lang=\"ja\"> アカウントIDです。<br> このフィールドは、レスポンスの際に返却されますが、リクエストの際には無視されます。 </div> 

**`memberof`** FeedSet

___

### conditionSets

• `Optional` **conditionSets**: ``null`` \| [*FeedSetServiceConditionSet*](feedsetserviceconditionset.md)[]

**`memberof`** FeedSet

___

### feedId

• `Optional` **feedId**: ``null`` \| *number*

<div lang=\"ja\"> Feedを識別するIDです。<br> このフィールドは、リクエストの場合は必須です。 </div> 

**`memberof`** FeedSet

___

### feedSetId

• `Optional` **feedSetId**: ``null`` \| *number*

<div lang=\"ja\"> 商品セットIDです。<br> REMOVE時、このフィールドは必須です。 </div> 

**`memberof`** FeedSet

___

### feedSetName

• `Optional` **feedSetName**: ``null`` \| *string*

<div lang=\"ja\"> 商品セット名です。<br> ADD時、このフィールドは必須です。 </div> 

**`memberof`** FeedSet

___

### isDefaultSet

• `Optional` **isDefaultSet**: ``null`` \| *boolean*

<div lang=\"ja\"> デフォルトセット判定です。<br> このフィールドは、レスポンスの際に返却されますが、リクエストの際には無視されます。 </div> 

**`memberof`** FeedSet

___

### itemCount

• `Optional` **itemCount**: ``null`` \| *number*

<div lang=\"ja\"> 商品セットの条件に含まれるアイテム数です。<br> このフィールドは、レスポンスの際に返却されますが、リクエストの際には無視されます。 </div> 

**`memberof`** FeedSet
