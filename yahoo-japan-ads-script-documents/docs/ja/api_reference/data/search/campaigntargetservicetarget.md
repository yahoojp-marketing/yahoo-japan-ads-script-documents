# CampaignTargetServiceTarget


<div lang=\"ja\">CampaignTargetServiceTargetオブジェクトは、ターゲティング設定を表します。<br> このフィールドは、いずれの場合でも必須となります。</div> 

## Table of contents

### Properties

- [locationTarget](campaigntargetservicetarget.md#locationtarget)
- [networkTarget](campaigntargetservicetarget.md#networktarget)
- [platformTarget](campaigntargetservicetarget.md#platformtarget)
- [scheduleTarget](campaigntargetservicetarget.md#scheduletarget)
- [targetId](campaigntargetservicetarget.md#targetid)
- [targetType](campaigntargetservicetarget.md#targettype)

## Properties

### locationTarget

• `Optional` **locationTarget**: ``null`` \| [*CampaignTargetServiceLocationTarget*](campaigntargetservicelocationtarget.md)

**`memberof`** CampaignTargetServiceTarget

___

### networkTarget

• `Optional` **networkTarget**: ``null`` \| [*CampaignTargetServiceNetworkTarget*](campaigntargetservicenetworktarget.md)

**`memberof`** CampaignTargetServiceTarget

___

### platformTarget

• `Optional` **platformTarget**: ``null`` \| [*CampaignTargetServicePlatformTarget*](campaigntargetserviceplatformtarget.md)

**`memberof`** CampaignTargetServiceTarget

___

### scheduleTarget

• `Optional` **scheduleTarget**: ``null`` \| [*CampaignTargetServiceScheduleTarget*](campaigntargetservicescheduletarget.md)

**`memberof`** CampaignTargetServiceTarget

___

### targetId

• `Optional` **targetId**: ``null`` \| *string*

<div lang=\"ja\">ターゲットIDです。<br> このフィールドは、ADD時は無視され、SETおよびREMOVE時は必須となります。<br> ※LocationCampaignTargetServiceTargetの場合、ADD時に必須となります。<br> ※PlatformCampaignTargetServiceTargetの場合、SET時に無視されます。</div> 

**`memberof`** CampaignTargetServiceTarget

___

### targetType

• `Optional` **targetType**: ``null`` \| [*Location*](./enums/campaigntargetservicetargettype.md#location) \| [*Schedule*](./enums/campaigntargetservicetargettype.md#schedule) \| [*Network*](./enums/campaigntargetservicetargettype.md#network) \| [*Platform*](./enums/campaigntargetservicetargettype.md#platform) \| [*Unknown*](./enums/campaigntargetservicetargettype.md#unknown)

**`memberof`** CampaignTargetServiceTarget
