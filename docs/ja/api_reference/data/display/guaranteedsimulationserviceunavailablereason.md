# GuaranteedSimulationServiceUnavailableReason


<div lang=\"ja\">GuaranteedSimulationServiceUnavailableReasonオブジェクトは、在庫の不足理由を表します。<br> このオブジェクトで返される各フィールドに対応する在庫は不足しています。<br> このフィールドは、レスポンスの際に返却されますが、リクエストの際には無視されます。</div> 

## Table of contents

### Properties

- [ages](guaranteedsimulationserviceunavailablereason.md#ages)
- [audienceCategories](guaranteedsimulationserviceunavailablereason.md#audiencecategories)
- [date](guaranteedsimulationserviceunavailablereason.md#date)
- [devices](guaranteedsimulationserviceunavailablereason.md#devices)
- [genders](guaranteedsimulationserviceunavailablereason.md#genders)
- [hours](guaranteedsimulationserviceunavailablereason.md#hours)

## Properties

### ages

• `Optional` **ages**: ``null`` \| [*GuaranteedSimulationServiceAge*](./enums/guaranteedsimulationserviceage.md)[]

**`memberof`** GuaranteedSimulationServiceUnavailableReason

___

### audienceCategories

• `Optional` **audienceCategories**: ``null`` \| *string*[]

<div lang=\"ja\"> 在庫がないオーディエンスカテゴリーのターゲットID（カテゴリーコード）のリストです。 </div> 

**`memberof`** GuaranteedSimulationServiceUnavailableReason

___

### date

• `Optional` **date**: ``null`` \| *string*

<div lang=\"ja\"> 在庫がない日を表します。 </div>  Format: yyyyMMdd

**`memberof`** GuaranteedSimulationServiceUnavailableReason

___

### devices

• `Optional` **devices**: ``null`` \| [*GuaranteedSimulationServiceDeviceType*](./enums/guaranteedsimulationservicedevicetype.md)[]

**`memberof`** GuaranteedSimulationServiceUnavailableReason

___

### genders

• `Optional` **genders**: ``null`` \| [*GuaranteedSimulationServiceGender*](./enums/guaranteedsimulationservicegender.md)[]

**`memberof`** GuaranteedSimulationServiceUnavailableReason

___

### hours

• `Optional` **hours**: ``null`` \| *number*[]

<div lang=\"ja\"> 予約ができない時間帯のリストです。 </div> 

**`memberof`** GuaranteedSimulationServiceUnavailableReason
