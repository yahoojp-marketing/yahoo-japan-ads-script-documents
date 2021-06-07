# Label


<div lang=\"ja\">Labelオブジェクトは、ラベルの情報を表します。</div> 

## Table of contents

### Properties

- [accountId](label.md#accountid)
- [color](label.md#color)
- [description](label.md#description)
- [labelId](label.md#labelid)
- [labelName](label.md#labelname)

## Properties

### accountId

• `Optional` **accountId**: ``null`` \| *number*

<div lang=\"ja\"> アカウントIDです。<br> このフィールドは、レスポンスの際に返却されますが、リクエストの際には無視されます。 </div> 

**`memberof`** Label

___

### color

• `Optional` **color**: ``null`` \| *string*

<div lang=\"ja\"> カラーです。<br> ADD時およびSET時、このフィールドは省略可能となります。ADD時のデフォルト設定値は#FFFFFFとなります。 </div> 

**`memberof`** Label

___

### description

• `Optional` **description**: ``null`` \| *string*

<div lang=\"ja\"> 説明文です。<br> ADD時およびSET時、このフィールドは省略可能となります。 </div> 

**`memberof`** Label

___

### labelId

• `Optional` **labelId**: ``null`` \| *number*

<div lang=\"ja\"> ラベルIDです。<br> SET時およびREMOVE時、このフィールドは必須です。 </div> 

**`memberof`** Label

___

### labelName

• `Optional` **labelName**: ``null`` \| *string*

<div lang=\"ja\"> ラベル名です。<br> このフィールドは、ADD時は必須となり、SET時は省略可能となります。 </div> 

**`memberof`** Label
