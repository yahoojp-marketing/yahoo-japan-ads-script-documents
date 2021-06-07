# RetargetingListServiceRuleTargetList


<div lang=\"ja\"> RetargetingListServiceRuleTargetListオブジェクトは、ルール設定のリストを表します。<br> このフィールドは、ADDおよびSET時に省略可能となります。<br> ※targetListTypeがDEFAULT_LISTまたはRULEの場合は、ADDおよびSET時に必須となります。 </div> 

## Table of contents

### Properties

- [isOpen](retargetinglistserviceruletargetlist.md#isopen)
- [isPreset](retargetinglistserviceruletargetlist.md#ispreset)
- [reachPeriod](retargetinglistserviceruletargetlist.md#reachperiod)
- [retargetingTagId](retargetinglistserviceruletargetlist.md#retargetingtagid)
- [rules](retargetinglistserviceruletargetlist.md#rules)

## Properties

### isOpen

• `Optional` **isOpen**: ``null`` \| [*True*](./enums/retargetinglistserviceisopen.md#true) \| [*False*](./enums/retargetinglistserviceisopen.md#false) \| [*Unknown*](./enums/retargetinglistserviceisopen.md#unknown)

**`memberof`** RetargetingListServiceRuleTargetList

___

### isPreset

• `Optional` **isPreset**: ``null`` \| [*True*](./enums/retargetinglistserviceispreset.md#true) \| [*False*](./enums/retargetinglistserviceispreset.md#false) \| [*Unknown*](./enums/retargetinglistserviceispreset.md#unknown)

**`memberof`** RetargetingListServiceRuleTargetList

___

### reachPeriod

• `Optional` **reachPeriod**: ``null`` \| *number*

<div lang=\"ja\"> リーチの蓄積期間（1日～540日）です。<br> このフィールドは、ADD時に必須となり、SET時に省略可能となります。 </div> 

**`memberof`** RetargetingListServiceRuleTargetList

___

### retargetingTagId

• `Optional` **retargetingTagId**: ``null`` \| *string*

<div lang=\"ja\"> リターゲティングタグIDです。<br> このフィールドは、ADD時に必須となります。 </div> 

**`memberof`** RetargetingListServiceRuleTargetList

___

### rules

• `Optional` **rules**: ``null`` \| [*RetargetingListServiceRule*](retargetinglistservicerule.md)[]

**`memberof`** RetargetingListServiceRuleTargetList
