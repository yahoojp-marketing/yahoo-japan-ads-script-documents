# LabelServiceSelector


<div lang=\"ja\">LabelServiceSelectorオブジェクトは、操作の対象とするラベルの情報およびフィルタ条件を表します。</div> 

## Table of contents

### Properties

- [accountId](labelserviceselector.md#accountid)
- [labelIds](labelserviceselector.md#labelids)
- [numberResults](labelserviceselector.md#numberresults)
- [startIndex](labelserviceselector.md#startindex)

## Properties

### accountId

• **accountId**: *number*

<div lang=\"ja\">検索条件：アカウントID</div> 

**`memberof`** LabelServiceSelector

___

### labelIds

• `Optional` **labelIds**: ``null`` \| *number*[]

<div lang=\"ja\"> 検索条件：ラベルID<br> 指定しない場合は、フィルタ条件に すべてのラベルが含まれます。 </div> 

**`memberof`** LabelServiceSelector

___

### numberResults

• `Optional` **numberResults**: ``null`` \| *number*

<div lang=\"ja\">ページの最大件数です。このフィールドは、1以上を指定する必要があります。</div> 

**`memberof`** LabelServiceSelector

___

### startIndex

• `Optional` **startIndex**: ``null`` \| *number*

<div lang=\"ja\">ページの先頭のインデックスです。このフィールドは、1以上を指定する必要があります。</div> 

**`memberof`** LabelServiceSelector
