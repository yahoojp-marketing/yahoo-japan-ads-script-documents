# FeedItemServiceSchedule


<div lang=\"ja\">FeedItemServiceScheduleオブジェクトは、広告表示オプションの配信スケジュール設定を表します。<br> このフィールドは、ADDおよびSET時に省略可能となります。</div> 

## Table of contents

### Properties

- [dayOfWeek](feeditemserviceschedule.md#dayofweek)
- [endHour](feeditemserviceschedule.md#endhour)
- [endMinute](feeditemserviceschedule.md#endminute)
- [startHour](feeditemserviceschedule.md#starthour)
- [startMinute](feeditemserviceschedule.md#startminute)

## Properties

### dayOfWeek

• `Optional` **dayOfWeek**: ``null`` \| [*Monday*](./enums/feeditemservicedayofweek.md#monday) \| [*Tuesday*](./enums/feeditemservicedayofweek.md#tuesday) \| [*Wednesday*](./enums/feeditemservicedayofweek.md#wednesday) \| [*Thursday*](./enums/feeditemservicedayofweek.md#thursday) \| [*Friday*](./enums/feeditemservicedayofweek.md#friday) \| [*Saturday*](./enums/feeditemservicedayofweek.md#saturday) \| [*Sunday*](./enums/feeditemservicedayofweek.md#sunday) \| [*Unknown*](./enums/feeditemservicedayofweek.md#unknown)

**`memberof`** FeedItemServiceSchedule

___

### endHour

• `Optional` **endHour**: ``null`` \| *number*

<div lang=\"ja\">終了時です。<br> ※0 ～ 24の範囲で設定してください。<br> このフィールドは、ADDおよびSET時に必須となります。</div> 

**`memberof`** FeedItemServiceSchedule

___

### endMinute

• `Optional` **endMinute**: ``null`` \| [*Zero*](./enums/feeditemserviceminuteofhour.md#zero) \| [*Fifteen*](./enums/feeditemserviceminuteofhour.md#fifteen) \| [*Thirty*](./enums/feeditemserviceminuteofhour.md#thirty) \| [*FortyFive*](./enums/feeditemserviceminuteofhour.md#fortyfive) \| [*Unknown*](./enums/feeditemserviceminuteofhour.md#unknown)

**`memberof`** FeedItemServiceSchedule

___

### startHour

• `Optional` **startHour**: ``null`` \| *number*

<div lang=\"ja\">開始時です。<br> ※0 ～ 23の範囲で設定してください。<br> このフィールドは、ADDおよびSET時に必須となります。</div> 

**`memberof`** FeedItemServiceSchedule

___

### startMinute

• `Optional` **startMinute**: ``null`` \| [*Zero*](./enums/feeditemserviceminuteofhour.md#zero) \| [*Fifteen*](./enums/feeditemserviceminuteofhour.md#fifteen) \| [*Thirty*](./enums/feeditemserviceminuteofhour.md#thirty) \| [*FortyFive*](./enums/feeditemserviceminuteofhour.md#fortyfive) \| [*Unknown*](./enums/feeditemserviceminuteofhour.md#unknown)

**`memberof`** FeedItemServiceSchedule
