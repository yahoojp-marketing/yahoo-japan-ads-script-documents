# ReportDefinitionServiceConversionPathReportCondition


<div lang=\"ja\">   ReportDefinitionServiceConversionPathReportConditionオブジェクトは、コンバージョン経路レポートの作成条件を表します。<br>   このフィールドは、ADD時に省略可能となり、REMOVE時に無視されます。<br>   ※ADD時、reportTypeが<code>CONVERSION_PATH</code>の場合は必須です。 </div> 

## Table of contents

### Properties

- [conversionPathAccountSetting](reportdefinitionserviceconversionpathreportcondition.md#conversionpathaccountsetting)
- [conversionPathFilters](reportdefinitionserviceconversionpathreportcondition.md#conversionpathfilters)
- [includeViewInteraction](reportdefinitionserviceconversionpathreportcondition.md#includeviewinteraction)
- [lookbackWindow](reportdefinitionserviceconversionpathreportcondition.md#lookbackwindow)

## Properties

### conversionPathAccountSetting

• `Optional` **conversionPathAccountSetting**: ``null`` \| [*ReportDefinitionServiceConversionPathAccountSetting*](reportdefinitionserviceconversionpathaccountsetting.md)

**`memberof`** ReportDefinitionServiceConversionPathReportCondition

___

### conversionPathFilters

• `Optional` **conversionPathFilters**: ``null`` \| [*ReportDefinitionServiceConversionPathFilter*](reportdefinitionserviceconversionpathfilter.md)[]

**`memberof`** ReportDefinitionServiceConversionPathReportCondition

___

### includeViewInteraction

• `Optional` **includeViewInteraction**: ``null`` \| [*True*](./enums/reportdefinitionserviceincludeviewinteractionflg.md#true) \| [*False*](./enums/reportdefinitionserviceincludeviewinteractionflg.md#false) \| [*Unknown*](./enums/reportdefinitionserviceincludeviewinteractionflg.md#unknown)

**`memberof`** ReportDefinitionServiceConversionPathReportCondition

___

### lookbackWindow

• `Optional` **lookbackWindow**: ``null`` \| *number*

<div lang=\"ja\">   ルックバック期間（日数）です。<br>   指定できる値の下限は0、上限は90です。<br>   このフィールドは、ADDに必須となります。 </div> 

**`memberof`** ReportDefinitionServiceConversionPathReportCondition
