# PlacementUrlList


<div lang=\"ja\">PlacementUrlListオブジェクトは、プレイスメントUrl情報を保持するオブジェクトです。</div> 

## Table of contents

### Properties

- [accountId](placementurllist.md#accountid)
- [brandSafetyDenyListFlg](placementurllist.md#brandsafetydenylistflg)
- [description](placementurllist.md#description)
- [isRemoveDescription](placementurllist.md#isremovedescription)
- [unknownDomainFlg](placementurllist.md#unknowndomainflg)
- [urlListId](placementurllist.md#urllistid)
- [urlListName](placementurllist.md#urllistname)
- [urls](placementurllist.md#urls)

## Properties

### accountId

• **accountId**: *number*

<div lang=\"ja\"> アカウントIDです。<br> このフィールドは、リクエストの場合は必須です。 </div> 

**`memberof`** PlacementUrlList

___

### brandSafetyDenyListFlg

• `Optional` **brandSafetyDenyListFlg**: ``null`` \| *boolean*

<div lang=\"ja\"> 除外専用リストかどうかのフラグです。<br> 除外専用リストには下記の制約があります。<br> ・１アカウントにつき1つ作成が可能です。<br> ・除外にのみ紐付け可能です。<br> ・YDNキャンペーンには紐付けできません。<br> このフィールドは、ADD時に省略可能(デフォルトの値はFALSE)、SET時に指定不可となります。 </div>  <hr> <p>* <code>TRUE</code> - <span lang=\"ja\">除外専用リストです。</span></p> <p>* <code>FALSE</code> - <span lang=\"ja\">通常のurlリストです。</span></p>

**`memberof`** PlacementUrlList

___

### description

• `Optional` **description**: ``null`` \| *string*

<div lang=\"ja\"> urlリストの説明です。<br> このフィールドは、ADDおよびSET時に省略可能となります。 </div> 

**`memberof`** PlacementUrlList

___

### isRemoveDescription

• `Optional` **isRemoveDescription**: ``null`` \| [*True*](./enums/placementurllistserviceisremoveflg.md#true) \| [*False*](./enums/placementurllistserviceisremoveflg.md#false) \| [*Unknown*](./enums/placementurllistserviceisremoveflg.md#unknown)

**`memberof`** PlacementUrlList

___

### unknownDomainFlg

• `Optional` **unknownDomainFlg**: ``null`` \| [*True*](./enums/placementurllistserviceunknowndomainflg.md#true) \| [*False*](./enums/placementurllistserviceunknowndomainflg.md#false) \| [*Unknown*](./enums/placementurllistserviceunknowndomainflg.md#unknown)

**`memberof`** PlacementUrlList

___

### urlListId

• `Optional` **urlListId**: ``null`` \| *number*

<div lang=\"ja\"> urlリストIDです。<br> このフィールドは、SETおよびREMOVE時に必須となります。 </div> 

**`memberof`** PlacementUrlList

___

### urlListName

• `Optional` **urlListName**: ``null`` \| *string*

<div lang=\"ja\"> urlリスト名です。<br> このフィールドは、ADD時に必須となり、SET時に省略可能となります。 </div> 

**`memberof`** PlacementUrlList

___

### urls

• `Optional` **urls**: ``null`` \| [*PlacementUrlListServiceUrlList*](placementurllistserviceurllist.md)[]

**`memberof`** PlacementUrlList
