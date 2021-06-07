# AdGroupWebpageServiceWebpageCondition


<div lang=\"ja\">AdGroupWebpageServiceWebpageConditionオブジェクトは、Webpageの条件を保持します。<br> このフィールドは、ADD時は必須となり、SET時は無視されます。</div> 

## Table of contents

### Properties

- [argument](adgroupwebpageservicewebpagecondition.md#argument)
- [operator](adgroupwebpageservicewebpagecondition.md#operator)
- [webpageConditionType](adgroupwebpageservicewebpagecondition.md#webpageconditiontype)

## Properties

### argument

• `Optional` **argument**: ``null`` \| *string*

<div lang=\"ja\">条件の設定値(正規表現の指定可)です。<br>ADD時、このフィールドは必須です。※typeがALL_PAGESの場合は省略可能となります。SET時、このフィールドは無視されます。</div> 

**`memberof`** AdGroupWebpageServiceWebpageCondition

___

### operator

• `Optional` **operator**: ``null`` \| [*Contains*](./enums/adgroupwebpageserviceoperator.md#contains) \| [*Equals*](./enums/adgroupwebpageserviceoperator.md#equals) \| [*Unknown*](./enums/adgroupwebpageserviceoperator.md#unknown)

**`memberof`** AdGroupWebpageServiceWebpageCondition

___

### webpageConditionType

• `Optional` **webpageConditionType**: ``null`` \| [*Url*](./enums/adgroupwebpageservicewebpageconditiontype.md#url) \| [*PageTitle*](./enums/adgroupwebpageservicewebpageconditiontype.md#pagetitle) \| [*PageContent*](./enums/adgroupwebpageservicewebpageconditiontype.md#pagecontent) \| [*CustomLabel*](./enums/adgroupwebpageservicewebpageconditiontype.md#customlabel) \| [*AllPages*](./enums/adgroupwebpageservicewebpageconditiontype.md#allpages) \| [*Unknown*](./enums/adgroupwebpageservicewebpageconditiontype.md#unknown)

**`memberof`** AdGroupWebpageServiceWebpageCondition
