# RetargetingListServiceRuleItem


<div lang=\"ja\">RetargetingListServiceRuleItemは、ルールの評価条件を保持するオブジェクトです。<br> このフィールドは、ADDおよびSET時に必須となります。</div> 

## Table of contents

### Properties

- [customKeyRuleItem](retargetinglistserviceruleitem.md#customkeyruleitem)
- [ruleOperator](retargetinglistserviceruleitem.md#ruleoperator)
- [ruleType](retargetinglistserviceruleitem.md#ruletype)
- [urlRuleItem](retargetinglistserviceruleitem.md#urlruleitem)
- [value](retargetinglistserviceruleitem.md#value)

## Properties

### customKeyRuleItem

• `Optional` **customKeyRuleItem**: ``null`` \| [*RetargetingListServiceCustomKeyRuleItem*](retargetinglistservicecustomkeyruleitem.md)

**`memberof`** RetargetingListServiceRuleItem

___

### ruleOperator

• `Optional` **ruleOperator**: ``null`` \| [*Unknown*](./enums/retargetinglistserviceruleoperator.md#unknown) \| [*Equals*](./enums/retargetinglistserviceruleoperator.md#equals) \| [*NotEqual*](./enums/retargetinglistserviceruleoperator.md#notequal) \| [*Contains*](./enums/retargetinglistserviceruleoperator.md#contains) \| [*NotContain*](./enums/retargetinglistserviceruleoperator.md#notcontain) \| [*StartsWith*](./enums/retargetinglistserviceruleoperator.md#startswith) \| [*NotStartWith*](./enums/retargetinglistserviceruleoperator.md#notstartwith) \| [*EndsWith*](./enums/retargetinglistserviceruleoperator.md#endswith) \| [*NotEndWith*](./enums/retargetinglistserviceruleoperator.md#notendwith)

**`memberof`** RetargetingListServiceRuleItem

___

### ruleType

• `Optional` **ruleType**: ``null`` \| [*UrlRule*](./enums/retargetinglistserviceruletype.md#urlrule) \| [*CustomKeyRule*](./enums/retargetinglistserviceruletype.md#customkeyrule) \| [*Unknown*](./enums/retargetinglistserviceruletype.md#unknown)

**`memberof`** RetargetingListServiceRuleItem

___

### urlRuleItem

• `Optional` **urlRuleItem**: ``null`` \| [*RetargetingListServiceUrlRuleItem*](retargetinglistserviceurlruleitem.md)

**`memberof`** RetargetingListServiceRuleItem

___

### value

• `Optional` **value**: ``null`` \| *string*

<div lang=\"ja\">評価値です。<br> ADDおよびSET時、このフィールドは必須となります。<br> ※括弧（()）、シングルクォート（&#39;）、ダブルクォート（&#34;）、タブ（\\t）は利用できません。<br> ※250文字まで指定可能です。</div> 

**`memberof`** RetargetingListServiceRuleItem
