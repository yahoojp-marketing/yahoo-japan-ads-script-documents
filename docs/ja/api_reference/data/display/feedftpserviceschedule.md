# FeedFtpServiceSchedule


<div lang=\"ja\"> FeedFtpServiceScheduleオブジェクトは、定期アップロードのスケジュールを表します。<br> このフィールドは、ADD時は必須となり、SET時は省略可能となります。 </div> 

## Table of contents

### Properties

- [scheduleDaily](feedftpserviceschedule.md#scheduledaily)
- [scheduleHourly](feedftpserviceschedule.md#schedulehourly)
- [scheduleType](feedftpserviceschedule.md#scheduletype)
- [scheduleWeekly](feedftpserviceschedule.md#scheduleweekly)

## Properties

### scheduleDaily

• `Optional` **scheduleDaily**: ``null`` \| [*FeedFtpServiceScheduleDaily*](feedftpservicescheduledaily.md)

**`memberof`** FeedFtpServiceSchedule

___

### scheduleHourly

• `Optional` **scheduleHourly**: ``null`` \| [*FeedFtpServiceScheduleHourly*](feedftpserviceschedulehourly.md)

**`memberof`** FeedFtpServiceSchedule

___

### scheduleType

• `Optional` **scheduleType**: ``null`` \| [*Hourly*](./enums/feedftpservicescheduletype.md#hourly) \| [*Daily*](./enums/feedftpservicescheduletype.md#daily) \| [*Weekly*](./enums/feedftpservicescheduletype.md#weekly) \| [*Unknown*](./enums/feedftpservicescheduletype.md#unknown)

**`memberof`** FeedFtpServiceSchedule

___

### scheduleWeekly

• `Optional` **scheduleWeekly**: ``null`` \| [*FeedFtpServiceScheduleWeekly*](feedftpservicescheduleweekly.md)

**`memberof`** FeedFtpServiceSchedule
