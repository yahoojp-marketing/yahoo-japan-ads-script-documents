# ReportDefinitionServiceFilter


<div lang=\"ja\"> ReportDefinitionServiceFilterオブジェクトは、フィルター定義を表します。<br> フィルタ条件は最大6つまで設定が可能です。<br> このフィールドは、ADD時に省略可能となり、REMOVE時に無視されます。 </div> 

## Table of contents

### Properties

- [field](reportdefinitionservicefilter.md#field)
- [filterOperator](reportdefinitionservicefilter.md#filteroperator)
- [values](reportdefinitionservicefilter.md#values)

## Properties

### field

• `Optional` **field**: ``null`` \| *string*

<div lang=\"ja\"> フィルター対象となるフィールドです。<br> このフィールドは、ADD時に必須となります。<br> ※getReportFieldsのレスポンスで「filterable=true」のフィールドのみ指定可能です。 </div> 

**`memberof`** ReportDefinitionServiceFilter

___

### filterOperator

• `Optional` **filterOperator**: ``null`` \| [*Equals*](./enums/reportdefinitionservicefilteroperator.md#equals) \| [*NotEquals*](./enums/reportdefinitionservicefilteroperator.md#notequals) \| [*GreaterThan*](./enums/reportdefinitionservicefilteroperator.md#greaterthan) \| [*GreaterThanEquals*](./enums/reportdefinitionservicefilteroperator.md#greaterthanequals) \| [*LessThan*](./enums/reportdefinitionservicefilteroperator.md#lessthan) \| [*LessThanEquals*](./enums/reportdefinitionservicefilteroperator.md#lessthanequals) \| [*Contains*](./enums/reportdefinitionservicefilteroperator.md#contains) \| [*In*](./enums/reportdefinitionservicefilteroperator.md#in) \| [*ContainsAll*](./enums/reportdefinitionservicefilteroperator.md#containsall) \| [*ContainsAny*](./enums/reportdefinitionservicefilteroperator.md#containsany) \| [*Unknown*](./enums/reportdefinitionservicefilteroperator.md#unknown)

**`memberof`** ReportDefinitionServiceFilter

___

### values

• `Optional` **values**: ``null`` \| *string*[]

<div lang=\"ja\"> 条件値です。<br> このフィールドは、ADD時に必須となります。 </div> 

**`memberof`** ReportDefinitionServiceFilter
