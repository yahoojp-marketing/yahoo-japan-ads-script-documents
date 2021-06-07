# CampaignWebpageServiceWebpageCondition


<div lang=\"ja\">CampaignWebpageServiceWebpageConditionオブジェクトは、Webpageの条件を保持します。<br> このフィールドは、ADD時に必須となり、REMOVE時に無視されます。</div> 

## Table of contents

### Properties

- [argument](campaignwebpageservicewebpagecondition.md#argument)
- [operator](campaignwebpageservicewebpagecondition.md#operator)
- [type](campaignwebpageservicewebpagecondition.md#type)

## Properties

### argument

• `Optional` **argument**: ``null`` \| *string*

<div lang=\"ja\">条件の設定値(正規表現の指定可)です。<br> このフィールドは、ADD時に必須となり、REMOVE時に無視されます。</div> 

**`memberof`** CampaignWebpageServiceWebpageCondition

___

### operator

• `Optional` **operator**: ``null`` \| [*Contains*](./enums/campaignwebpageservicewebpageoperator.md#contains) \| [*Equals*](./enums/campaignwebpageservicewebpageoperator.md#equals) \| [*Unknown*](./enums/campaignwebpageservicewebpageoperator.md#unknown)

**`memberof`** CampaignWebpageServiceWebpageCondition

___

### type

• `Optional` **type**: ``null`` \| [*Url*](./enums/campaignwebpageservicewebpageconditiontype.md#url) \| [*PageTitle*](./enums/campaignwebpageservicewebpageconditiontype.md#pagetitle) \| [*PageContent*](./enums/campaignwebpageservicewebpageconditiontype.md#pagecontent) \| [*CustomLabel*](./enums/campaignwebpageservicewebpageconditiontype.md#customlabel) \| [*AllPages*](./enums/campaignwebpageservicewebpageconditiontype.md#allpages) \| [*Unknown*](./enums/campaignwebpageservicewebpageconditiontype.md#unknown)

**`memberof`** CampaignWebpageServiceWebpageCondition
