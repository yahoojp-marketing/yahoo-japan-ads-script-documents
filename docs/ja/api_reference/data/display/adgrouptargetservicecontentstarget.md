# AdGroupTargetServiceContentsTarget


<div lang=\"ja\"> AdGroupTargetServiceContentsTargetオブジェクトは、コンテンツターゲティングの設定情報を保持します。<br> ADD、SETおよびREPLACE時、このフィールドは省略可能となります。<br> ※targetTypeがCONTENTS_TARGETの場合は必須です。<br> ※現在利用できません </div> 

## Table of contents

### Properties

- [contentsKeywordListName](adgrouptargetservicecontentstarget.md#contentskeywordlistname)
- [targetListDeliverType](adgrouptargetservicecontentstarget.md#targetlistdelivertype)

## Properties

### contentsKeywordListName

• `Optional` **contentsKeywordListName**: ``null`` \| *string*

<div lang=\"ja\"> コンテンツキーワードリスト名です。<br> このフィールドは、レスポンスの際に返却されますが、リクエストの際には無視されます。 </div> 

**`memberof`** AdGroupTargetServiceContentsTarget

___

### targetListDeliverType

• `Optional` **targetListDeliverType**: ``null`` \| [*Include*](./enums/adgrouptargetservicetargetlistdelivertype.md#include) \| [*Exclude*](./enums/adgrouptargetservicetargetlistdelivertype.md#exclude) \| [*Unknown*](./enums/adgrouptargetservicetargetlistdelivertype.md#unknown)

**`memberof`** AdGroupTargetServiceContentsTarget
