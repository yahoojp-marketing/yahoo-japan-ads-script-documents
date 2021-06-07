# ReportDefinition


<div lang=\"ja\">ReportDefinitionオブジェクトは、レポートの情報を表します。</div> </td>     <td>-</td>   </tr>   <tr>     <td>reportCompressType</td>     <td>-</td>     <td>Optional</td>     <td>-</td>   </tr>   <tr>     <td>reportDateRangeType</td>     <td>-</td>     <td>Requirement</td>     <td>-</td>   </tr>   <tr>     <td>reportDownloadFormat</td>     <td>-</td>     <td>Optional</td>     <td>-</td>   </tr>   <tr>     <td>reportLanguage</td>     <td>-</td>     <td>Optional</td>     <td>-</td>   </tr>   <tr>     <td>reportDownloadEncode</td>     <td>-</td>     <td>Optional</td>     <td>-</td>   </tr>   <tr>     <td>reportIncludeZeroImpressions</td>     <td>-</td>     <td>Optional</td>     <td>-</td>   </tr> </table></details>

## Table of contents

### Properties

- [accountId](reportdefinition.md#accountid)
- [completeTime](reportdefinition.md#completetime)
- [dateRange](reportdefinition.md#daterange)
- [fields](reportdefinition.md#fields)
- [filters](reportdefinition.md#filters)
- [reportCompressType](reportdefinition.md#reportcompresstype)
- [reportDateRangeType](reportdefinition.md#reportdaterangetype)
- [reportDownloadEncode](reportdefinition.md#reportdownloadencode)
- [reportDownloadFormat](reportdefinition.md#reportdownloadformat)
- [reportIncludeDeleted](reportdefinition.md#reportincludedeleted)
- [reportIncludeZeroImpressions](reportdefinition.md#reportincludezeroimpressions)
- [reportJobErrorDetail](reportdefinition.md#reportjoberrordetail)
- [reportJobId](reportdefinition.md#reportjobid)
- [reportJobStatus](reportdefinition.md#reportjobstatus)
- [reportLanguage](reportdefinition.md#reportlanguage)
- [reportName](reportdefinition.md#reportname)
- [reportType](reportdefinition.md#reporttype)
- [requestTime](reportdefinition.md#requesttime)
- [sortFields](reportdefinition.md#sortfields)

## Properties

### accountId

• `Optional` **accountId**: ``null`` \| *number*

<div lang=\"ja\">アカウントIDです。</div> 

**`memberof`** ReportDefinition

___

### completeTime

• `Optional` **completeTime**: ``null`` \| *string*

<div lang=\"ja\">ジョブの完了時刻です。<br> ※YYYY/MM/DD hh:mm:ss形式になります。<br> ※hhは24時間表記になります。</div> 

**`memberof`** ReportDefinition

___

### dateRange

• `Optional` **dateRange**: ``null`` \| [*ReportDefinitionServiceReportDateRange*](reportdefinitionservicereportdaterange.md)

**`memberof`** ReportDefinition

___

### fields

• `Optional` **fields**: ``null`` \| *string*[]

<div lang=\"ja\">フィールド（レポートの出力項目名）です。<br> ADD時、このフィールドは必須となります。</div> 

**`memberof`** ReportDefinition

___

### filters

• `Optional` **filters**: ``null`` \| [*ReportDefinitionServiceReportFilter*](reportdefinitionservicereportfilter.md)[]

**`memberof`** ReportDefinition

___

### reportCompressType

• `Optional` **reportCompressType**: ``null`` \| [*None*](./enums/reportdefinitionservicereportcompresstype.md#none) \| [*Zip*](./enums/reportdefinitionservicereportcompresstype.md#zip) \| [*Unknown*](./enums/reportdefinitionservicereportcompresstype.md#unknown)

**`memberof`** ReportDefinition

___

### reportDateRangeType

• `Optional` **reportDateRangeType**: ``null`` \| [*Today*](./enums/reportdefinitionservicereportdaterangetype.md#today) \| [*Yesterday*](./enums/reportdefinitionservicereportdaterangetype.md#yesterday) \| [*Last7Days*](./enums/reportdefinitionservicereportdaterangetype.md#last7days) \| [*LastWeek*](./enums/reportdefinitionservicereportdaterangetype.md#lastweek) \| [*Last14Days*](./enums/reportdefinitionservicereportdaterangetype.md#last14days) \| [*Last30Days*](./enums/reportdefinitionservicereportdaterangetype.md#last30days) \| [*LastBusinessWeek*](./enums/reportdefinitionservicereportdaterangetype.md#lastbusinessweek) \| [*ThisMonth*](./enums/reportdefinitionservicereportdaterangetype.md#thismonth) \| [*LastMonth*](./enums/reportdefinitionservicereportdaterangetype.md#lastmonth) \| [*AllTime*](./enums/reportdefinitionservicereportdaterangetype.md#alltime) \| [*CustomDate*](./enums/reportdefinitionservicereportdaterangetype.md#customdate) \| [*Unknown*](./enums/reportdefinitionservicereportdaterangetype.md#unknown)

**`memberof`** ReportDefinition

___

### reportDownloadEncode

• `Optional` **reportDownloadEncode**: ``null`` \| [*Utf8*](./enums/reportdefinitionservicereportdownloadencode.md#utf8) \| [*Sjis*](./enums/reportdefinitionservicereportdownloadencode.md#sjis) \| [*Euc*](./enums/reportdefinitionservicereportdownloadencode.md#euc) \| [*Utf16Le*](./enums/reportdefinitionservicereportdownloadencode.md#utf16le) \| [*Unknown*](./enums/reportdefinitionservicereportdownloadencode.md#unknown)

**`memberof`** ReportDefinition

___

### reportDownloadFormat

• `Optional` **reportDownloadFormat**: ``null`` \| [*Csv*](./enums/reportdefinitionservicereportdownloadformat.md#csv) \| [*Xml*](./enums/reportdefinitionservicereportdownloadformat.md#xml) \| [*Tsv*](./enums/reportdefinitionservicereportdownloadformat.md#tsv) \| [*Unknown*](./enums/reportdefinitionservicereportdownloadformat.md#unknown)

**`memberof`** ReportDefinition

___

### reportIncludeDeleted

• `Optional` **reportIncludeDeleted**: ``null`` \| [*True*](./enums/reportdefinitionservicereportincludedeleted.md#true) \| [*False*](./enums/reportdefinitionservicereportincludedeleted.md#false) \| [*Unknown*](./enums/reportdefinitionservicereportincludedeleted.md#unknown)

**`memberof`** ReportDefinition

___

### reportIncludeZeroImpressions

• `Optional` **reportIncludeZeroImpressions**: ``null`` \| [*True*](./enums/reportdefinitionservicereportincludezeroimpressions.md#true) \| [*False*](./enums/reportdefinitionservicereportincludezeroimpressions.md#false) \| [*Unknown*](./enums/reportdefinitionservicereportincludezeroimpressions.md#unknown)

**`memberof`** ReportDefinition

___

### reportJobErrorDetail

• `Optional` **reportJobErrorDetail**: ``null`` \| *string*

<div lang=\"ja\">レポートジョブのエラー詳細です。</div> 

**`memberof`** ReportDefinition

___

### reportJobId

• `Optional` **reportJobId**: ``null`` \| *number*

<div lang=\"ja\">レポートジョブIDです。<br> REMOVE時、このフィールドは必須となります。</div> 

**`memberof`** ReportDefinition

___

### reportJobStatus

• `Optional` **reportJobStatus**: ``null`` \| [*Wait*](./enums/reportdefinitionservicereportjobstatus.md#wait) \| [*Completed*](./enums/reportdefinitionservicereportjobstatus.md#completed) \| [*InProgress*](./enums/reportdefinitionservicereportjobstatus.md#inprogress) \| [*Failed*](./enums/reportdefinitionservicereportjobstatus.md#failed) \| [*Unknown*](./enums/reportdefinitionservicereportjobstatus.md#unknown)

**`memberof`** ReportDefinition

___

### reportLanguage

• `Optional` **reportLanguage**: ``null`` \| [*Ja*](./enums/reportdefinitionservicereportlanguage.md#ja) \| [*En*](./enums/reportdefinitionservicereportlanguage.md#en) \| [*Unknown*](./enums/reportdefinitionservicereportlanguage.md#unknown)

**`memberof`** ReportDefinition

___

### reportName

• `Optional` **reportName**: ``null`` \| *string*

<div lang=\"ja\">レポート名称です。<br> ADD時、このフィールドは必須となります。</div> 

**`memberof`** ReportDefinition

___

### reportType

• `Optional` **reportType**: ``null`` \| [*Account*](./enums/reportdefinitionservicereporttype.md#account) \| [*Campaign*](./enums/reportdefinitionservicereporttype.md#campaign) \| [*Adgroup*](./enums/reportdefinitionservicereporttype.md#adgroup) \| [*Ad*](./enums/reportdefinitionservicereporttype.md#ad) \| [*Keywords*](./enums/reportdefinitionservicereporttype.md#keywords) \| [*SearchQuery*](./enums/reportdefinitionservicereporttype.md#searchquery) \| [*Geo*](./enums/reportdefinitionservicereporttype.md#geo) \| [*FeedItem*](./enums/reportdefinitionservicereporttype.md#feeditem) \| [*GeoTarget*](./enums/reportdefinitionservicereporttype.md#geotarget) \| [*ScheduleTarget*](./enums/reportdefinitionservicereporttype.md#scheduletarget) \| [*BidStrategy*](./enums/reportdefinitionservicereporttype.md#bidstrategy) \| [*AdCustomizers*](./enums/reportdefinitionservicereporttype.md#adcustomizers) \| [*TargetList*](./enums/reportdefinitionservicereporttype.md#targetlist) \| [*LandingPageUrl*](./enums/reportdefinitionservicereporttype.md#landingpageurl) \| [*KeywordlessQuery*](./enums/reportdefinitionservicereporttype.md#keywordlessquery) \| [*WebpageCriterion*](./enums/reportdefinitionservicereporttype.md#webpagecriterion) \| [*Unknown*](./enums/reportdefinitionservicereporttype.md#unknown)

**`memberof`** ReportDefinition

___

### requestTime

• `Optional` **requestTime**: ``null`` \| *string*

<div lang=\"ja\">ジョブの起動時刻です。<br> ※YYYY/MM/DD hh:mm:ss形式になります。<br> ※hhは24時間表記になります。</div> 

**`memberof`** ReportDefinition

___

### sortFields

• `Optional` **sortFields**: ``null`` \| [*ReportDefinitionServiceReportSortField*](reportdefinitionservicereportsortfield.md)[]

**`memberof`** ReportDefinition
