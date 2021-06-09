# GuaranteedInventoryServiceAdScheduleTarget


<div lang=\"ja\"> GuaranteedInventoryServiceAdScheduleTargetオブジェクトは、時間帯ターゲティングの設定情報を保持します。<br> ADD時、このフィールドは省略可能となります。<br> ※targetTypeがAD_SCHEDULE_TARGETの場合は必須です。 </div> 

## Table of contents

### Properties

- [dayOfWeek](guaranteedinventoryserviceadscheduletarget.md#dayofweek)
- [endHour](guaranteedinventoryserviceadscheduletarget.md#endhour)
- [startHour](guaranteedinventoryserviceadscheduletarget.md#starthour)

## Properties

### dayOfWeek

• `Optional` **dayOfWeek**: ``null`` \| [*Monday*](./enums/guaranteedinventoryservicedayofweek.md#monday) \| [*Tuesday*](./enums/guaranteedinventoryservicedayofweek.md#tuesday) \| [*Wednesday*](./enums/guaranteedinventoryservicedayofweek.md#wednesday) \| [*Thursday*](./enums/guaranteedinventoryservicedayofweek.md#thursday) \| [*Friday*](./enums/guaranteedinventoryservicedayofweek.md#friday) \| [*Saturday*](./enums/guaranteedinventoryservicedayofweek.md#saturday) \| [*Sunday*](./enums/guaranteedinventoryservicedayofweek.md#sunday) \| [*Unknown*](./enums/guaranteedinventoryservicedayofweek.md#unknown)

**`memberof`** GuaranteedInventoryServiceAdScheduleTarget

___

### endHour

• `Optional` **endHour**: ``null`` \| *number*

<div lang=\"ja\"> 終了時間（時のみ）です。<br> このフィールドは、ADD時は必須となります。 </div> 

**`memberof`** GuaranteedInventoryServiceAdScheduleTarget

___

### startHour

• `Optional` **startHour**: ``null`` \| *number*

<div lang=\"ja\"> 開始時間（時のみ）です。<br> このフィールドは、ADD時は必須となります。 </div> 

**`memberof`** GuaranteedInventoryServiceAdScheduleTarget
