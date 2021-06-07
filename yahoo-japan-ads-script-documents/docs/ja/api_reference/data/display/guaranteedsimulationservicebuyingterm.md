# GuaranteedSimulationServiceBuyingTerm


<div lang=\"ja\"> GuaranteedSimulationServiceBuyingTermは、商品購入期間情報を保持します。<br> このフィールドは、レスポンスの際に返却されますが、リクエストの際には無視されます。 </div> 

## Table of contents

### Properties

- [buyingTermType](guaranteedsimulationservicebuyingterm.md#buyingtermtype)
- [customRangeBuyingTerm](guaranteedsimulationservicebuyingterm.md#customrangebuyingterm)
- [singleDayBuyingTerm](guaranteedsimulationservicebuyingterm.md#singledaybuyingterm)
- [singleTermBuyingTerm](guaranteedsimulationservicebuyingterm.md#singletermbuyingterm)

## Properties

### buyingTermType

• `Optional` **buyingTermType**: ``null`` \| [*SingleDay*](./enums/guaranteedsimulationservicebuyingtermtype.md#singleday) \| [*SingleTerm*](./enums/guaranteedsimulationservicebuyingtermtype.md#singleterm) \| [*CustomRange*](./enums/guaranteedsimulationservicebuyingtermtype.md#customrange) \| [*Unknown*](./enums/guaranteedsimulationservicebuyingtermtype.md#unknown)

**`memberof`** GuaranteedSimulationServiceBuyingTerm

___

### customRangeBuyingTerm

• `Optional` **customRangeBuyingTerm**: ``null`` \| [*GuaranteedSimulationServiceCustomRangeBuyingTerm*](guaranteedsimulationservicecustomrangebuyingterm.md)

**`memberof`** GuaranteedSimulationServiceBuyingTerm

___

### singleDayBuyingTerm

• `Optional` **singleDayBuyingTerm**: ``null`` \| [*GuaranteedSimulationServiceSingleDayBuyingTerm*](guaranteedsimulationservicesingledaybuyingterm.md)

**`memberof`** GuaranteedSimulationServiceBuyingTerm

___

### singleTermBuyingTerm

• `Optional` **singleTermBuyingTerm**: ``null`` \| [*GuaranteedSimulationServiceSingleTermBuyingTerm*](guaranteedsimulationservicesingletermbuyingterm.md)

**`memberof`** GuaranteedSimulationServiceBuyingTerm
