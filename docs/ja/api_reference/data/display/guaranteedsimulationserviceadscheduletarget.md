# GuaranteedSimulationServiceAdScheduleTarget


<div lang=\"ja\"> GuaranteedSimulationServiceAdScheduleTargetオブジェクトは、時間帯ターゲティングの設定情報を保持します。<br> ADD時、このフィールドは省略可能となります。<br> ※targetTypeがAD_SCHEDULE_TARGETの場合は必須です。 </div> 

## Table of contents

### Properties

- [dayOfWeek](guaranteedsimulationserviceadscheduletarget.md#dayofweek)
- [endHour](guaranteedsimulationserviceadscheduletarget.md#endhour)
- [startHour](guaranteedsimulationserviceadscheduletarget.md#starthour)

## Properties

### dayOfWeek

• `Optional` **dayOfWeek**: ``null`` \| [*Monday*](./enums/guaranteedsimulationservicedayofweek.md#monday) \| [*Tuesday*](./enums/guaranteedsimulationservicedayofweek.md#tuesday) \| [*Wednesday*](./enums/guaranteedsimulationservicedayofweek.md#wednesday) \| [*Thursday*](./enums/guaranteedsimulationservicedayofweek.md#thursday) \| [*Friday*](./enums/guaranteedsimulationservicedayofweek.md#friday) \| [*Saturday*](./enums/guaranteedsimulationservicedayofweek.md#saturday) \| [*Sunday*](./enums/guaranteedsimulationservicedayofweek.md#sunday) \| [*Unknown*](./enums/guaranteedsimulationservicedayofweek.md#unknown)

**`memberof`** GuaranteedSimulationServiceAdScheduleTarget

___

### endHour

• `Optional` **endHour**: ``null`` \| *number*

<div lang=\"ja\"> 終了時間（時のみ）です。<br> このフィールドは、ADD時は必須となります。 </div> 

**`memberof`** GuaranteedSimulationServiceAdScheduleTarget

___

### startHour

• `Optional` **startHour**: ``null`` \| *number*

<div lang=\"ja\"> 開始時間（時のみ）です。<br> このフィールドは、ADD時は必須となります。 </div> 

**`memberof`** GuaranteedSimulationServiceAdScheduleTarget
