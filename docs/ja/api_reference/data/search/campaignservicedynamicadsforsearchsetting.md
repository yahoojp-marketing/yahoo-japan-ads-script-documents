# CampaignServiceDynamicAdsForSearchSetting


<div lang=\"ja\">   CampaignServiceDynamicAdsForSearchSettingは、動的検索連動型広告に関する検索条件を表します。<br>   ADD時、settingTypeがDYNAMIC_ADS_FOR_SEARCH_SETTINGの場合、必須となり、それ以外では省略可能となります。 </div> 

## Table of contents

### Properties

- [dasUseUrlsType](campaignservicedynamicadsforsearchsetting.md#dasuseurlstype)
- [domain](campaignservicedynamicadsforsearchsetting.md#domain)
- [feedIds](campaignservicedynamicadsforsearchsetting.md#feedids)

## Properties

### dasUseUrlsType

• `Optional` **dasUseUrlsType**: ``null`` \| [*UseSuppliedUrlsOnly*](./enums/campaignservicedasuseurlstype.md#usesuppliedurlsonly) \| [*TopDomainOnly*](./enums/campaignservicedasuseurlstype.md#topdomainonly) \| [*DomainAndSuppliedUrls*](./enums/campaignservicedasuseurlstype.md#domainandsuppliedurls) \| [*Unknown*](./enums/campaignservicedasuseurlstype.md#unknown)

**`memberof`** CampaignServiceDynamicAdsForSearchSetting

___

### domain

• `Optional` **domain**: ``null`` \| *string*

<div lang=\"ja\">   ドメインです。<br>   ADDおよびSET時、DasUseUrlsTypeがTOP_DOMAIN_ONLYまたはDOMAIN_AND_SUPPLIED_URLSの場合、このフィールドは必須となります。 </div> 

**`memberof`** CampaignServiceDynamicAdsForSearchSetting

___

### feedIds

• `Optional` **feedIds**: ``null`` \| *number*[]

<div lang=\"ja\">   キャンペーンで使用するページフィードIDです。<br>   ADD時およびSET時、DasUseUrlsTypeがUSE_SUPPLIED_URLS_ONLYまたはDOMAIN_AND_SUPPLIED_URLSの場合、このフィールドは必須となります。 </div> 

**`memberof`** CampaignServiceDynamicAdsForSearchSetting
