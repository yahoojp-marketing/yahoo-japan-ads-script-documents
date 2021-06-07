# Feed


<div lang=\"ja\">Feedオブジェクトは、Feed情報を保持します。</div> 

## Table of contents

### Properties

- [accountId](feed.md#accountid)
- [approvedItemCount](feed.md#approveditemcount)
- [disApprovedItemCount](feed.md#disapproveditemcount)
- [feedId](feed.md#feedid)
- [feedName](feed.md#feedname)
- [itemCount](feed.md#itemcount)

## Properties

### accountId

• `Optional` **accountId**: ``null`` \| *number*

<div lang=\"ja\"> アカウントIDです。<br> このフィールドは、リクエストの場合は必須です。 </div> 

**`memberof`** Feed

___

### approvedItemCount

• `Optional` **approvedItemCount**: ``null`` \| *number*

<div lang=\"ja\"> 審査済みアイテム数です。<br> このフィールドは、レスポンスの際に返却されますが、リクエストの際には無視されます。 </div> 

**`memberof`** Feed

___

### disApprovedItemCount

• `Optional` **disApprovedItemCount**: ``null`` \| *number*

<div lang=\"ja\"> 審査否認アイテム数です。<br> このフィールドは、レスポンスの際に返却されますが、リクエストの際には無視されます。 </div> 

**`memberof`** Feed

___

### feedId

• `Optional` **feedId**: ``null`` \| *number*

<div lang=\"ja\"> Feedを識別するIDです。<br> SET時およびREMOVE時、このフィールドは必須です。 </div> 

**`memberof`** Feed

___

### feedName

• `Optional` **feedName**: ``null`` \| *string*

<div lang=\"ja\"> Feedを識別する名称です。<br> このフィールドは、ADD時は必須となり、SET時は省略可能となります。 </div> 

**`memberof`** Feed

___

### itemCount

• `Optional` **itemCount**: ``null`` \| *number*

<div lang=\"ja\"> アイテム数です。<br> このフィールドは、レスポンスの際に返却されますが、リクエストの際には無視されます。 </div> 

**`memberof`** Feed
