# CampaignTargetServiceScheduleTarget


<div lang=\"ja\">CampaignTargetServiceScheduleTargetオブジェクトは、曜日・時間帯ターゲティングレポートを表します。<br> このフィールドは、ADD時およびSET時に省略可能となります。<br> ※targetTypeがSCHEDULEの場合、このフィールドはADD時に必須となります。</div> 

## Table of contents

### Properties

- [dayOfWeek](campaigntargetservicescheduletarget.md#dayofweek)
- [endHour](campaigntargetservicescheduletarget.md#endhour)
- [endMinute](campaigntargetservicescheduletarget.md#endminute)
- [startHour](campaigntargetservicescheduletarget.md#starthour)
- [startMinute](campaigntargetservicescheduletarget.md#startminute)

## Properties

### dayOfWeek

• `Optional` **dayOfWeek**: ``null`` \| [*Monday*](./enums/campaigntargetservicedayofweek.md#monday) \| [*Tuesday*](./enums/campaigntargetservicedayofweek.md#tuesday) \| [*Wednesday*](./enums/campaigntargetservicedayofweek.md#wednesday) \| [*Thursday*](./enums/campaigntargetservicedayofweek.md#thursday) \| [*Friday*](./enums/campaigntargetservicedayofweek.md#friday) \| [*Saturday*](./enums/campaigntargetservicedayofweek.md#saturday) \| [*Sunday*](./enums/campaigntargetservicedayofweek.md#sunday) \| [*Unknown*](./enums/campaigntargetservicedayofweek.md#unknown)

**`memberof`** CampaignTargetServiceScheduleTarget

___

### endHour

• `Optional` **endHour**: ``null`` \| *number*

<div lang=\"ja\">24時間表示の終了時刻です。<br>このフィールドは、ADD時に必須となります。</div> 

**`memberof`** CampaignTargetServiceScheduleTarget

___

### endMinute

• `Optional` **endMinute**: ``null`` \| [*Zero*](./enums/campaigntargetserviceminuteofhour.md#zero) \| [*Fifteen*](./enums/campaigntargetserviceminuteofhour.md#fifteen) \| [*Thirty*](./enums/campaigntargetserviceminuteofhour.md#thirty) \| [*FortyFive*](./enums/campaigntargetserviceminuteofhour.md#fortyfive) \| [*Unknown*](./enums/campaigntargetserviceminuteofhour.md#unknown)

**`memberof`** CampaignTargetServiceScheduleTarget

___

### startHour

• `Optional` **startHour**: ``null`` \| *number*

<div lang=\"ja\">24時間表示の開始時刻です。<br>このフィールドは、ADD時に必須となります。</div> 

**`memberof`** CampaignTargetServiceScheduleTarget

___

### startMinute

• `Optional` **startMinute**: ``null`` \| [*Zero*](./enums/campaigntargetserviceminuteofhour.md#zero) \| [*Fifteen*](./enums/campaigntargetserviceminuteofhour.md#fifteen) \| [*Thirty*](./enums/campaigntargetserviceminuteofhour.md#thirty) \| [*FortyFive*](./enums/campaigntargetserviceminuteofhour.md#fortyfive) \| [*Unknown*](./enums/campaigntargetserviceminuteofhour.md#unknown)

**`memberof`** CampaignTargetServiceScheduleTarget
