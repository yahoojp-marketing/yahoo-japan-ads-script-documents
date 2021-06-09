# GuaranteedInventoryServiceAdRequirement


<div lang=\"ja\"> GuaranteedInventoryServiceAdRequirementオブジェクトは、予約型の広告を構成する条件を表します。<br> ADD時、このフィールドは必須となります。 </div> 

## Table of contents

### Properties

- [adType](guaranteedinventoryserviceadrequirement.md#adtype)
- [aspectRatio](guaranteedinventoryserviceadrequirement.md#aspectratio)
- [mediaAdFormat](guaranteedinventoryserviceadrequirement.md#mediaadformat)

## Properties

### adType

• `Optional` **adType**: ``null`` \| [*BannerVideoAd*](./enums/guaranteedinventoryserviceadtype.md#bannervideoad) \| [*BannerImageAd*](./enums/guaranteedinventoryserviceadtype.md#bannerimagead) \| [*BrandpanelQuintie*](./enums/guaranteedinventoryserviceadtype.md#brandpanelquintie) \| [*BrandpanelQuintieVideo*](./enums/guaranteedinventoryserviceadtype.md#brandpanelquintievideo) \| [*BrandpanelPanorama*](./enums/guaranteedinventoryserviceadtype.md#brandpanelpanorama) \| [*BrandpanelPanoramaVideo*](./enums/guaranteedinventoryserviceadtype.md#brandpanelpanoramavideo) \| [*TopImpactSquare*](./enums/guaranteedinventoryserviceadtype.md#topimpactsquare) \| [*TopImpactSquareVideo*](./enums/guaranteedinventoryserviceadtype.md#topimpactsquarevideo) \| [*TopImpactQuintie*](./enums/guaranteedinventoryserviceadtype.md#topimpactquintie) \| [*TopImpactQuintieVideo*](./enums/guaranteedinventoryserviceadtype.md#topimpactquintievideo) \| [*TopImpactPanorama*](./enums/guaranteedinventoryserviceadtype.md#topimpactpanorama) \| [*TopImpactPanoramaVideo*](./enums/guaranteedinventoryserviceadtype.md#topimpactpanoramavideo) \| [*TopImpactPanoramaSideVisionVideo*](./enums/guaranteedinventoryserviceadtype.md#topimpactpanoramasidevisionvideo) \| [*TopImpactPanoramaSideSwitchVideo*](./enums/guaranteedinventoryserviceadtype.md#topimpactpanoramasideswitchvideo) \| [*TopImpactTheaterVideo*](./enums/guaranteedinventoryserviceadtype.md#topimpacttheatervideo) \| [*TopImpactSquareSpecial*](./enums/guaranteedinventoryserviceadtype.md#topimpactsquarespecial) \| [*TopImpactSquareSpecialVideo*](./enums/guaranteedinventoryserviceadtype.md#topimpactsquarespecialvideo) \| [*TopImpactPrimeDisplayDouble*](./enums/guaranteedinventoryserviceadtype.md#topimpactprimedisplaydouble) \| [*TopImpactPrimeDisplayDoubleVideo*](./enums/guaranteedinventoryserviceadtype.md#topimpactprimedisplaydoublevideo) \| [*InstreamVideoAd*](./enums/guaranteedinventoryserviceadtype.md#instreamvideoad) \| [*CarouselAd*](./enums/guaranteedinventoryserviceadtype.md#carouselad) \| [*Unknown*](./enums/guaranteedinventoryserviceadtype.md#unknown)

**`memberof`** GuaranteedInventoryServiceAdRequirement

___

### aspectRatio

• `Optional` **aspectRatio**: ``null`` \| *string*

<div lang=\"ja\"> アスペクト比の種類です。<br> このフィールドは、レスポンスの際に返却されますが、リクエストの際には無視されます。 </div> 

**`memberof`** GuaranteedInventoryServiceAdRequirement

___

### mediaAdFormat

• `Optional` **mediaAdFormat**: ``null`` \| *string*

<div lang=\"ja\"> メディアのフォーマットです。<br> ADD時、このフィールドは必須となります。<br> ※指定可能な値は、DictionaryServiceのgetMediaAdFormatで取得されるDictionaryServiceMediaAdFormatのadFormatフィールドをご確認ください。 </div> 

**`memberof`** GuaranteedInventoryServiceAdRequirement
