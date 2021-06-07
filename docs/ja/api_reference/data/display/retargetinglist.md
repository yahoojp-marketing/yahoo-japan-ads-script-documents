# RetargetingList


<div lang=\"ja\">RetargetingListオブジェクトは、サイトリターゲティング のターゲットリストの情報を表します。</div> 

## Table of contents

### Properties

- [accountId](retargetinglist.md#accountid)
- [deliveryStatus](retargetinglist.md#deliverystatus)
- [description](retargetinglist.md#description)
- [isRemoveDescription](retargetinglist.md#isremovedescription)
- [isShared](retargetinglist.md#isshared)
- [reach](retargetinglist.md#reach)
- [sourceAccountId](retargetinglist.md#sourceaccountid)
- [sourceAccountName](retargetinglist.md#sourceaccountname)
- [targetList](retargetinglist.md#targetlist)
- [targetListId](retargetinglist.md#targetlistid)
- [targetListName](retargetinglist.md#targetlistname)

## Properties

### accountId

• `Optional` **accountId**: ``null`` \| *number*

<div lang=\"ja\"> アカウントIDです。<br> このフィールドは、レスポンスの際に返却されますが、リクエストの際には無視されます。 </div> 

**`memberof`** RetargetingList

___

### deliveryStatus

• `Optional` **deliveryStatus**: ``null`` \| [*Active*](./enums/retargetinglistservicedeliverystatus.md#active) \| [*Paused*](./enums/retargetinglistservicedeliverystatus.md#paused) \| [*Unknown*](./enums/retargetinglistservicedeliverystatus.md#unknown)

**`memberof`** RetargetingList

___

### description

• `Optional` **description**: ``null`` \| *string*

<div lang=\"ja\"> ターゲットリストの説明です。<br> このフィールドは、ADDおよびSET時に省略可能となり、REMOVE時に無視されます。 </div> 

**`memberof`** RetargetingList

___

### isRemoveDescription

• `Optional` **isRemoveDescription**: ``null`` \| [*True*](./enums/retargetinglistserviceisremoveflg.md#true) \| [*False*](./enums/retargetinglistserviceisremoveflg.md#false) \| [*Unknown*](./enums/retargetinglistserviceisremoveflg.md#unknown)

**`memberof`** RetargetingList

___

### isShared

• `Optional` **isShared**: ``null`` \| *boolean*

<div lang=\"ja\">   RetargetingListServiceIsSharedは、ターゲットリストの共有ステータスを示します。<br>   このフィールドは、レスポンスの際に返却されますが、リクエストの際には無視されます。 </div>  <hr> <dl class=term>   <dt class=\"term__item\">TRUE</dt>   <dd class=\"term__desc\"><span lang=\"ja\">共有されたターゲットリストです。</span></dd>   <dt class=\"term__item\">FALSE</dt>   <dd class=\"term__desc\"><span lang=\"ja\">共有されていないターゲットリストです。</span></dd>   <dt class=\"term__item\">UNKNOWN</dt>   <dd class=\"term__desc\"><span lang=\"ja\">未知の値です。</span></dd> </dl>

**`memberof`** RetargetingList

___

### reach

• `Optional` **reach**: ``null`` \| *number*

<div lang=\"ja\"> リーチ数です。<br> このフィールドは、レスポンスの際に返却されますが、リクエストの際には無視されます。 </div> 

**`memberof`** RetargetingList

___

### sourceAccountId

• `Optional` **sourceAccountId**: ``null`` \| *number*

<div lang=\"ja\">   共有元アカウントIDです。<br>   このフィールドは、レスポンスの際に返却されますが、リクエストの際には無視されます。 </div> 

**`memberof`** RetargetingList

___

### sourceAccountName

• `Optional` **sourceAccountName**: ``null`` \| *string*

<div lang=\"ja\">   共有元アカウント名です。<br>   このフィールドは、レスポンスの際に返却されますが、リクエストの際には無視されます。 </div> 

**`memberof`** RetargetingList

___

### targetList

• `Optional` **targetList**: ``null`` \| [*RetargetingListServiceTargetList*](retargetinglistservicetargetlist.md)

**`memberof`** RetargetingList

___

### targetListId

• `Optional` **targetListId**: ``null`` \| *number*

<div lang=\"ja\"> ターゲットリストIDです。<br> このフィールドは、SETおよびREMOVE時に必須となり、ADD時には無視されます。 </div> 

**`memberof`** RetargetingList

___

### targetListName

• `Optional` **targetListName**: ``null`` \| *string*

<div lang=\"ja\"> ターゲットリスト名です。<br> このフィールドは、ADD時は必須、SET時は省略可能となり、REMOVE時は無視されます。 </div> 

**`memberof`** RetargetingList
