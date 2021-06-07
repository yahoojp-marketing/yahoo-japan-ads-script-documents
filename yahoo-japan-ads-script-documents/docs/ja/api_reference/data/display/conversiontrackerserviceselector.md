# ConversionTrackerServiceSelector


<div lang=\"ja\">ConversionTrackerServiceSelectorオブジェクトは、getメソッドの検索条件（実行パラメータ）を保持します。</div> 

## Table of contents

### Properties

- [accountId](conversiontrackerserviceselector.md#accountid)
- [appConversionPlatform](conversiontrackerserviceselector.md#appconversionplatform)
- [appIds](conversiontrackerserviceselector.md#appids)
- [categories](conversiontrackerserviceselector.md#categories)
- [conversionTrackerIds](conversiontrackerserviceselector.md#conversiontrackerids)
- [conversionTrackerTypes](conversiontrackerserviceselector.md#conversiontrackertypes)
- [countingType](conversiontrackerserviceselector.md#countingtype)
- [excludeFromBidding](conversiontrackerserviceselector.md#excludefrombidding)
- [numberResults](conversiontrackerserviceselector.md#numberresults)
- [startIndex](conversiontrackerserviceselector.md#startindex)
- [statsPeriod](conversiontrackerserviceselector.md#statsperiod)
- [statsPeriodCustomDate](conversiontrackerserviceselector.md#statsperiodcustomdate)
- [statuses](conversiontrackerserviceselector.md#statuses)

## Properties

### accountId

• **accountId**: *number*

<div lang=\"ja\">アカウントID。</div> 

**`memberof`** ConversionTrackerServiceSelector

___

### appConversionPlatform

• `Optional` **appConversionPlatform**: ``null`` \| [*Itunes*](./enums/conversiontrackerserviceappconversionplatform.md#itunes) \| [*AndroidMarket*](./enums/conversiontrackerserviceappconversionplatform.md#androidmarket) \| [*Unknown*](./enums/conversiontrackerserviceappconversionplatform.md#unknown)

**`memberof`** ConversionTrackerServiceSelector

___

### appIds

• `Optional` **appIds**: ``null`` \| *string*[]

<div lang=\"ja\">アプリID。</div> 

**`memberof`** ConversionTrackerServiceSelector

___

### categories

• `Optional` **categories**: ``null`` \| [*ConversionTrackerServiceCategory*](./enums/conversiontrackerservicecategory.md)[]

**`memberof`** ConversionTrackerServiceSelector

___

### conversionTrackerIds

• `Optional` **conversionTrackerIds**: ``null`` \| *number*[]

<div lang=\"ja\">コンバージョントラッカーのID。</div> 

**`memberof`** ConversionTrackerServiceSelector

___

### conversionTrackerTypes

• `Optional` **conversionTrackerTypes**: ``null`` \| [*ConversionTrackerServiceType*](./enums/conversiontrackerservicetype.md)[]

**`memberof`** ConversionTrackerServiceSelector

___

### countingType

• `Optional` **countingType**: ``null`` \| [*OnePerClick*](./enums/conversiontrackerservicecountingtype.md#oneperclick) \| [*ManyPerClick*](./enums/conversiontrackerservicecountingtype.md#manyperclick) \| [*Unknown*](./enums/conversiontrackerservicecountingtype.md#unknown)

**`memberof`** ConversionTrackerServiceSelector

___

### excludeFromBidding

• `Optional` **excludeFromBidding**: ``null`` \| [*False*](./enums/conversiontrackerserviceexcludefrombidding.md#false) \| [*True*](./enums/conversiontrackerserviceexcludefrombidding.md#true) \| [*Unknown*](./enums/conversiontrackerserviceexcludefrombidding.md#unknown)

**`memberof`** ConversionTrackerServiceSelector

___

### numberResults

• `Optional` **numberResults**: ``null`` \| *number*

<div lang=\"ja\">ページの最大件数です。このフィールドは、1以上を指定する必要があります。</div> 

**`memberof`** ConversionTrackerServiceSelector

___

### startIndex

• `Optional` **startIndex**: ``null`` \| *number*

<div lang=\"ja\">ページの先頭のインデックスです。このフィールドは、1以上を指定する必要があります。</div> 

**`memberof`** ConversionTrackerServiceSelector

___

### statsPeriod

• `Optional` **statsPeriod**: ``null`` \| [*DefiniteValueYesterday*](./enums/conversiontrackerservicestatsperiod.md#definitevalueyesterday) \| [*DefiniteValueLastbsday*](./enums/conversiontrackerservicestatsperiod.md#definitevaluelastbsday) \| [*DefiniteValueLastweek*](./enums/conversiontrackerservicestatsperiod.md#definitevaluelastweek) \| [*DefiniteValueWeek*](./enums/conversiontrackerservicestatsperiod.md#definitevalueweek) \| [*DefiniteValueTwoweek*](./enums/conversiontrackerservicestatsperiod.md#definitevaluetwoweek) \| [*DefiniteValueThirtyday*](./enums/conversiontrackerservicestatsperiod.md#definitevaluethirtyday) \| [*DefiniteValueLastmonth*](./enums/conversiontrackerservicestatsperiod.md#definitevaluelastmonth) \| [*RealtimeToday*](./enums/conversiontrackerservicestatsperiod.md#realtimetoday) \| [*RealtimeMonth*](./enums/conversiontrackerservicestatsperiod.md#realtimemonth) \| [*DefiniteValueLast13Month*](./enums/conversiontrackerservicestatsperiod.md#definitevaluelast13month) \| [*CustomDate*](./enums/conversiontrackerservicestatsperiod.md#customdate) \| [*Unknown*](./enums/conversiontrackerservicestatsperiod.md#unknown)

**`memberof`** ConversionTrackerServiceSelector

___

### statsPeriodCustomDate

• `Optional` **statsPeriodCustomDate**: ``null`` \| [*ConversionTrackerServiceStatsPeriodCustomDate*](conversiontrackerservicestatsperiodcustomdate.md)

**`memberof`** ConversionTrackerServiceSelector

___

### statuses

• `Optional` **statuses**: ``null`` \| [*ConversionTrackerServiceStatus*](./enums/conversiontrackerservicestatus.md)[]

**`memberof`** ConversionTrackerServiceSelector
