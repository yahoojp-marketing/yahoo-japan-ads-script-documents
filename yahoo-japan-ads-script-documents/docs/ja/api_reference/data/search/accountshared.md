# AccountShared


<div lang=\"ja\">AccountSharedオブジェクトは、アカウント内で共有できる対象外キーワードリストの情報を表します。</div> 

## Table of contents

### Properties

- [accountId](accountshared.md#accountid)
- [memberCount](accountshared.md#membercount)
- [name](accountshared.md#name)
- [referenceCount](accountshared.md#referencecount)
- [sharedListId](accountshared.md#sharedlistid)

## Properties

### accountId

• `Optional` **accountId**: ``null`` \| *number*

<div lang=\"ja\">アカウントIDです。</div> 

**`memberof`** AccountShared

___

### memberCount

• `Optional` **memberCount**: ``null`` \| *number*

<div lang=\"ja\">対象外キーワードリストに含まれるアイテム（検索対象外キーワード）数です。</div> 

**`memberof`** AccountShared

___

### name

• `Optional` **name**: ``null`` \| *string*

<div lang=\"ja\">対象外キーワードリスト名です。<br>ADDおよびSET時、このフィールドは必須となります。</div> 

**`memberof`** AccountShared

___

### referenceCount

• `Optional` **referenceCount**: ``null`` \| *number*

<div lang=\"ja\">対象外キーワードリストを使用している キャンペーン数です。</div> 

**`memberof`** AccountShared

___

### sharedListId

• `Optional` **sharedListId**: ``null`` \| *number*

<div lang=\"ja\">対象外キーワードリストIDです。<br>SETおよびREMOVE時、このフィールドは必須となります。</div> 

**`memberof`** AccountShared
