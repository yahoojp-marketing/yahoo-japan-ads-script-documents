# StatsServiceSelector


<div lang=\"ja\">StatsServiceSelectorオブジェクトは、getメソッドの検索条件（実行パラメータ）を保持します。</div> 

## Table of contents

### Properties

- [accountId](statsserviceselector.md#accountid)
- [adGroupIds](statsserviceselector.md#adgroupids)
- [adIds](statsserviceselector.md#adids)
- [campaignIds](statsserviceselector.md#campaignids)
- [mediaIds](statsserviceselector.md#mediaids)
- [numberResults](statsserviceselector.md#numberresults)
- [periodCustomDate](statsserviceselector.md#periodcustomdate)
- [startIndex](statsserviceselector.md#startindex)
- [statsPeriod](statsserviceselector.md#statsperiod)
- [targetTypes](statsserviceselector.md#targettypes)
- [type](statsserviceselector.md#type)

## Properties

### accountId

• **accountId**: *number*

<div lang=\"ja\">アカウントID</div> 

**`memberof`** StatsServiceSelector

___

### adGroupIds

• `Optional` **adGroupIds**: ``null`` \| *number*[]

<div lang=\"ja\"> 広告グループID<br> typeで「ADGROUP」または「AD」または「TARGET」を指定した場合のみ有効です。 </div> 

**`memberof`** StatsServiceSelector

___

### adIds

• `Optional` **adIds**: ``null`` \| *number*[]

<div lang=\"ja\"> 広告ID<br> typeで「AD」を指定した場合のみ有効です。 </div> 

**`memberof`** StatsServiceSelector

___

### campaignIds

• `Optional` **campaignIds**: ``null`` \| *number*[]

<div lang=\"ja\"> キャンペーンID<br> typeで「CAMPAIGN」または「ADGROUP」または「AD」または「TARGET」を指定した場合のみ有効です。 </div> 

**`memberof`** StatsServiceSelector

___

### mediaIds

• `Optional` **mediaIds**: ``null`` \| *number*[]

<div lang=\"ja\"> 画像ID<br> typeで「MEDIA」を指定した場合のみ有効です。 </div> 

**`memberof`** StatsServiceSelector

___

### numberResults

• `Optional` **numberResults**: ``null`` \| *number*

<div lang=\"ja\">ページの最大件数です。このフィールドは、1以上を指定する必要があります。</div> 

**`memberof`** StatsServiceSelector

___

### periodCustomDate

• `Optional` **periodCustomDate**: ``null`` \| [*StatsServicePeriodCustomDate*](statsserviceperiodcustomdate.md)

**`memberof`** StatsServiceSelector

___

### startIndex

• `Optional` **startIndex**: ``null`` \| *number*

<div lang=\"ja\">ページの先頭のインデックスです。このフィールドは、1以上を指定する必要があります。</div> 

**`memberof`** StatsServiceSelector

___

### statsPeriod

• `Optional` **statsPeriod**: ``null`` \| [*RealtimeToday*](./enums/statsservicestatsperiod.md#realtimetoday) \| [*DefiniteValueYesterday*](./enums/statsservicestatsperiod.md#definitevalueyesterday) \| [*DefiniteValueLastweek*](./enums/statsservicestatsperiod.md#definitevaluelastweek) \| [*DefiniteValueLastbsday*](./enums/statsservicestatsperiod.md#definitevaluelastbsday) \| [*DefiniteValueWeek*](./enums/statsservicestatsperiod.md#definitevalueweek) \| [*DefiniteValueTwoweek*](./enums/statsservicestatsperiod.md#definitevaluetwoweek) \| [*DefiniteValueThirtyday*](./enums/statsservicestatsperiod.md#definitevaluethirtyday) \| [*RealtimeMonth*](./enums/statsservicestatsperiod.md#realtimemonth) \| [*DefiniteValueLastmonth*](./enums/statsservicestatsperiod.md#definitevaluelastmonth) \| [*DefiniteValueLast13Month*](./enums/statsservicestatsperiod.md#definitevaluelast13month) \| [*CustomDate*](./enums/statsservicestatsperiod.md#customdate) \| [*Unknown*](./enums/statsservicestatsperiod.md#unknown)

**`memberof`** StatsServiceSelector

___

### targetTypes

• `Optional` **targetTypes**: ``null`` \| [*StatsServiceTargetType*](./enums/statsservicetargettype.md)[]

**`memberof`** StatsServiceSelector

___

### type

• `Optional` **type**: ``null`` \| [*Campaign*](./enums/statsservicetype.md#campaign) \| [*Adgroup*](./enums/statsservicetype.md#adgroup) \| [*Ad*](./enums/statsservicetype.md#ad) \| [*Image*](./enums/statsservicetype.md#image) \| [*Video*](./enums/statsservicetype.md#video) \| [*Target*](./enums/statsservicetype.md#target) \| [*Unknown*](./enums/statsservicetype.md#unknown)

**`memberof`** StatsServiceSelector
