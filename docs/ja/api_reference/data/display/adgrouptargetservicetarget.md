# AdGroupTargetServiceTarget


<div lang=\"ja\"> AdGroupTargetServiceTargetオブジェクトは、ターゲティング設定情報を保持します。<br> このフィールドは、リクエストの場合は必須です。 </div> 

## Table of contents

### Properties

- [adScheduleTarget](adgrouptargetservicetarget.md#adscheduletarget)
- [ageTarget](adgrouptargetservicetarget.md#agetarget)
- [appTarget](adgrouptargetservicetarget.md#apptarget)
- [audienceCategoryTarget](adgrouptargetservicetarget.md#audiencecategorytarget)
- [contentsTarget](adgrouptargetservicetarget.md#contentstarget)
- [deviceTarget](adgrouptargetservicetarget.md#devicetarget)
- [genderTarget](adgrouptargetservicetarget.md#gendertarget)
- [geoTarget](adgrouptargetservicetarget.md#geotarget)
- [isRemove](adgrouptargetservicetarget.md#isremove)
- [osTarget](adgrouptargetservicetarget.md#ostarget)
- [osVersionTarget](adgrouptargetservicetarget.md#osversiontarget)
- [placementCategoryDetailTarget](adgrouptargetservicetarget.md#placementcategorydetailtarget)
- [placementCategoryTarget](adgrouptargetservicetarget.md#placementcategorytarget)
- [placementTarget](adgrouptargetservicetarget.md#placementtarget)
- [positionTarget](adgrouptargetservicetarget.md#positiontarget)
- [searchTarget](adgrouptargetservicetarget.md#searchtarget)
- [siteCategoryTarget](adgrouptargetservicetarget.md#sitecategorytarget)
- [siteRetargetingTarget](adgrouptargetservicetarget.md#siteretargetingtarget)
- [targetId](adgrouptargetservicetarget.md#targetid)
- [targetType](adgrouptargetservicetarget.md#targettype)

## Properties

### adScheduleTarget

• `Optional` **adScheduleTarget**: ``null`` \| [*AdGroupTargetServiceAdScheduleTarget*](adgrouptargetserviceadscheduletarget.md)

**`memberof`** AdGroupTargetServiceTarget

___

### ageTarget

• `Optional` **ageTarget**: ``null`` \| [*AdGroupTargetServiceAgeTarget*](adgrouptargetserviceagetarget.md)

**`memberof`** AdGroupTargetServiceTarget

___

### appTarget

• `Optional` **appTarget**: ``null`` \| [*AdGroupTargetServiceAppTarget*](adgrouptargetserviceapptarget.md)

**`memberof`** AdGroupTargetServiceTarget

___

### audienceCategoryTarget

• `Optional` **audienceCategoryTarget**: ``null`` \| [*AdGroupTargetServiceAudienceCategoryTarget*](adgrouptargetserviceaudiencecategorytarget.md)

**`memberof`** AdGroupTargetServiceTarget

___

### contentsTarget

• `Optional` **contentsTarget**: ``null`` \| [*AdGroupTargetServiceContentsTarget*](adgrouptargetservicecontentstarget.md)

**`memberof`** AdGroupTargetServiceTarget

___

### deviceTarget

• `Optional` **deviceTarget**: ``null`` \| [*AdGroupTargetServiceDeviceTarget*](adgrouptargetservicedevicetarget.md)

**`memberof`** AdGroupTargetServiceTarget

___

### genderTarget

• `Optional` **genderTarget**: ``null`` \| [*AdGroupTargetServiceGenderTarget*](adgrouptargetservicegendertarget.md)

**`memberof`** AdGroupTargetServiceTarget

___

### geoTarget

• `Optional` **geoTarget**: ``null`` \| [*AdGroupTargetServiceGeoTarget*](adgrouptargetservicegeotarget.md)

**`memberof`** AdGroupTargetServiceTarget

___

### isRemove

• `Optional` **isRemove**: ``null`` \| *boolean*

<div lang=\"ja\"> trueの場合、ターゲティング種別をすべて削除します。<br> このフィールドは、ADD、SETおよびREMOVE時は無視され、REPLACE時は省略可能となります。 </div> 

**`memberof`** AdGroupTargetServiceTarget

___

### osTarget

• `Optional` **osTarget**: ``null`` \| [*AdGroupTargetServiceOsTarget*](adgrouptargetserviceostarget.md)

**`memberof`** AdGroupTargetServiceTarget

___

### osVersionTarget

• `Optional` **osVersionTarget**: ``null`` \| [*AdGroupTargetServiceOsVersionTarget*](adgrouptargetserviceosversiontarget.md)

**`memberof`** AdGroupTargetServiceTarget

___

### placementCategoryDetailTarget

• `Optional` **placementCategoryDetailTarget**: ``null`` \| [*AdGroupTargetServicePlacementCategoryDetailTarget*](adgrouptargetserviceplacementcategorydetailtarget.md)

**`memberof`** AdGroupTargetServiceTarget

___

### placementCategoryTarget

• `Optional` **placementCategoryTarget**: ``null`` \| [*AdGroupTargetServicePlacementCategoryTarget*](adgrouptargetserviceplacementcategorytarget.md)

**`memberof`** AdGroupTargetServiceTarget

___

### placementTarget

• `Optional` **placementTarget**: ``null`` \| [*AdGroupTargetServicePlacementTarget*](adgrouptargetserviceplacementtarget.md)

**`memberof`** AdGroupTargetServiceTarget

___

### positionTarget

• `Optional` **positionTarget**: ``null`` \| [*AdGroupTargetServicePositionTarget*](adgrouptargetservicepositiontarget.md)

**`memberof`** AdGroupTargetServiceTarget

___

### searchTarget

• `Optional` **searchTarget**: ``null`` \| [*AdGroupTargetServiceSearchTarget*](adgrouptargetservicesearchtarget.md)

**`memberof`** AdGroupTargetServiceTarget

___

### siteCategoryTarget

• `Optional` **siteCategoryTarget**: ``null`` \| [*AdGroupTargetServiceSiteCategoryTarget*](adgrouptargetservicesitecategorytarget.md)

**`memberof`** AdGroupTargetServiceTarget

___

### siteRetargetingTarget

• `Optional` **siteRetargetingTarget**: ``null`` \| [*AdGroupTargetServiceSiteRetargetingTarget*](adgrouptargetservicesiteretargetingtarget.md)

**`memberof`** AdGroupTargetServiceTarget

___

### targetId

• `Optional` **targetId**: ``null`` \| *string*

<div lang=\"ja\"> ターゲットIDです。<br> このフィールドは、ADDおよびREPLACE時は省略可能となり、SETおよびREMOVE時は必須となります。<br> ※ADD時、targetTypeが以下のいずれかの場合は必須です。<br> ‐SITE_RETARGETING<br> ‐PLACEMENT_TARGET<br> ‐SEARCH_TARGET<br> ‐GEO_TARGET<br> ‐SITE_CATEGORY<br> ‐AUDIENCE_CATEGORY_TARGET<br> ‐PLACEMENT_CATEGORY_TARGET<br> -PLACEMENT_CATEGORY_DETAIL_TARGET<br> -CONTENTS_TARGET<br> ※REPLACE時、isRemoveがtrueの場合は設定不要です。<br> <br> ‐SITE_RETARGETING: targetListId<br> ‐PLACEMENT_TARGET: placementUrlListId<br> ‐SEARCH_TARGET: searchKeywordListId<br> ‐GEO_TARGET: IM地域コード(geo)<br> ‐SITE_CATEGORY: カテゴリーコード(category)<br> ‐OS_VERSION_TARGET: osVersion<br> ‐AUDIENCE_CATEGORY_TARGET: オーディエンスカテゴリーコード(audience category)<br> ‐POSITION_TARGET: PositionTypeのコード値<br> ‐PLACEMENT_CATEGORY_TARGET: placementCategoryListId<br> -PLACEMENT_CATEGORY_DETAIL_TARGET: placementCategoryId<br> -CONTENTS_TARGET: contentsKeywordListId </div> 

**`memberof`** AdGroupTargetServiceTarget

___

### targetType

• `Optional` **targetType**: ``null`` \| [*AdScheduleTarget*](./enums/adgrouptargetservicetargettype.md#adscheduletarget) \| [*GeoTarget*](./enums/adgrouptargetservicetargettype.md#geotarget) \| [*AgeTarget*](./enums/adgrouptargetservicetargettype.md#agetarget) \| [*GenderTarget*](./enums/adgrouptargetservicetargettype.md#gendertarget) \| [*SiteCategory*](./enums/adgrouptargetservicetargettype.md#sitecategory) \| [*SiteRetargeting*](./enums/adgrouptargetservicetargettype.md#siteretargeting) \| [*SearchTarget*](./enums/adgrouptargetservicetargettype.md#searchtarget) \| [*PlacementTarget*](./enums/adgrouptargetservicetargettype.md#placementtarget) \| [*DeviceTarget*](./enums/adgrouptargetservicetargettype.md#devicetarget) \| [*AppTarget*](./enums/adgrouptargetservicetargettype.md#apptarget) \| [*OsTarget*](./enums/adgrouptargetservicetargettype.md#ostarget) \| [*OsVersionTarget*](./enums/adgrouptargetservicetargettype.md#osversiontarget) \| [*AudienceCategoryTarget*](./enums/adgrouptargetservicetargettype.md#audiencecategorytarget) \| [*PositionTarget*](./enums/adgrouptargetservicetargettype.md#positiontarget) \| [*PlacementCategoryTarget*](./enums/adgrouptargetservicetargettype.md#placementcategorytarget) \| [*PlacementCategoryDetailTarget*](./enums/adgrouptargetservicetargettype.md#placementcategorydetailtarget) \| [*ContentsTarget*](./enums/adgrouptargetservicetargettype.md#contentstarget) \| [*Unknown*](./enums/adgrouptargetservicetargettype.md#unknown)

**`memberof`** AdGroupTargetServiceTarget
