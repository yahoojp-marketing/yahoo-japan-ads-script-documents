# CampaignServiceSettings


<div lang=\"ja\">CampaignServiceSettingsオブジェクトは、キャンペーンの地域ターゲットを格納するコンテナです。<br> ADD時、このフィールドは、campaignTypeがDYNAMIC_ADS_FOR_SEARCH_SETTINGの場合、必須となり、それ以外では省略可能となります。また、TargetingSettingが未設定の場合、デフォルト設定値は[SettingType:TARGET_LIST_SETTING, TargetAll:ACTIVE]となります。</div> 

## Table of contents

### Properties

- [dynamicAdsForSearchSetting](campaignservicesettings.md#dynamicadsforsearchsetting)
- [geoTargetTypeSetting](campaignservicesettings.md#geotargettypesetting)
- [settingType](campaignservicesettings.md#settingtype)
- [targetingSetting](campaignservicesettings.md#targetingsetting)

## Properties

### dynamicAdsForSearchSetting

• `Optional` **dynamicAdsForSearchSetting**: ``null`` \| [*CampaignServiceDynamicAdsForSearchSetting*](campaignservicedynamicadsforsearchsetting.md)

**`memberof`** CampaignServiceSettings

___

### geoTargetTypeSetting

• `Optional` **geoTargetTypeSetting**: ``null`` \| [*CampaignServiceGeoTargetTypeSetting*](campaignservicegeotargettypesetting.md)

**`memberof`** CampaignServiceSettings

___

### settingType

• `Optional` **settingType**: ``null`` \| [*GeoTargetTypeSetting*](./enums/campaignservicesettingtype.md#geotargettypesetting) \| [*TargetListSetting*](./enums/campaignservicesettingtype.md#targetlistsetting) \| [*DynamicAdsForSearchSetting*](./enums/campaignservicesettingtype.md#dynamicadsforsearchsetting) \| [*Unknown*](./enums/campaignservicesettingtype.md#unknown)

**`memberof`** CampaignServiceSettings

___

### targetingSetting

• `Optional` **targetingSetting**: ``null`` \| [*CampaignServiceTargetingSetting*](campaignservicetargetingsetting.md)

**`memberof`** CampaignServiceSettings
