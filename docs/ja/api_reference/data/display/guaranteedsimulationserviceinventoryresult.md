# GuaranteedSimulationServiceInventoryResult


<div lang=\"ja\">GuaranteedSimulationServiceInventoryResultオブジェクトは、在庫の確認結果を表します。<br> このフィールドは、レスポンスの際に返却されますが、リクエストの際には無視されます。</div> 

## Table of contents

### Properties

- [endDate](guaranteedsimulationserviceinventoryresult.md#enddate)
- [maxReservableSlots](guaranteedsimulationserviceinventoryresult.md#maxreservableslots)
- [maxReservableVImps](guaranteedsimulationserviceinventoryresult.md#maxreservablevimps)
- [maxSellableVImps](guaranteedsimulationserviceinventoryresult.md#maxsellablevimps)
- [sellingSlots](guaranteedsimulationserviceinventoryresult.md#sellingslots)
- [startDate](guaranteedsimulationserviceinventoryresult.md#startdate)
- [unavailableReasons](guaranteedsimulationserviceinventoryresult.md#unavailablereasons)
- [unreservableReason](guaranteedsimulationserviceinventoryresult.md#unreservablereason)

## Properties

### endDate

• `Optional` **endDate**: ``null`` \| *string*

<div lang=\"ja\"> キャンペーンの終了日です。<br> </div>  Format: yyyyMMdd

**`memberof`** GuaranteedSimulationServiceInventoryResult

___

### maxReservableSlots

• `Optional` **maxReservableSlots**: ``null`` \| *number*

<div lang=\"ja\"> 指定期間で予約可能な最大枠数です。<br> </div> 

**`memberof`** GuaranteedSimulationServiceInventoryResult

___

### maxReservableVImps

• `Optional` **maxReservableVImps**: ``null`` \| *number*

<div lang=\"ja\"> 指定期間のビューアブルインプレッション数の残在庫です。<br> </div> 

**`memberof`** GuaranteedSimulationServiceInventoryResult

___

### maxSellableVImps

• `Optional` **maxSellableVImps**: ``null`` \| *number*

<div lang=\"ja\"> 指定期間で販売可能なビューアブルインプレッション数の在庫です。<br> </div> 

**`memberof`** GuaranteedSimulationServiceInventoryResult

___

### sellingSlots

• `Optional` **sellingSlots**: ``null`` \| *number*

<div lang=\"ja\"> 指定期間で販売可能な枠数の在庫です。<br> </div> 

**`memberof`** GuaranteedSimulationServiceInventoryResult

___

### startDate

• `Optional` **startDate**: ``null`` \| *string*

<div lang=\"ja\"> キャンペーンの開始日です。<br> </div>  Format: yyyyMMdd

**`memberof`** GuaranteedSimulationServiceInventoryResult

___

### unavailableReasons

• `Optional` **unavailableReasons**: ``null`` \| [*GuaranteedSimulationServiceUnavailableReason*](guaranteedsimulationserviceunavailablereason.md)[]

**`memberof`** GuaranteedSimulationServiceInventoryResult

___

### unreservableReason

• `Optional` **unreservableReason**: ``null`` \| [*NotEnoughDeliveryTarget*](./enums/guaranteedsimulationserviceunreservablereason.md#notenoughdeliverytarget) \| [*OutOfStock*](./enums/guaranteedsimulationserviceunreservablereason.md#outofstock) \| [*OverSovDailyLimit*](./enums/guaranteedsimulationserviceunreservablereason.md#oversovdailylimit) \| [*OverSovWeeklyLimit*](./enums/guaranteedsimulationserviceunreservablereason.md#oversovweeklylimit) \| [*Unknown*](./enums/guaranteedsimulationserviceunreservablereason.md#unknown)

**`memberof`** GuaranteedSimulationServiceInventoryResult
