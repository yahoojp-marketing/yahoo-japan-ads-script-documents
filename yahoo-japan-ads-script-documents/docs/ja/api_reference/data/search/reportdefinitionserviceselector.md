# ReportDefinitionServiceSelector


<div lang=\"ja\">ReportDefinitionServiceSelectorオブジェクトは、操作の対象とするレポートです。</div> 

## Table of contents

### Properties

- [accountId](reportdefinitionserviceselector.md#accountid)
- [numberResults](reportdefinitionserviceselector.md#numberresults)
- [reportJobIds](reportdefinitionserviceselector.md#reportjobids)
- [reportJobStatuses](reportdefinitionserviceselector.md#reportjobstatuses)
- [reportTypes](reportdefinitionserviceselector.md#reporttypes)
- [startIndex](reportdefinitionserviceselector.md#startindex)

## Properties

### accountId

• **accountId**: *number*

<div lang=\"ja\">検索条件： アカウントIDです。</div> 

**`memberof`** ReportDefinitionServiceSelector

___

### numberResults

• `Optional` **numberResults**: ``null`` \| *number*

<div lang=\"ja\">ページの最大件数です。このフィールドは、1以上を指定する必要があります。</div> 

**`memberof`** ReportDefinitionServiceSelector

___

### reportJobIds

• `Optional` **reportJobIds**: ``null`` \| *number*[]

<div lang=\"ja\">検索条件： レポートジョブIDです。</div> 

**`memberof`** ReportDefinitionServiceSelector

___

### reportJobStatuses

• `Optional` **reportJobStatuses**: ``null`` \| [*ReportDefinitionServiceReportJobStatus*](./enums/reportdefinitionservicereportjobstatus.md)[]

**`memberof`** ReportDefinitionServiceSelector

___

### reportTypes

• `Optional` **reportTypes**: ``null`` \| [*ReportDefinitionServiceReportType*](./enums/reportdefinitionservicereporttype.md)[]

**`memberof`** ReportDefinitionServiceSelector

___

### startIndex

• `Optional` **startIndex**: ``null`` \| *number*

<div lang=\"ja\">ページの先頭のインデックスです。このフィールドは、1以上を指定する必要があります。</div> 

**`memberof`** ReportDefinitionServiceSelector
