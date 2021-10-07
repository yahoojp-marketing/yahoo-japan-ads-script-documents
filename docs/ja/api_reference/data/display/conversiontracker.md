# ConversionTracker


<div lang=\"ja\">ConversionTrackerオブジェクトは、コンバージョン測定タグやタグごとのパフォーマンスデータなどのコンバージョントラッカー情報を表します。</div> 

## Table of contents

### Properties

- [accountId](conversiontracker.md#accountid)
- [allConversionValue](conversiontracker.md#allconversionvalue)
- [allConversions](conversiontracker.md#allconversions)
- [appConversion](conversiontracker.md#appconversion)
- [category](conversiontracker.md#category)
- [conversionTrackerId](conversiontracker.md#conversiontrackerid)
- [conversionTrackerName](conversiontracker.md#conversiontrackername)
- [conversionTrackerType](conversiontracker.md#conversiontrackertype)
- [conversionValue](conversiontracker.md#conversionvalue)
- [conversionValueViaAdClick](conversiontracker.md#conversionvalueviaadclick)
- [conversions](conversiontracker.md#conversions)
- [conversionsViaAdClick](conversiontracker.md#conversionsviaadclick)
- [countingType](conversiontracker.md#countingtype)
- [crossDeviceConversions](conversiontracker.md#crossdeviceconversions)
- [excludeFromBidding](conversiontracker.md#excludefrombidding)
- [isPreviousConversion](conversiontracker.md#ispreviousconversion)
- [measurementPeriod](conversiontracker.md#measurementperiod)
- [measurementPeriodView](conversiontracker.md#measurementperiodview)
- [mostRecentConversionDate](conversiontracker.md#mostrecentconversiondate)
- [status](conversiontracker.md#status)
- [userRevenueValue](conversiontracker.md#userrevenuevalue)
- [viewThroughConversions](conversiontracker.md#viewthroughconversions)
- [webConversion](conversiontracker.md#webconversion)

## Properties

### accountId

• `Optional` **accountId**: ``null`` \| *number*

<div lang=\"ja\"> アカウントIDです。<br> このフィールドは、レスポンスの際に返却されますが、リクエストの際には無視されます。 </div> 

**`memberof`** ConversionTracker

___

### allConversionValue

• `Optional` **allConversionValue**: ``null`` \| *string*

<div lang=\"ja\"> コンバージョンの価値（全て）です。 </div> 

**`memberof`** ConversionTracker

___

### allConversions

• `Optional` **allConversions**: ``null`` \| *number*

<div lang=\"ja\"> コンバージョン数（全て）です。<br> このフィールドは、レスポンスの際に返却されますが、リクエストの際には無視されます。 </div> 

**`memberof`** ConversionTracker

___

### appConversion

• `Optional` **appConversion**: ``null`` \| [*ConversionTrackerServiceAppConversion*](conversiontrackerserviceappconversion.md)

**`memberof`** ConversionTracker

___

### category

• `Optional` **category**: ``null`` \| [*None*](./enums/conversiontrackerservicecategory.md#none) \| [*Default*](./enums/conversiontrackerservicecategory.md#default) \| [*PageView*](./enums/conversiontrackerservicecategory.md#pageview) \| [*Purchase*](./enums/conversiontrackerservicecategory.md#purchase) \| [*Signup*](./enums/conversiontrackerservicecategory.md#signup) \| [*Lead*](./enums/conversiontrackerservicecategory.md#lead) \| [*Download*](./enums/conversiontrackerservicecategory.md#download) \| [*Unknown*](./enums/conversiontrackerservicecategory.md#unknown)

**`memberof`** ConversionTracker

___

### conversionTrackerId

• `Optional` **conversionTrackerId**: ``null`` \| *number*

<div lang=\"ja\"> コンバージョントラッカーIDです。<br> このフィールドは、ADD時は無視され、SET時は必須となります。 </div> 

**`memberof`** ConversionTracker

___

### conversionTrackerName

• `Optional` **conversionTrackerName**: ``null`` \| *string*

<div lang=\"ja\"> コンバージョントラッカー名です。<br> このフィールドは、ADD時は必須となり、SET時は省略可能となります。 </div> 

**`memberof`** ConversionTracker

___

### conversionTrackerType

• `Optional` **conversionTrackerType**: ``null`` \| [*WebConversion*](./enums/conversiontrackerservicetype.md#webconversion) \| [*AppConversion*](./enums/conversiontrackerservicetype.md#appconversion) \| [*Unknown*](./enums/conversiontrackerservicetype.md#unknown)

**`memberof`** ConversionTracker

___

### conversionValue

• `Optional` **conversionValue**: ``null`` \| *string*

<div lang=\"ja\"> コンバージョンの価値/コンバージョン数です。<br> このフィールドは、レスポンスの際に返却されますが、リクエストの際には無視されます。 </div> 

**`memberof`** ConversionTracker

___

### conversionValueViaAdClick

• `Optional` **conversionValueViaAdClick**: ``null`` \| *string*

<div lang=\"ja\"> コンバージョンの価値（クリック経由）です。<br> このフィールドは、レスポンスの際に返却されますが、リクエストの際には無視されます。 </div> 

**`memberof`** ConversionTracker

___

### conversions

• `Optional` **conversions**: ``null`` \| *number*

<div lang=\"ja\"> コンバージョン数です。<br> このフィールドは、レスポンスの際に返却されますが、リクエストの際には無視されます。 </div> 

**`memberof`** ConversionTracker

___

### conversionsViaAdClick

• `Optional` **conversionsViaAdClick**: ``null`` \| *number*

<div lang=\"ja\"> コンバージョン数（クリック経由）です。<br> このフィールドは、レスポンスの際に返却されますが、リクエストの際には無視されます。 </div> 

**`memberof`** ConversionTracker

___

### countingType

• `Optional` **countingType**: ``null`` \| [*OnePerClick*](./enums/conversiontrackerservicecountingtype.md#oneperclick) \| [*ManyPerClick*](./enums/conversiontrackerservicecountingtype.md#manyperclick) \| [*Unknown*](./enums/conversiontrackerservicecountingtype.md#unknown)

**`memberof`** ConversionTracker

___

### crossDeviceConversions

• `Optional` **crossDeviceConversions**: ``null`` \| *number*

<div lang=\"ja\"> クロスデバイスコンバージョン数です。<br> このフィールドは、レスポンスの際に返却されますが、リクエストの際には無視されます。 </div> 

**`memberof`** ConversionTracker

___

### excludeFromBidding

• `Optional` **excludeFromBidding**: ``null`` \| [*False*](./enums/conversiontrackerserviceexcludefrombidding.md#false) \| [*True*](./enums/conversiontrackerserviceexcludefrombidding.md#true) \| [*Unknown*](./enums/conversiontrackerserviceexcludefrombidding.md#unknown)

**`memberof`** ConversionTracker

___

### isPreviousConversion

• `Optional` **isPreviousConversion**: ``null`` \| [*True*](./enums/conversiontrackerserviceispreviousconversion.md#true) \| [*False*](./enums/conversiontrackerserviceispreviousconversion.md#false) \| [*Unknown*](./enums/conversiontrackerserviceispreviousconversion.md#unknown)

**`memberof`** ConversionTracker

___

### measurementPeriod

• `Optional` **measurementPeriod**: ``null`` \| *number*

<div lang=\"ja\"> 計測期間（単位：日）です。<br> ※7～90の範囲内で指定可能です。<br> このフィールドは、リクエストの場合は省略可能です。ADD時のデフォルト設定値は30となります。 </div> 

**`memberof`** ConversionTracker

___

### measurementPeriodView

• `Optional` **measurementPeriodView**: ``null`` \| *number*

<div lang=\"ja\"> 測定期間（動画視聴）<br> ※1-30の範囲で指定可能です。<br> このフィールドは、リクエストの場合は省略可能です。ADD時のデフォルト設定値は1となります。 </div> 

**`memberof`** ConversionTracker

___

### mostRecentConversionDate

• `Optional` **mostRecentConversionDate**: ``null`` \| *string*

<div lang=\"ja\"> コンバージョンが発生した直近の日付です。<br> ※YYYYMMDD形式です。<br> このフィールドは、レスポンスの際に返却されますが、リクエストの際には無視されます。 </div> 

**`memberof`** ConversionTracker

___

### status

• `Optional` **status**: ``null`` \| [*Enabled*](./enums/conversiontrackerservicestatus.md#enabled) \| [*Disabled*](./enums/conversiontrackerservicestatus.md#disabled) \| [*Unknown*](./enums/conversiontrackerservicestatus.md#unknown)

**`memberof`** ConversionTracker

___

### userRevenueValue

• `Optional` **userRevenueValue**: ``null`` \| *number*

<div lang=\"ja\"> コンバージョンの収益値です。<br> このフィールドは、リクエストの場合は省略可能です。ADD時のデフォルト設定値は0となります。 </div> 

**`memberof`** ConversionTracker

___

### viewThroughConversions

• `Optional` **viewThroughConversions**: ``null`` \| *number*

<div lang=\"ja\">ビュースルーコンバージョン数</div> 

**`memberof`** ConversionTracker

___

### webConversion

• `Optional` **webConversion**: ``null`` \| [*ConversionTrackerServiceWebConversion*](conversiontrackerservicewebconversion.md)

**`memberof`** ConversionTracker
