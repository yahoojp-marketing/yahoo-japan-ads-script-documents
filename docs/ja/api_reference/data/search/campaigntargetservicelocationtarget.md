# CampaignTargetServiceLocationTarget


<div lang=\"ja\">CampaignTargetServiceLocationTargetオブジェクトは、地域ターゲティング設定です。<br> このフィールドは、ADDおよびSET時に省略可能となります。<br> ※targetTypeがLOCATIONの場合、このフィールドはADD時に必須となります。</div> 

## Table of contents

### Properties

- [cityNameEN](campaigntargetservicelocationtarget.md#citynameen)
- [cityNameJA](campaigntargetservicelocationtarget.md#citynameja)
- [excludedType](campaigntargetservicelocationtarget.md#excludedtype)
- [provinceNameEN](campaigntargetservicelocationtarget.md#provincenameen)
- [provinceNameJA](campaigntargetservicelocationtarget.md#provincenameja)
- [targetingStatus](campaigntargetservicelocationtarget.md#targetingstatus)

## Properties

### cityNameEN

• `Optional` **cityNameEN**: ``null`` \| *string*

<div lang=\"ja\">市区町村名（英語）です。<br> このフィールドは、レスポンスの際に返却されますが、リクエストの際には無視されます。</div> 

**`memberof`** CampaignTargetServiceLocationTarget

___

### cityNameJA

• `Optional` **cityNameJA**: ``null`` \| *string*

<div lang=\"ja\">市区町村名（日本語）です。<br> このフィールドは、レスポンスの際に返却されますが、リクエストの際には無視されます。</div> 

**`memberof`** CampaignTargetServiceLocationTarget

___

### excludedType

• `Optional` **excludedType**: ``null`` \| [*Included*](./enums/campaigntargetserviceexcludedtype.md#included) \| [*Excluded*](./enums/campaigntargetserviceexcludedtype.md#excluded) \| [*Unknown*](./enums/campaigntargetserviceexcludedtype.md#unknown)

**`memberof`** CampaignTargetServiceLocationTarget

___

### provinceNameEN

• `Optional` **provinceNameEN**: ``null`` \| *string*

<div lang=\"ja\">都道府県名（英語）です。<br> このフィールドは、レスポンスの際に返却されますが、リクエストの際には無視されます。</div> 

**`memberof`** CampaignTargetServiceLocationTarget

___

### provinceNameJA

• `Optional` **provinceNameJA**: ``null`` \| *string*

<div lang=\"ja\">都道府県名（日本語）です。<br> このフィールドは、レスポンスの際に返却されますが、リクエストの際には無視されます。</div> 

**`memberof`** CampaignTargetServiceLocationTarget

___

### targetingStatus

• `Optional` **targetingStatus**: ``null`` \| [*Active*](./enums/campaigntargetservicetargetingstatus.md#active) \| [*Obsolete*](./enums/campaigntargetservicetargetingstatus.md#obsolete) \| [*PhasingOut*](./enums/campaigntargetservicetargetingstatus.md#phasingout) \| [*Unknown*](./enums/campaigntargetservicetargetingstatus.md#unknown)

**`memberof`** CampaignTargetServiceLocationTarget
