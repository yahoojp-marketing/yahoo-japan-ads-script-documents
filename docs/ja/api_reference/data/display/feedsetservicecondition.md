# FeedSetServiceCondition


<div lang=\"ja\"> FeedSetServiceConditionオブジェクトは、商品セット情報のOR条件を保持します。<br> ADD時、このフィールドは必須です。 </div> 

## Table of contents

### Properties

- [compareOperator](feedsetservicecondition.md#compareoperator)
- [value](feedsetservicecondition.md#value)

## Properties

### compareOperator

• `Optional` **compareOperator**: ``null`` \| [*Equal*](./enums/feedsetservicecompareoperator.md#equal) \| [*NotEqual*](./enums/feedsetservicecompareoperator.md#notequal) \| [*GreaterThanEquals*](./enums/feedsetservicecompareoperator.md#greaterthanequals) \| [*LessThanEquals*](./enums/feedsetservicecompareoperator.md#lessthanequals) \| [*Unknown*](./enums/feedsetservicecompareoperator.md#unknown)

**`memberof`** FeedSetServiceCondition

___

### value

• `Optional` **value**: ``null`` \| *string*

<div lang=\"ja\"> 値です。<br> ADD時、このフィールドは必須です。<br> 設定可能な値はFeedSetServiceConditionTypeをご参照ください。<br> </div> 

**`memberof`** FeedSetServiceCondition
