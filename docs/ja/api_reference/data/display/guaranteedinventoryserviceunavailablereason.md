# GuaranteedInventoryServiceUnavailableReason


<div lang=\"ja\">GuaranteedInventoryServiceUnavailableReasonオブジェクトは、在庫の不足理由を表します。<br> このオブジェクトで返される各フィールドに対応する在庫は不足しています。<br> このフィールドは、レスポンスの際に返却されますが、リクエストの際には無視されます。</div> 

## Table of contents

### Properties

- [ages](guaranteedinventoryserviceunavailablereason.md#ages)
- [audienceCategories](guaranteedinventoryserviceunavailablereason.md#audiencecategories)
- [date](guaranteedinventoryserviceunavailablereason.md#date)
- [devices](guaranteedinventoryserviceunavailablereason.md#devices)
- [genders](guaranteedinventoryserviceunavailablereason.md#genders)

## Properties

### ages

• `Optional` **ages**: ``null`` \| [*GuaranteedInventoryServiceAge*](./enums/guaranteedinventoryserviceage.md)[]

**`memberof`** GuaranteedInventoryServiceUnavailableReason

___

### audienceCategories

• `Optional` **audienceCategories**: ``null`` \| *string*[]

<div lang=\"ja\"> 在庫がないオーディエンスカテゴリーのターゲットID（カテゴリーコード）のリストです。 </div> 

**`memberof`** GuaranteedInventoryServiceUnavailableReason

___

### date

• `Optional` **date**: ``null`` \| *string*

<div lang=\"ja\"> 在庫がない日を表します。 </div>  Format: yyyyMMdd

**`memberof`** GuaranteedInventoryServiceUnavailableReason

___

### devices

• `Optional` **devices**: ``null`` \| [*GuaranteedInventoryServiceDeviceType*](./enums/guaranteedinventoryservicedevicetype.md)[]

**`memberof`** GuaranteedInventoryServiceUnavailableReason

___

### genders

• `Optional` **genders**: ``null`` \| [*GuaranteedInventoryServiceGender*](./enums/guaranteedinventoryservicegender.md)[]

**`memberof`** GuaranteedInventoryServiceUnavailableReason
