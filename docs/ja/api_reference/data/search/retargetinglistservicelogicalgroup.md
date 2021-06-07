# RetargetingListServiceLogicalGroup


<div lang=\"ja\">RetargetingListServiceLogicalGroupは、組合せグループの情報を保持するオブジェクトです。<br> このフィールドは、ADDおよびSET時に必須となります。</div> 

## Table of contents

### Properties

- [logicalCondition](retargetinglistservicelogicalgroup.md#logicalcondition)
- [logicalOperand](retargetinglistservicelogicalgroup.md#logicaloperand)

## Properties

### logicalCondition

• `Optional` **logicalCondition**: ``null`` \| [*And*](./enums/retargetinglistservicelogicalcondition.md#and) \| [*Or*](./enums/retargetinglistservicelogicalcondition.md#or) \| [*Not*](./enums/retargetinglistservicelogicalcondition.md#not) \| [*Unknown*](./enums/retargetinglistservicelogicalcondition.md#unknown)

**`memberof`** RetargetingListServiceLogicalGroup

___

### logicalOperand

• `Optional` **logicalOperand**: ``null`` \| [*RetargetingListServiceLogicalRuleOperand*](retargetinglistservicelogicalruleoperand.md)[]

**`memberof`** RetargetingListServiceLogicalGroup
