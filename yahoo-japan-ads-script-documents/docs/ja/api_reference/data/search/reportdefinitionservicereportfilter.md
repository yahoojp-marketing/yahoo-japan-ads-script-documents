# ReportDefinitionServiceReportFilter


<div lang=\"ja\">ReportDefinitionServiceReportFilterオブジェクトは、レポートのフィルタ条件を表します。フィルタ条件は最大6つまで設定が可能です。<br> ADD時、このフィールドは省略可能となります。 </div> 

## Table of contents

### Properties

- [field](reportdefinitionservicereportfilter.md#field)
- [filterOperator](reportdefinitionservicereportfilter.md#filteroperator)
- [values](reportdefinitionservicereportfilter.md#values)

## Properties

### field

• `Optional` **field**: ``null`` \| *string*

<div lang=\"ja\">フィルタ条件を設定する表示項目です。<br> ADD時、このフィールドは必須となります。 </div> 

**`memberof`** ReportDefinitionServiceReportFilter

___

### filterOperator

• `Optional` **filterOperator**: ``null`` \| [*Equals*](./enums/reportdefinitionservicefilteroperator.md#equals) \| [*NotEquals*](./enums/reportdefinitionservicefilteroperator.md#notequals) \| [*GreaterThan*](./enums/reportdefinitionservicefilteroperator.md#greaterthan) \| [*GreaterThanEquals*](./enums/reportdefinitionservicefilteroperator.md#greaterthanequals) \| [*LessThan*](./enums/reportdefinitionservicefilteroperator.md#lessthan) \| [*LessThanEquals*](./enums/reportdefinitionservicefilteroperator.md#lessthanequals) \| [*Contains*](./enums/reportdefinitionservicefilteroperator.md#contains) \| [*In*](./enums/reportdefinitionservicefilteroperator.md#in) \| [*Unknown*](./enums/reportdefinitionservicefilteroperator.md#unknown)

**`memberof`** ReportDefinitionServiceReportFilter

___

### values

• `Optional` **values**: ``null`` \| *string*[]

<div lang=\"ja\">表示項目の条件値です。<br> ADD時、このフィールドは必須となります。</div> 

**`memberof`** ReportDefinitionServiceReportFilter
