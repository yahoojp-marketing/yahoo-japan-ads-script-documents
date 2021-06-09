# GuaranteedInventoryServiceSiteRetargetingTarget


<div lang=\"ja\"> GuaranteedInventoryServiceSiteRetargetingTargetオブジェクトは、サイトリターゲティングの設定情報を保持します。<br> ADD時、このフィールドは省略可能となります。<br> ※targetTypeがSITE_RETARGETINGの場合は必須です。 </div> 

## Table of contents

### Properties

- [accountId](guaranteedinventoryservicesiteretargetingtarget.md#accountid)
- [accountName](guaranteedinventoryservicesiteretargetingtarget.md#accountname)
- [deliverType](guaranteedinventoryservicesiteretargetingtarget.md#delivertype)
- [targetListName](guaranteedinventoryservicesiteretargetingtarget.md#targetlistname)

## Properties

### accountId

• `Optional` **accountId**: ``null`` \| *number*

<div lang=\"ja\"> アカウントIDです。<br> このフィールドは、ADD時は必須となります。 </div> 

**`memberof`** GuaranteedInventoryServiceSiteRetargetingTarget

___

### accountName

• `Optional` **accountName**: ``null`` \| *string*

<div lang=\"ja\"> アカウント名です。<br> このフィールドは、レスポンスの際に返却されますが、リクエストの際には無視されます。 </div> 

**`memberof`** GuaranteedInventoryServiceSiteRetargetingTarget

___

### deliverType

• `Optional` **deliverType**: ``null`` \| [*Include*](./enums/guaranteedinventoryservicetargetlistdelivertype.md#include) \| [*Exclude*](./enums/guaranteedinventoryservicetargetlistdelivertype.md#exclude) \| [*Unknown*](./enums/guaranteedinventoryservicetargetlistdelivertype.md#unknown)

**`memberof`** GuaranteedInventoryServiceSiteRetargetingTarget

___

### targetListName

• `Optional` **targetListName**: ``null`` \| *string*

<div lang=\"ja\"> ターゲットリスト名です。<br> このフィールドは、レスポンスの際に返却されますが、リクエストの際には無視されます。 </div> 

**`memberof`** GuaranteedInventoryServiceSiteRetargetingTarget
