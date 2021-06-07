# RetargetingListServiceSelector


<div lang=\"ja\">RetargetingListServiceSelectorは、ターゲットリストの検索条件（実行パラメータ）を保持するオブジェクトです。</div> 

## Table of contents

### Properties

- [accountId](retargetinglistserviceselector.md#accountid)
- [numberResults](retargetinglistserviceselector.md#numberresults)
- [startIndex](retargetinglistserviceselector.md#startindex)
- [targetListIds](retargetinglistserviceselector.md#targetlistids)
- [targetListOwner](retargetinglistserviceselector.md#targetlistowner)
- [targetListTypes](retargetinglistserviceselector.md#targetlisttypes)

## Properties

### accountId

• **accountId**: *number*

<div lang=\"ja\">検索条件：アカウントIDです。</div> 

**`memberof`** RetargetingListServiceSelector

___

### numberResults

• `Optional` **numberResults**: ``null`` \| *number*

<div lang=\"ja\">ページの最大件数です。このフィールドは、1以上を指定する必要があります。</div> 

**`memberof`** RetargetingListServiceSelector

___

### startIndex

• `Optional` **startIndex**: ``null`` \| *number*

<div lang=\"ja\">ページの先頭のインデックスです。このフィールドは、1以上を指定する必要があります。</div> 

**`memberof`** RetargetingListServiceSelector

___

### targetListIds

• `Optional` **targetListIds**: ``null`` \| *number*[]

<div lang=\"ja\">検索条件：ターゲットリストIDです。</div> 

**`memberof`** RetargetingListServiceSelector

___

### targetListOwner

• `Optional` **targetListOwner**: ``null`` \| [*Owner*](./enums/retargetinglistservicetargetlistowner.md#owner) \| [*Shared*](./enums/retargetinglistservicetargetlistowner.md#shared) \| [*Unknown*](./enums/retargetinglistservicetargetlistowner.md#unknown)

**`memberof`** RetargetingListServiceSelector

___

### targetListTypes

• `Optional` **targetListTypes**: ``null`` \| [*RetargetingListServiceTargetListType*](./enums/retargetinglistservicetargetlisttype.md)[]

**`memberof`** RetargetingListServiceSelector
