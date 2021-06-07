# KeywordForecastMetricsServiceSelector


<div lang=\"ja\">KeywordForecastMetricsServiceSelector オブジェクトは、見積もりリクエストを格納します。</div> 

## Table of contents

### Properties

- [accountId](keywordforecastmetricsserviceselector.md#accountid)
- [dateInterval](keywordforecastmetricsserviceselector.md#dateinterval)
- [endDate](keywordforecastmetricsserviceselector.md#enddate)
- [keywordPlanCampaign](keywordforecastmetricsserviceselector.md#keywordplancampaign)
- [startDate](keywordforecastmetricsserviceselector.md#startdate)

## Properties

### accountId

• **accountId**: *number*

<div lang=\"ja\">アカウントIDです。</div> 

**`memberof`** KeywordForecastMetricsServiceSelector

___

### dateInterval

• **dateInterval**: ``null`` \| [*NextWeek*](./enums/keywordforecastmetricsservicedateinterval.md#nextweek) \| [*NextMonth*](./enums/keywordforecastmetricsservicedateinterval.md#nextmonth) \| [*NextQuarter*](./enums/keywordforecastmetricsservicedateinterval.md#nextquarter) \| [*CustomDate*](./enums/keywordforecastmetricsservicedateinterval.md#customdate) \| [*Unknown*](./enums/keywordforecastmetricsservicedateinterval.md#unknown)

**`memberof`** KeywordForecastMetricsServiceSelector

___

### endDate

• `Optional` **endDate**: ``null`` \| *string*

<div lang=\"ja\">dateIntervalがCUSTOM_DATEのときに指定する終了日です。<br> 現在より先の日付、かつ一年未満である必要があります。<br> ※フォーマット：yyyyMMdd</div> 

**`memberof`** KeywordForecastMetricsServiceSelector

___

### keywordPlanCampaign

• **keywordPlanCampaign**: ``null`` \| [*KeywordForecastMetricsServiceKeywordPlanCampaign*](keywordforecastmetricsservicekeywordplancampaign.md)

**`memberof`** KeywordForecastMetricsServiceSelector

___

### startDate

• `Optional` **startDate**: ``null`` \| *string*

<div lang=\"ja\">dateIntervalがCUSTOM_DATEのときに指定する開始日です。<br> 現在より先の日付、かつ一年未満である必要があります。<br> ※フォーマット：yyyyMMdd</div> 

**`memberof`** KeywordForecastMetricsServiceSelector
