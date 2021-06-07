# FeedSetServiceConditionSet


<div lang=\"ja\"> FeedSetServiceConditionSetオブジェクトは、商品セット情報の条件を保持します。<br> ADD時、このフィールドは必須です。 </div> 

## Table of contents

### Properties

- [conditionType](feedsetserviceconditionset.md#conditiontype)
- [orConditions](feedsetserviceconditionset.md#orconditions)

## Properties

### conditionType

• `Optional` **conditionType**: ``null`` \| [*CategoryId*](./enums/feedsetserviceconditiontype.md#categoryid) \| [*StockQuantity*](./enums/feedsetserviceconditiontype.md#stockquantity) \| [*Price*](./enums/feedsetserviceconditiontype.md#price) \| [*SalePrice*](./enums/feedsetserviceconditiontype.md#saleprice) \| [*Rating*](./enums/feedsetserviceconditiontype.md#rating) \| [*Reviews*](./enums/feedsetserviceconditiontype.md#reviews) \| [*Badge*](./enums/feedsetserviceconditiontype.md#badge) \| [*AgeGroup*](./enums/feedsetserviceconditiontype.md#agegroup) \| [*AvailabilityDate*](./enums/feedsetserviceconditiontype.md#availabilitydate) \| [*GenderGroup*](./enums/feedsetserviceconditiontype.md#gendergroup) \| [*GoogleProductCategory*](./enums/feedsetserviceconditiontype.md#googleproductcategory) \| [*Location*](./enums/feedsetserviceconditiontype.md#location) \| [*SalesRank*](./enums/feedsetserviceconditiontype.md#salesrank) \| [*Unknown*](./enums/feedsetserviceconditiontype.md#unknown)

**`memberof`** FeedSetServiceConditionSet

___

### orConditions

• `Optional` **orConditions**: ``null`` \| [*FeedSetServiceCondition*](feedsetservicecondition.md)[]

**`memberof`** FeedSetServiceConditionSet
