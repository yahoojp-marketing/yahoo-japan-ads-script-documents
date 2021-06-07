# RetargetingListServiceCombination


<div lang=\"ja\"> RetargetingListServiceCombinationオブジェクトは、ターゲットリストの組み合わせに関する情報を格納するコンテナです。<br> このフィールドは、ADDおよびSET時に必須となります。 </div> 

## Table of contents

### Properties

- [logicalOperator](retargetinglistservicecombination.md#logicaloperator)
- [targetLists](retargetinglistservicecombination.md#targetlists)

## Properties

### logicalOperator

• `Optional` **logicalOperator**: ``null`` \| [*Or*](./enums/retargetinglistservicelogicaloperator.md#or) \| [*And*](./enums/retargetinglistservicelogicaloperator.md#and) \| [*Notin*](./enums/retargetinglistservicelogicaloperator.md#notin) \| [*Unknown*](./enums/retargetinglistservicelogicaloperator.md#unknown)

**`memberof`** RetargetingListServiceCombination

___

### targetLists

• `Optional` **targetLists**: ``null`` \| [*RetargetingListServiceTargetListData*](retargetinglistservicetargetlistdata.md)[]

**`memberof`** RetargetingListServiceCombination
