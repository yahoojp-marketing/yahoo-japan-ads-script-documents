# AdGroupTargetServicePlacementTarget


<div lang=\"ja\"> AdGroupTargetServicePlacementTargetオブジェクトは、プレイスメントターゲティングの設定情報を保持するオブジェクトです。<br> ADD、SETおよびREPLACE時、このフィールドは省略可能となります。<br> ※targetTypeがPLACEMENT_TARGETの場合は必須です。 </div> 

## Table of contents

### Properties

- [placementUrlListName](adgrouptargetserviceplacementtarget.md#placementurllistname)
- [placementUrlListType](adgrouptargetserviceplacementtarget.md#placementurllisttype)

## Properties

### placementUrlListName

• `Optional` **placementUrlListName**: ``null`` \| *string*

<div lang=\"ja\"> プレイスメントリスト名です。<br> このフィールドは、レスポンスの際に返却されますが、リクエストの際には無視されます。 </div> 

**`memberof`** AdGroupTargetServicePlacementTarget

___

### placementUrlListType

• `Optional` **placementUrlListType**: ``null`` \| [*WhiteList*](./enums/adgrouptargetserviceplacementurllisttype.md#whitelist) \| [*BlackList*](./enums/adgrouptargetserviceplacementurllisttype.md#blacklist) \| [*Unknown*](./enums/adgrouptargetserviceplacementurllisttype.md#unknown)

**`memberof`** AdGroupTargetServicePlacementTarget
