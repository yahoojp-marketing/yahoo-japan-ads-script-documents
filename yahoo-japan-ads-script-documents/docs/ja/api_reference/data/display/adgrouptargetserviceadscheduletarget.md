# AdGroupTargetServiceAdScheduleTarget


<div lang=\"ja\"> AdGroupTargetServiceAdScheduleTargetオブジェクトは、時間帯ターゲティングの設定情報を保持します。<br> ADD、SETおよびREPLACE時、このフィールドは省略可能となります。<br> ※targetTypeがAD_SCHEDULE_TARGETの場合は必須です。 </div> 

## Table of contents

### Properties

- [dayOfWeek](adgrouptargetserviceadscheduletarget.md#dayofweek)
- [endHour](adgrouptargetserviceadscheduletarget.md#endhour)
- [startHour](adgrouptargetserviceadscheduletarget.md#starthour)

## Properties

### dayOfWeek

• `Optional` **dayOfWeek**: ``null`` \| [*Monday*](./enums/adgrouptargetservicedayofweek.md#monday) \| [*Tuesday*](./enums/adgrouptargetservicedayofweek.md#tuesday) \| [*Wednesday*](./enums/adgrouptargetservicedayofweek.md#wednesday) \| [*Thursday*](./enums/adgrouptargetservicedayofweek.md#thursday) \| [*Friday*](./enums/adgrouptargetservicedayofweek.md#friday) \| [*Saturday*](./enums/adgrouptargetservicedayofweek.md#saturday) \| [*Sunday*](./enums/adgrouptargetservicedayofweek.md#sunday) \| [*Unknown*](./enums/adgrouptargetservicedayofweek.md#unknown)

**`memberof`** AdGroupTargetServiceAdScheduleTarget

___

### endHour

• `Optional` **endHour**: ``null`` \| *number*

<div lang=\"ja\"> 終了時間（時のみ）です。<br> このフィールドは、ADD時は必須となり、REPLACE時は省略可能となります。 </div> 

**`memberof`** AdGroupTargetServiceAdScheduleTarget

___

### startHour

• `Optional` **startHour**: ``null`` \| *number*

<div lang=\"ja\"> 開始時間（時のみ）です。<br> このフィールドは、ADD時は必須となり、REPLACE時は省略可能となります。 </div> 

**`memberof`** AdGroupTargetServiceAdScheduleTarget
