# GuaranteedInventoryServiceInventoryResult


<div lang=\"ja\">GuaranteedInventoryServiceInventoryResultオブジェクトは、在庫の確認結果を表します。<br> このフィールドは、レスポンスの際に返却されますが、リクエストの際には無視されます。</div> 

## Table of contents

### Properties

- [endDate](guaranteedinventoryserviceinventoryresult.md#enddate)
- [maxReservableSlots](guaranteedinventoryserviceinventoryresult.md#maxreservableslots)
- [maxReservableVImps](guaranteedinventoryserviceinventoryresult.md#maxreservablevimps)
- [maxSellableVImps](guaranteedinventoryserviceinventoryresult.md#maxsellablevimps)
- [sellingSlots](guaranteedinventoryserviceinventoryresult.md#sellingslots)
- [startDate](guaranteedinventoryserviceinventoryresult.md#startdate)
- [unavailableReasons](guaranteedinventoryserviceinventoryresult.md#unavailablereasons)

## Properties

### endDate

• `Optional` **endDate**: ``null`` \| *string*

<div lang=\"ja\"> キャンペーンの終了日です。<br> </div>  Format: yyyyMMdd

**`memberof`** GuaranteedInventoryServiceInventoryResult

___

### maxReservableSlots

• `Optional` **maxReservableSlots**: ``null`` \| *number*

<div lang=\"ja\"> 指定期間で予約可能な最大枠数です。<br> </div> 

**`memberof`** GuaranteedInventoryServiceInventoryResult

___

### maxReservableVImps

• `Optional` **maxReservableVImps**: ``null`` \| *number*

<div lang=\"ja\"> 指定期間のビューアブルインプレッション数の残在庫です。<br> </div> 

**`memberof`** GuaranteedInventoryServiceInventoryResult

___

### maxSellableVImps

• `Optional` **maxSellableVImps**: ``null`` \| *number*

<div lang=\"ja\"> 指定期間で販売可能なビューアブルインプレッション数の在庫です。<br> </div> 

**`memberof`** GuaranteedInventoryServiceInventoryResult

___

### sellingSlots

• `Optional` **sellingSlots**: ``null`` \| *number*

<div lang=\"ja\"> 指定期間で販売可能な枠数の在庫です。<br> </div> 

**`memberof`** GuaranteedInventoryServiceInventoryResult

___

### startDate

• `Optional` **startDate**: ``null`` \| *string*

<div lang=\"ja\"> キャンペーンの開始日です。<br> </div>  Format: yyyyMMdd

**`memberof`** GuaranteedInventoryServiceInventoryResult

___

### unavailableReasons

• `Optional` **unavailableReasons**: ``null`` \| [*GuaranteedInventoryServiceUnavailableReason*](guaranteedinventoryserviceunavailablereason.md)[]

**`memberof`** GuaranteedInventoryServiceInventoryResult
