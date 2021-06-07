# Enumeration: ReportDefinitionServiceReportDateRangeType


<div lang=\"ja\"> ReportDefinitionServiceReportDateRangeTypeは、レポートの集計対象期間を表します。<br> このフィールドは、ADD時に必須となり、REMOVE時に無視されます。<br> 本日分を含む実績値を取得する(TODAY/CUSTOM_DATEで本日を含む)場合、以下の制約があります。<br> - 本日分の実績値は、その時点での速報値です。取得タイミングによって速報値は変動するため、4〜5時間前の実績値となる可能性があります。<br> - StatsServiceや広告管理ツールによる本日分の実績値とは、数値が異なる可能性があります。<br> - フリークエンシーレポートとリーチレポートでは、本日分の実績値は取得できません。<br> - 本日分の実績値は、翌朝5時(JST)前後に確定します。<br> </div>  <dl class=term>   <dt class=\"term__item\">LAST_7_DAYS</dt>   <dd class=\"term__desc\"><span lang=\"ja\">本日を除く、過去7日間です。</span></dd>   <dt class=\"term__item\">LAST_MONTH</dt>   <dd class=\"term__desc\"><span lang=\"ja\">前月です。</span></dd>   <dt class=\"term__item\">THIS_MONTH</dt>   <dd class=\"term__desc\"><span lang=\"ja\">本日を除く、当月です。</span></dd>   <dt class=\"term__item\">TODAY</dt>   <dd class=\"term__desc\"><span lang=\"ja\">本日です。</span></dd>   <dt class=\"term__item\">YESTERDAY</dt>   <dd class=\"term__desc\"><span lang=\"ja\">昨日です。</span></dd>   <dt class=\"term__item\">LAST_30_DAYS</dt>   <dd class=\"term__desc\"><span lang=\"ja\">本日を除く、過去30日間です。</span></dd>   <dt class=\"term__item\">LAST_14_DAYS</dt>   <dd class=\"term__desc\"><span lang=\"ja\">本日を除く、過去14日間です。</span></dd>   <dt class=\"term__item\">CUSTOM_DATE</dt>   <dd class=\"term__desc\"><span lang=\"ja\">ユーザーにより指定される期間です。CUSTOM_DATEを指定した場合、集計対象期間の指定が必要です。<br>※ReportType : REACHでは指定不可</span><span lang=\"en\">Reports are generated for the date range specified byDateRange. If select CUSTOM_DATE, DateRange must be input.<br>* CUSTOM_DATE cannot be specified if ReportType = REACH.</span></dd>   <dt class=\"term__item\">LAST_WEEK</dt>   <dd class=\"term__desc\"><span lang=\"ja\">先週の月曜日から日曜日です。</span></dd>   <dt class=\"term__item\">LAST_BUSINESS_WEEK</dt>   <dd class=\"term__desc\"><span lang=\"ja\">先週の月曜日から5営業日です。</span></dd>   <dt class=\"term__item\">GUARANTEED_CAMPAIGN_PERIOD</dt>   <dd class=\"term__desc\">   <span lang=\"ja\">     通期です。<br>     リーチレポートでのみ指定可能です。<br>     通期を指定する場合は、frequencyRangeでもGUARANTEED_CAMPAIGN_PERIODを指定する必要があります。<br>     ※この「通期」は、予約型キャンペーンの開始から終了までの全期間を意味します。   </span>   <span lang=\"en\">     Lifetime.<br>     Can be specified only in the reach report.<br>     If specified this, \"GUARANTEED_CAMPAIGN_PERIOD\" must be specified for frequencyRange as well.<br>     * \"lifetime\" means the entire period from the start to the end of the guaranteed campaign.   </span> </dd>   <dt class=\"term__item\">UNKNOWN</dt>   <dd class=\"term__desc\"><span lang=\"ja\">未知の値です。</span></dd> </dl>

## Table of contents

### Enumeration members

- [CustomDate](reportdefinitionservicereportdaterangetype.md#customdate)
- [GuaranteedCampaignPeriod](reportdefinitionservicereportdaterangetype.md#guaranteedcampaignperiod)
- [Last14Days](reportdefinitionservicereportdaterangetype.md#last14days)
- [Last30Days](reportdefinitionservicereportdaterangetype.md#last30days)
- [Last7Days](reportdefinitionservicereportdaterangetype.md#last7days)
- [LastBusinessWeek](reportdefinitionservicereportdaterangetype.md#lastbusinessweek)
- [LastMonth](reportdefinitionservicereportdaterangetype.md#lastmonth)
- [LastWeek](reportdefinitionservicereportdaterangetype.md#lastweek)
- [ThisMonth](reportdefinitionservicereportdaterangetype.md#thismonth)
- [Today](reportdefinitionservicereportdaterangetype.md#today)
- [Unknown](reportdefinitionservicereportdaterangetype.md#unknown)
- [Yesterday](reportdefinitionservicereportdaterangetype.md#yesterday)

## Enumeration members

### CustomDate

• **CustomDate**: = "CUSTOM\_DATE"

___

### GuaranteedCampaignPeriod

• **GuaranteedCampaignPeriod**: = "GUARANTEED\_CAMPAIGN\_PERIOD"

___

### Last14Days

• **Last14Days**: = "LAST\_14\_DAYS"

___

### Last30Days

• **Last30Days**: = "LAST\_30\_DAYS"

___

### Last7Days

• **Last7Days**: = "LAST\_7\_DAYS"

___

### LastBusinessWeek

• **LastBusinessWeek**: = "LAST\_BUSINESS\_WEEK"

___

### LastMonth

• **LastMonth**: = "LAST\_MONTH"

___

### LastWeek

• **LastWeek**: = "LAST\_WEEK"

___

### ThisMonth

• **ThisMonth**: = "THIS\_MONTH"

___

### Today

• **Today**: = "TODAY"

___

### Unknown

• **Unknown**: = "UNKNOWN"

___

### Yesterday

• **Yesterday**: = "YESTERDAY"
