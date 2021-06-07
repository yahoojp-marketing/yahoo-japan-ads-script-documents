# ReportDefinitionServiceConversionPathFilter


<div lang=\"ja\">   ReportDefinitionServiceConversionPathFilterオブジェクトは、コンバージョン経路レポートのフィルタ条件を表します。<br>   複数指定した場合、AND条件になります。<br>   このフィールドは、ADD時に省略可能となり、REMOVE時に無視されます。 </div> 

## Table of contents

### Properties

- [conversionPathFilterOperator](reportdefinitionserviceconversionpathfilter.md#conversionpathfilteroperator)
- [conversionPathFilterType](reportdefinitionserviceconversionpathfilter.md#conversionpathfiltertype)
- [values](reportdefinitionserviceconversionpathfilter.md#values)

## Properties

### conversionPathFilterOperator

• `Optional` **conversionPathFilterOperator**: ``null`` \| [*Equals*](./enums/reportdefinitionserviceconversionpathfilteroperator.md#equals) \| [*NotEquals*](./enums/reportdefinitionserviceconversionpathfilteroperator.md#notequals) \| [*Contains*](./enums/reportdefinitionserviceconversionpathfilteroperator.md#contains) \| [*NotContains*](./enums/reportdefinitionserviceconversionpathfilteroperator.md#notcontains) \| [*StartWith*](./enums/reportdefinitionserviceconversionpathfilteroperator.md#startwith) \| [*EndWith*](./enums/reportdefinitionserviceconversionpathfilteroperator.md#endwith) \| [*Unknown*](./enums/reportdefinitionserviceconversionpathfilteroperator.md#unknown)

**`memberof`** ReportDefinitionServiceConversionPathFilter

___

### conversionPathFilterType

• `Optional` **conversionPathFilterType**: ``null`` \| [*CampaignId*](./enums/reportdefinitionserviceconversionpathfiltertype.md#campaignid) \| [*CampaignName*](./enums/reportdefinitionserviceconversionpathfiltertype.md#campaignname) \| [*ConversionId*](./enums/reportdefinitionserviceconversionpathfiltertype.md#conversionid) \| [*Unknown*](./enums/reportdefinitionserviceconversionpathfiltertype.md#unknown)

**`memberof`** ReportDefinitionServiceConversionPathFilter

___

### values

• `Optional` **values**: ``null`` \| *string*[]

<div lang=\"ja\">条件値です。複数指定した場合は、OR条件になります。</div> 

**`memberof`** ReportDefinitionServiceConversionPathFilter
