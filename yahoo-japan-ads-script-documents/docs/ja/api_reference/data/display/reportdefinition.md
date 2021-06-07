# ReportDefinition


<div lang=\"ja\">ReportDefinitionオブジェクトは、レポート定義を表します。</div> 

## Table of contents

### Properties

- [accountId](reportdefinition.md#accountid)
- [completeTime](reportdefinition.md#completetime)
- [dateRange](reportdefinition.md#daterange)
- [fields](reportdefinition.md#fields)
- [filters](reportdefinition.md#filters)
- [reportCompressType](reportdefinition.md#reportcompresstype)
- [reportDateRangeType](reportdefinition.md#reportdaterangetype)
- [reportDecimalPartDisplayType](reportdefinition.md#reportdecimalpartdisplaytype)
- [reportDownloadEncode](reportdefinition.md#reportdownloadencode)
- [reportDownloadFormat](reportdefinition.md#reportdownloadformat)
- [reportJobErrorDetail](reportdefinition.md#reportjoberrordetail)
- [reportJobId](reportdefinition.md#reportjobid)
- [reportJobStatus](reportdefinition.md#reportjobstatus)
- [reportLanguage](reportdefinition.md#reportlanguage)
- [reportName](reportdefinition.md#reportname)
- [reportSkipColumnHeader](reportdefinition.md#reportskipcolumnheader)
- [reportSkipReportSummary](reportdefinition.md#reportskipreportsummary)
- [reportTypeCondition](reportdefinition.md#reporttypecondition)
- [requestTime](reportdefinition.md#requesttime)
- [sortFields](reportdefinition.md#sortfields)

## Properties

### accountId

• `Optional` **accountId**: ``null`` \| *number*

<div lang=\"ja\"> アカウントIDです。<br> このフィールドは、レスポンスの際に返却されますが、リクエストの際には無視されます。 </div> 

**`memberof`** ReportDefinition

___

### completeTime

• `Optional` **completeTime**: ``null`` \| *string*

<div lang=\"ja\"> ジョブ完了日時です。<br> このフィールドは、レスポンスの際に返却されますが、リクエストの際には無視されます。 </div> 

**`memberof`** ReportDefinition

___

### dateRange

• `Optional` **dateRange**: ``null`` \| [*ReportDefinitionServiceDateRange*](reportdefinitionservicedaterange.md)

**`memberof`** ReportDefinition

___

### fields

• `Optional` **fields**: ``null`` \| *string*[]

<div lang=\"ja\"> 表示項目です。<br> このフィールドは、ADD時に必須となり、REMOVE時に無視されます。<br> 指定可能な値は、ReportDefinitionServiceのgetReportFieldsで取得されるfieldNameをご確認ください。 </div> 

**`memberof`** ReportDefinition

___

### filters

• `Optional` **filters**: ``null`` \| [*ReportDefinitionServiceFilter*](reportdefinitionservicefilter.md)[]

**`memberof`** ReportDefinition

___

### reportCompressType

• `Optional` **reportCompressType**: ``null`` \| [*None*](./enums/reportdefinitionservicereportcompresstype.md#none) \| [*Zip*](./enums/reportdefinitionservicereportcompresstype.md#zip) \| [*Unknown*](./enums/reportdefinitionservicereportcompresstype.md#unknown)

**`memberof`** ReportDefinition

___

### reportDateRangeType

• `Optional` **reportDateRangeType**: ``null`` \| [*CustomDate*](./enums/reportdefinitionservicereportdaterangetype.md#customdate) \| [*Today*](./enums/reportdefinitionservicereportdaterangetype.md#today) \| [*Yesterday*](./enums/reportdefinitionservicereportdaterangetype.md#yesterday) \| [*Last7Days*](./enums/reportdefinitionservicereportdaterangetype.md#last7days) \| [*LastWeek*](./enums/reportdefinitionservicereportdaterangetype.md#lastweek) \| [*LastBusinessWeek*](./enums/reportdefinitionservicereportdaterangetype.md#lastbusinessweek) \| [*Last14Days*](./enums/reportdefinitionservicereportdaterangetype.md#last14days) \| [*Last30Days*](./enums/reportdefinitionservicereportdaterangetype.md#last30days) \| [*ThisMonth*](./enums/reportdefinitionservicereportdaterangetype.md#thismonth) \| [*LastMonth*](./enums/reportdefinitionservicereportdaterangetype.md#lastmonth) \| [*GuaranteedCampaignPeriod*](./enums/reportdefinitionservicereportdaterangetype.md#guaranteedcampaignperiod) \| [*Unknown*](./enums/reportdefinitionservicereportdaterangetype.md#unknown)

**`memberof`** ReportDefinition

___

### reportDecimalPartDisplayType

• `Optional` **reportDecimalPartDisplayType**: ``null`` \| [*FullDisplay*](./enums/reportdefinitionservicereportdecimalpartdisplaytype.md#fulldisplay) \| [*SimpleDisplay*](./enums/reportdefinitionservicereportdecimalpartdisplaytype.md#simpledisplay) \| [*Unknown*](./enums/reportdefinitionservicereportdecimalpartdisplaytype.md#unknown)

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

### reportJobErrorDetail

• `Optional` **reportJobErrorDetail**: ``null`` \| *string*

<div lang=\"ja\"> ジョブエラー詳細です。<br> このフィールドは、レスポンスの際に返却されますが、リクエストの際には無視されます。<br> 「Over limit of file size.」が返される場合は、レポートのサイズが小さくなるようにレポート作成時の条件を変更してください。 </div> 

**`memberof`** ReportDefinition

___

### reportJobId

• `Optional` **reportJobId**: ``null`` \| *number*

<div lang=\"ja\"> レポートジョブIDです。<br> このフィールドは、REMOVE時に必須となり、ADD時に無視されます。 </div> 

**`memberof`** ReportDefinition

___

### reportJobStatus

• `Optional` **reportJobStatus**: ``null`` \| [*Wait*](./enums/reportdefinitionservicereportjobstatus.md#wait) \| [*InProgress*](./enums/reportdefinitionservicereportjobstatus.md#inprogress) \| [*Completed*](./enums/reportdefinitionservicereportjobstatus.md#completed) \| [*Canceled*](./enums/reportdefinitionservicereportjobstatus.md#canceled) \| [*Failed*](./enums/reportdefinitionservicereportjobstatus.md#failed) \| [*Unknown*](./enums/reportdefinitionservicereportjobstatus.md#unknown)

**`memberof`** ReportDefinition

___

### reportLanguage

• `Optional` **reportLanguage**: ``null`` \| [*Ja*](./enums/reportdefinitionservicereportlanguage.md#ja) \| [*En*](./enums/reportdefinitionservicereportlanguage.md#en) \| [*Unknown*](./enums/reportdefinitionservicereportlanguage.md#unknown)

**`memberof`** ReportDefinition

___

### reportName

• `Optional` **reportName**: ``null`` \| *string*

<div lang=\"ja\"> レポート名です。<br> このフィールドは、ADD時に省略可能となり、REMOVE時に無視されます。 </div> 

**`memberof`** ReportDefinition

___

### reportSkipColumnHeader

• `Optional` **reportSkipColumnHeader**: ``null`` \| [*False*](./enums/reportdefinitionservicereportskipcolumnheader.md#false) \| [*True*](./enums/reportdefinitionservicereportskipcolumnheader.md#true) \| [*Unknown*](./enums/reportdefinitionservicereportskipcolumnheader.md#unknown)

**`memberof`** ReportDefinition

___

### reportSkipReportSummary

• `Optional` **reportSkipReportSummary**: ``null`` \| [*False*](./enums/reportdefinitionservicereportskipreportsummary.md#false) \| [*True*](./enums/reportdefinitionservicereportskipreportsummary.md#true) \| [*Unknown*](./enums/reportdefinitionservicereportskipreportsummary.md#unknown)

**`memberof`** ReportDefinition

___

### reportTypeCondition

• `Optional` **reportTypeCondition**: ``null`` \| [*ReportDefinitionServiceReportTypeCondition*](reportdefinitionservicereporttypecondition.md)

**`memberof`** ReportDefinition

___

### requestTime

• `Optional` **requestTime**: ``null`` \| *string*

<div lang=\"ja\"> ジョブ依頼日時です。<br> このフィールドは、レスポンスの際に返却されますが、リクエストの際には無視されます。 </div> 

**`memberof`** ReportDefinition

___

### sortFields

• `Optional` **sortFields**: ``null`` \| [*ReportDefinitionServiceReportSortField*](reportdefinitionservicereportsortfield.md)[]

**`memberof`** ReportDefinition
