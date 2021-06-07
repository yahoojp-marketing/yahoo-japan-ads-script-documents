# StatsServiceValue


<div lang=\"ja\">StatsServiceValueオブジェクトは、統計情報1件あたりの実行結果（1 Entity）を保持します。</div> 

## Table of contents

### Properties

- [accountId](statsservicevalue.md#accountid)
- [adGroupStatsValue](statsservicevalue.md#adgroupstatsvalue)
- [adStatsValue](statsservicevalue.md#adstatsvalue)
- [campaignStatsValue](statsservicevalue.md#campaignstatsvalue)
- [errors](statsservicevalue.md#errors)
- [imageStatsValue](statsservicevalue.md#imagestatsvalue)
- [operationSucceeded](statsservicevalue.md#operationsucceeded)
- [periodCustomDate](statsservicevalue.md#periodcustomdate)
- [statsPeriod](statsservicevalue.md#statsperiod)
- [targetStatsValue](statsservicevalue.md#targetstatsvalue)
- [type](statsservicevalue.md#type)
- [videoStatsValue](statsservicevalue.md#videostatsvalue)

## Properties

### accountId

• `Optional` **accountId**: ``null`` \| *number*

<div lang=\"ja\">アカウントIDです。</div> 

**`memberof`** StatsServiceValue

___

### adGroupStatsValue

• `Optional` **adGroupStatsValue**: ``null`` \| [*StatsServiceAdGroupStatsValue*](statsserviceadgroupstatsvalue.md)

**`memberof`** StatsServiceValue

___

### adStatsValue

• `Optional` **adStatsValue**: ``null`` \| [*StatsServiceAdStatsValue*](statsserviceadstatsvalue.md)

**`memberof`** StatsServiceValue

___

### campaignStatsValue

• `Optional` **campaignStatsValue**: ``null`` \| [*StatsServiceCampaignStatsValue*](statsservicecampaignstatsvalue.md)

**`memberof`** StatsServiceValue

___

### errors

• `Optional` **errors**: ``null`` \| [*ModelError*](modelerror.md)[]

**`memberof`** StatsServiceValue

___

### imageStatsValue

• `Optional` **imageStatsValue**: ``null`` \| [*StatsServiceImageStatsValue*](statsserviceimagestatsvalue.md)

**`memberof`** StatsServiceValue

___

### operationSucceeded

• `Optional` **operationSucceeded**: ``null`` \| *boolean*

<div lang=\"ja\">処理結果です。trueの場合は、処理は成功しました。falseの場合は処理が失敗しています。</div> 

**`memberof`** StatsServiceValue

___

### periodCustomDate

• `Optional` **periodCustomDate**: ``null`` \| [*StatsServicePeriodCustomDate*](statsserviceperiodcustomdate.md)

**`memberof`** StatsServiceValue

___

### statsPeriod

• `Optional` **statsPeriod**: ``null`` \| [*RealtimeToday*](./enums/statsservicestatsperiod.md#realtimetoday) \| [*DefiniteValueYesterday*](./enums/statsservicestatsperiod.md#definitevalueyesterday) \| [*DefiniteValueLastweek*](./enums/statsservicestatsperiod.md#definitevaluelastweek) \| [*DefiniteValueLastbsday*](./enums/statsservicestatsperiod.md#definitevaluelastbsday) \| [*DefiniteValueWeek*](./enums/statsservicestatsperiod.md#definitevalueweek) \| [*DefiniteValueTwoweek*](./enums/statsservicestatsperiod.md#definitevaluetwoweek) \| [*DefiniteValueThirtyday*](./enums/statsservicestatsperiod.md#definitevaluethirtyday) \| [*RealtimeMonth*](./enums/statsservicestatsperiod.md#realtimemonth) \| [*DefiniteValueLastmonth*](./enums/statsservicestatsperiod.md#definitevaluelastmonth) \| [*DefiniteValueLast13Month*](./enums/statsservicestatsperiod.md#definitevaluelast13month) \| [*CustomDate*](./enums/statsservicestatsperiod.md#customdate) \| [*Unknown*](./enums/statsservicestatsperiod.md#unknown)

**`memberof`** StatsServiceValue

___

### targetStatsValue

• `Optional` **targetStatsValue**: ``null`` \| [*StatsServiceTargetStatsValue*](statsservicetargetstatsvalue.md)

**`memberof`** StatsServiceValue

___

### type

• `Optional` **type**: ``null`` \| [*Campaign*](./enums/statsservicetype.md#campaign) \| [*Adgroup*](./enums/statsservicetype.md#adgroup) \| [*Ad*](./enums/statsservicetype.md#ad) \| [*Image*](./enums/statsservicetype.md#image) \| [*Video*](./enums/statsservicetype.md#video) \| [*Target*](./enums/statsservicetype.md#target) \| [*Unknown*](./enums/statsservicetype.md#unknown)

**`memberof`** StatsServiceValue

___

### videoStatsValue

• `Optional` **videoStatsValue**: ``null`` \| [*StatsServiceVideoStatsValue*](statsservicevideostatsvalue.md)

**`memberof`** StatsServiceValue
