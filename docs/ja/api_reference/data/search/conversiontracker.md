# ConversionTracker


<div lang=\"ja\">ConversionTrackerオブジェクトは、コンバージョン測定タグやタグごとのパフォーマンスデータなどのコンバージョントラッカー情報を表します。</div> 

## Table of contents

### Properties

- [accountId](conversiontracker.md#accountid)
- [allConversionValue](conversiontracker.md#allconversionvalue)
- [allConversions](conversiontracker.md#allconversions)
- [appConversion](conversiontracker.md#appconversion)
- [appLinkConversion](conversiontracker.md#applinkconversion)
- [category](conversiontracker.md#category)
- [conversionCountingType](conversiontracker.md#conversioncountingtype)
- [conversionTrackerId](conversiontracker.md#conversiontrackerid)
- [conversionTrackerName](conversiontracker.md#conversiontrackername)
- [conversionTrackerTrackId](conversiontracker.md#conversiontrackertrackid)
- [conversionTrackerType](conversiontracker.md#conversiontrackertype)
- [conversionValue](conversiontracker.md#conversionvalue)
- [conversions](conversiontracker.md#conversions)
- [excludeFromBidding](conversiontracker.md#excludefrombidding)
- [measurementPeriod](conversiontracker.md#measurementperiod)
- [mostRecentConversionDate](conversiontracker.md#mostrecentconversiondate)
- [status](conversiontracker.md#status)
- [userRevenueValue](conversiontracker.md#userrevenuevalue)
- [webConversion](conversiontracker.md#webconversion)

## Properties

### accountId

• `Optional` **accountId**: ``null`` \| *number*

<div lang=\"ja\">アカウントIDです。</div> 

**`memberof`** ConversionTracker

___

### allConversionValue

• `Optional` **allConversionValue**: ``null`` \| *string*

<div lang=\"ja\">自動入札設定対象のコンバージョン値と、対象外のコンバージョン値の合計です。</div> 

**`memberof`** ConversionTracker

___

### allConversions

• `Optional` **allConversions**: ``null`` \| *number*

<div lang=\"ja\">自動入札設定対象のコンバージョン数と、対象外のコンバージョン数の合計です。</div> 

**`memberof`** ConversionTracker

___

### appConversion

• `Optional` **appConversion**: ``null`` \| [*ConversionTrackerServiceAppConversion*](conversiontrackerserviceappconversion.md)

**`memberof`** ConversionTracker

___

### appLinkConversion

• `Optional` **appLinkConversion**: ``null`` \| [*ConversionTrackerServiceAppLinkConversion*](conversiontrackerserviceapplinkconversion.md)

**`memberof`** ConversionTracker

___

### category

• `Optional` **category**: ``null`` \| [*Default*](./enums/conversiontrackerservicecategory.md#default) \| [*PageView*](./enums/conversiontrackerservicecategory.md#pageview) \| [*Purchase*](./enums/conversiontrackerservicecategory.md#purchase) \| [*Signup*](./enums/conversiontrackerservicecategory.md#signup) \| [*Lead*](./enums/conversiontrackerservicecategory.md#lead) \| [*Download*](./enums/conversiontrackerservicecategory.md#download) \| [*Unknown*](./enums/conversiontrackerservicecategory.md#unknown)

**`memberof`** ConversionTracker

___

### conversionCountingType

• `Optional` **conversionCountingType**: ``null`` \| [*OnePerClick*](./enums/conversiontrackerserviceconversioncountingtype.md#oneperclick) \| [*ManyPerClick*](./enums/conversiontrackerserviceconversioncountingtype.md#manyperclick) \| [*Unknown*](./enums/conversiontrackerserviceconversioncountingtype.md#unknown)

**`memberof`** ConversionTracker

___

### conversionTrackerId

• `Optional` **conversionTrackerId**: ``null`` \| *number*

<div lang=\"ja\">コンバージョントラッカーのIDです。<br> このフィールドは、SET時に必須となります。</div> 

**`memberof`** ConversionTracker

___

### conversionTrackerName

• `Optional` **conversionTrackerName**: ``null`` \| *string*

<div lang=\"ja\">コンバージョントラッカーの名称です。<br> このフィールドは、ADD時に必須となり、SET時に省略可能となります。</div> 

**`memberof`** ConversionTracker

___

### conversionTrackerTrackId

• `Optional` **conversionTrackerTrackId**: ``null`` \| *number*

<div lang=\"ja\">トラッキング用コンバージョントラッカーIDです。<br> ADD時、このフィールドは省略可能となります。※conversionTrackerTypeがAPP_LINK_CONVERSIONの場合は必須です。</div> 

**`memberof`** ConversionTracker

___

### conversionTrackerType

• `Optional` **conversionTrackerType**: ``null`` \| [*WebConversion*](./enums/conversiontrackerserviceconversiontrackertype.md#webconversion) \| [*AppConversion*](./enums/conversiontrackerserviceconversiontrackertype.md#appconversion) \| [*AppLinkConversion*](./enums/conversiontrackerserviceconversiontrackertype.md#applinkconversion) \| [*Unknown*](./enums/conversiontrackerserviceconversiontrackertype.md#unknown)

**`memberof`** ConversionTracker

___

### conversionValue

• `Optional` **conversionValue**: ``null`` \| *string*

<div lang=\"ja\">自動入札設定対象のコンバージョン値です。</div> 

**`memberof`** ConversionTracker

___

### conversions

• `Optional` **conversions**: ``null`` \| *number*

<div lang=\"ja\">自動入札設定対象のコンバージョン数です。<br> ユニークコンバージョンか総コンバージョンかは、countingTypeに依存します。</div> 

**`memberof`** ConversionTracker

___

### excludeFromBidding

• `Optional` **excludeFromBidding**: ``null`` \| [*True*](./enums/conversiontrackerserviceexcludefrombidding.md#true) \| [*False*](./enums/conversiontrackerserviceexcludefrombidding.md#false) \| [*Unknown*](./enums/conversiontrackerserviceexcludefrombidding.md#unknown)

**`memberof`** ConversionTracker

___

### measurementPeriod

• `Optional` **measurementPeriod**: ``null`` \| *number*

<div lang=\"ja\">コンバージョン計測期間です（単位：日)。<br> 7～90日間で設定可能です。<br>※アプリダウンロードの場合は30日間固定。<br> このフィールドは、ADDおよびSET時に省略可能となります。<br>※ADD時のデフォルト設定値は30となります。</div> 

**`memberof`** ConversionTracker

___

### mostRecentConversionDate

• `Optional` **mostRecentConversionDate**: ``null`` \| *string*

<div lang=\"ja\">直近のコンバージョン発生日です。</div> 

**`memberof`** ConversionTracker

___

### status

• `Optional` **status**: ``null`` \| [*Enabled*](./enums/conversiontrackerservicestatus.md#enabled) \| [*Disabled*](./enums/conversiontrackerservicestatus.md#disabled) \| [*Unknown*](./enums/conversiontrackerservicestatus.md#unknown)

**`memberof`** ConversionTracker

___

### userRevenueValue

• `Optional` **userRevenueValue**: ``null`` \| *string*

<div lang=\"ja\">このコンバージョントラッカーに対するユーザー指定の収益値です。<br> 1コンバージョンあたりの売上金額が固定値の場合、その金額を設定することで、売上金額をレポートなどで確認できます。<br> ADDリクエスト時に未指定の場合、0が設定されます。<br> このフィールドは、ADD時およびSET時に省略可能となります。</div> 

**`memberof`** ConversionTracker

___

### webConversion

• `Optional` **webConversion**: ``null`` \| [*ConversionTrackerServiceWebConversion*](conversiontrackerservicewebconversion.md)

**`memberof`** ConversionTracker
