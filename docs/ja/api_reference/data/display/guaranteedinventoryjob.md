# GuaranteedInventoryJob


<div lang=\"ja\">GuaranteedInventoryJobオブジェクトは、在庫情報のジョブを格納するコンテナです。</div> 

## Table of contents

### Properties

- [accountId](guaranteedinventoryjob.md#accountid)
- [createdBusinessId](guaranteedinventoryjob.md#createdbusinessid)
- [inventories](guaranteedinventoryjob.md#inventories)
- [inventoryJobEndDate](guaranteedinventoryjob.md#inventoryjobenddate)
- [inventoryJobId](guaranteedinventoryjob.md#inventoryjobid)
- [inventoryJobName](guaranteedinventoryjob.md#inventoryjobname)
- [inventoryJobStartDate](guaranteedinventoryjob.md#inventoryjobstartdate)
- [inventoryJobStatus](guaranteedinventoryjob.md#inventoryjobstatus)
- [isExpiredPackage](guaranteedinventoryjob.md#isexpiredpackage)
- [notificationBusinessIds](guaranteedinventoryjob.md#notificationbusinessids)

## Properties

### accountId

• `Optional` **accountId**: ``null`` \| *number*

<div lang=\"ja\"> アカウントIDです。<br> このフィールドは、レスポンスの際に返却されますが、リクエストの際には無視されます。 </div> 

**`memberof`** GuaranteedInventoryJob

___

### createdBusinessId

• `Optional` **createdBusinessId**: ``null`` \| *string*

<div lang=\"ja\">在庫確認ジョブ作成者のYahoo! JAPANビジネスIDです。<br> このフィールドは、レスポンスの際に返却されますが、リクエストの際には無視されます。</div> 

**`memberof`** GuaranteedInventoryJob

___

### inventories

• `Optional` **inventories**: ``null`` \| [*GuaranteedInventoryServiceInventory*](guaranteedinventoryserviceinventory.md)[]

**`memberof`** GuaranteedInventoryJob

___

### inventoryJobEndDate

• `Optional` **inventoryJobEndDate**: ``null`` \| *string*

<div lang=\"ja\"> 在庫確認ジョブの完了日時です。<br> 在庫確認ジョブが実行中の場合はnullで返ります。<br> このフィールドは、レスポンスの際に返却されますが、リクエストの際には無視されます。</div>  Format: yyyyMMddHHmmss

**`memberof`** GuaranteedInventoryJob

___

### inventoryJobId

• `Optional` **inventoryJobId**: ``null`` \| *number*

<div lang=\"ja\">在庫確認ジョブIDです。<br> このフィールドは、レスポンスの際に返却されますが、リクエストの際には無視されます。</div> 

**`memberof`** GuaranteedInventoryJob

___

### inventoryJobName

• `Optional` **inventoryJobName**: ``null`` \| *string*

<div lang=\"ja\">在庫確認ジョブ名です。<br> ADD時、このフィールドは必須となります。</div> 

**`memberof`** GuaranteedInventoryJob

___

### inventoryJobStartDate

• `Optional` **inventoryJobStartDate**: ``null`` \| *string*

<div lang=\"ja\"> 在庫確認ジョブの開始日時です。<br> このフィールドは、レスポンスの際に返却されますが、リクエストの際には無視されます。 </div>  Format: yyyyMMddHHmmss

**`memberof`** GuaranteedInventoryJob

___

### inventoryJobStatus

• `Optional` **inventoryJobStatus**: ``null`` \| [*Processing*](./enums/guaranteedinventoryserviceinventoryjobstatus.md#processing) \| [*Succeeded*](./enums/guaranteedinventoryserviceinventoryjobstatus.md#succeeded) \| [*Failed*](./enums/guaranteedinventoryserviceinventoryjobstatus.md#failed) \| [*Unknown*](./enums/guaranteedinventoryserviceinventoryjobstatus.md#unknown)

**`memberof`** GuaranteedInventoryJob

___

### isExpiredPackage

• `Optional` **isExpiredPackage**: ``null`` \| *boolean*

<div lang=\"ja\"> 予約有効終了日が過去日の商品が指定されているかどうかのフラグです。<br> trueの場合、その商品の予約有効終了日を超えていることを示しています。<br> このフィールドは、レスポンスの際に返却されますが、リクエストの際には無視されます。</div> 

**`memberof`** GuaranteedInventoryJob

___

### notificationBusinessIds

• `Optional` **notificationBusinessIds**: ``null`` \| *string*[]

<div lang=\"ja\">連絡先Yahoo! JAPANビジネスIDです。<br> ADD時、このフィールドは省略可能となります。</div> 

**`memberof`** GuaranteedInventoryJob
