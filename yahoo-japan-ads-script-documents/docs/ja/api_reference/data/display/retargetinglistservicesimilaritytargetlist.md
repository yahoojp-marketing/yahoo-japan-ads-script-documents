# RetargetingListServiceSimilarityTargetList


<div lang=\"ja\"> 類似ユーザーターゲットの情報を保持するオブジェクトです。<br> このフィールドは、ADDおよびSET時に省略可能となります。<br> ※targetListTypeがSIMILARITYの場合は、ADDおよびSET時に必須となります。 </div> 

## Table of contents

### Properties

- [targetListId](retargetinglistservicesimilaritytargetlist.md#targetlistid)
- [targetListSize](retargetinglistservicesimilaritytargetlist.md#targetlistsize)
- [targetListSizeReaches](retargetinglistservicesimilaritytargetlist.md#targetlistsizereaches)

## Properties

### targetListId

• `Optional` **targetListId**: ``null`` \| *number*

<div lang=\"ja\"> 類似ユーザーをリターゲティングするターゲットIDです。<br> このフィールドは、ADD時に必須となり、SETおよびREMOVE時に無視されます。 </div> 

**`memberof`** RetargetingListServiceSimilarityTargetList

___

### targetListSize

• `Optional` **targetListSize**: ``null`` \| [*Rate1*](./enums/retargetinglistservicetargetlistsize.md#rate1) \| [*Rate2*](./enums/retargetinglistservicetargetlistsize.md#rate2) \| [*Rate3*](./enums/retargetinglistservicetargetlistsize.md#rate3) \| [*Rate4*](./enums/retargetinglistservicetargetlistsize.md#rate4) \| [*Rate5*](./enums/retargetinglistservicetargetlistsize.md#rate5) \| [*Rate6*](./enums/retargetinglistservicetargetlistsize.md#rate6) \| [*Rate7*](./enums/retargetinglistservicetargetlistsize.md#rate7) \| [*Rate8*](./enums/retargetinglistservicetargetlistsize.md#rate8) \| [*Rate9*](./enums/retargetinglistservicetargetlistsize.md#rate9) \| [*Rate10*](./enums/retargetinglistservicetargetlistsize.md#rate10) \| [*Unknown*](./enums/retargetinglistservicetargetlistsize.md#unknown)

**`memberof`** RetargetingListServiceSimilarityTargetList

___

### targetListSizeReaches

• `Optional` **targetListSizeReaches**: ``null`` \| [*RetargetingListServiceTargetListSizeReaches*](retargetinglistservicetargetlistsizereaches.md)[]

**`memberof`** RetargetingListServiceSimilarityTargetList
