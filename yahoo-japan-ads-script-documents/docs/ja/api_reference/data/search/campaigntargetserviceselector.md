# CampaignTargetServiceSelector


<div lang=\"ja\">CampaignTargetServiceSelectorオブジェクトは、操作の対象とするキャンペーンのターゲティング設定を表します。</div> 

## Table of contents

### Properties

- [accountId](campaigntargetserviceselector.md#accountid)
- [campaignIds](campaigntargetserviceselector.md#campaignids)
- [excludedType](campaigntargetserviceselector.md#excludedtype)
- [numberResults](campaigntargetserviceselector.md#numberresults)
- [platformTypes](campaigntargetserviceselector.md#platformtypes)
- [startIndex](campaigntargetserviceselector.md#startindex)
- [targetIds](campaigntargetserviceselector.md#targetids)
- [targetTypes](campaigntargetserviceselector.md#targettypes)

## Properties

### accountId

• **accountId**: *number*

<div lang=\"ja\">アカウントIDです。</div> 

**`memberof`** CampaignTargetServiceSelector

___

### campaignIds

• `Optional` **campaignIds**: ``null`` \| *number*[]

<div lang=\"ja\">キャンペーンIDです。</div> 

**`memberof`** CampaignTargetServiceSelector

___

### excludedType

• `Optional` **excludedType**: ``null`` \| [*Included*](./enums/campaigntargetserviceexcludedtype.md#included) \| [*Excluded*](./enums/campaigntargetserviceexcludedtype.md#excluded) \| [*Unknown*](./enums/campaigntargetserviceexcludedtype.md#unknown)

**`memberof`** CampaignTargetServiceSelector

___

### numberResults

• `Optional` **numberResults**: ``null`` \| *number*

<div lang=\"ja\">ページの最大件数です。このフィールドは、1以上を指定する必要があります。</div> 

**`memberof`** CampaignTargetServiceSelector

___

### platformTypes

• `Optional` **platformTypes**: ``null`` \| [*CampaignTargetServicePlatformType*](./enums/campaigntargetserviceplatformtype.md)[]

**`memberof`** CampaignTargetServiceSelector

___

### startIndex

• `Optional` **startIndex**: ``null`` \| *number*

<div lang=\"ja\">ページの先頭のインデックスです。このフィールドは、1以上を指定する必要があります。</div> 

**`memberof`** CampaignTargetServiceSelector

___

### targetIds

• `Optional` **targetIds**: ``null`` \| *string*[]

<div lang=\"ja\">ターゲットIDです。</div> 

**`memberof`** CampaignTargetServiceSelector

___

### targetTypes

• `Optional` **targetTypes**: ``null`` \| [*CampaignTargetServiceTargetType*](./enums/campaigntargetservicetargettype.md)[]

**`memberof`** CampaignTargetServiceSelector
