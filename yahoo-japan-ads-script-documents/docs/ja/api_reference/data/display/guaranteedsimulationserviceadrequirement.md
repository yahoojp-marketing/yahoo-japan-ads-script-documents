# GuaranteedSimulationServiceAdRequirement


<div lang=\"ja\"> GuaranteedSimulationServiceAdRequirementオブジェクトは、予約型の広告を構成する条件を表します。<br> ADD時、このフィールドは必須となります。 </div> 

## Table of contents

### Properties

- [adType](guaranteedsimulationserviceadrequirement.md#adtype)
- [aspectRatio](guaranteedsimulationserviceadrequirement.md#aspectratio)
- [mediaAdFormat](guaranteedsimulationserviceadrequirement.md#mediaadformat)

## Properties

### adType

• `Optional` **adType**: ``null`` \| [*BannerVideoAd*](./enums/guaranteedsimulationserviceadtype.md#bannervideoad) \| [*BannerImageAd*](./enums/guaranteedsimulationserviceadtype.md#bannerimagead) \| [*BrandpanelQuintie*](./enums/guaranteedsimulationserviceadtype.md#brandpanelquintie) \| [*BrandpanelQuintieVideo*](./enums/guaranteedsimulationserviceadtype.md#brandpanelquintievideo) \| [*BrandpanelPanorama*](./enums/guaranteedsimulationserviceadtype.md#brandpanelpanorama) \| [*BrandpanelPanoramaVideo*](./enums/guaranteedsimulationserviceadtype.md#brandpanelpanoramavideo) \| [*TopImpactSquare*](./enums/guaranteedsimulationserviceadtype.md#topimpactsquare) \| [*TopImpactSquareVideo*](./enums/guaranteedsimulationserviceadtype.md#topimpactsquarevideo) \| [*TopImpactQuintie*](./enums/guaranteedsimulationserviceadtype.md#topimpactquintie) \| [*TopImpactQuintieVideo*](./enums/guaranteedsimulationserviceadtype.md#topimpactquintievideo) \| [*TopImpactPanorama*](./enums/guaranteedsimulationserviceadtype.md#topimpactpanorama) \| [*TopImpactPanoramaVideo*](./enums/guaranteedsimulationserviceadtype.md#topimpactpanoramavideo) \| [*TopImpactPanoramaSideVisionVideo*](./enums/guaranteedsimulationserviceadtype.md#topimpactpanoramasidevisionvideo) \| [*TopImpactPanoramaSideSwitchVideo*](./enums/guaranteedsimulationserviceadtype.md#topimpactpanoramasideswitchvideo) \| [*TopImpactTheaterVideo*](./enums/guaranteedsimulationserviceadtype.md#topimpacttheatervideo) \| [*TopImpactSquareSpecial*](./enums/guaranteedsimulationserviceadtype.md#topimpactsquarespecial) \| [*TopImpactSquareSpecialVideo*](./enums/guaranteedsimulationserviceadtype.md#topimpactsquarespecialvideo) \| [*TopImpactPrimeDisplayDouble*](./enums/guaranteedsimulationserviceadtype.md#topimpactprimedisplaydouble) \| [*TopImpactPrimeDisplayDoubleVideo*](./enums/guaranteedsimulationserviceadtype.md#topimpactprimedisplaydoublevideo) \| [*InstreamVideoAd*](./enums/guaranteedsimulationserviceadtype.md#instreamvideoad) \| [*Unknown*](./enums/guaranteedsimulationserviceadtype.md#unknown)

**`memberof`** GuaranteedSimulationServiceAdRequirement

___

### aspectRatio

• `Optional` **aspectRatio**: ``null`` \| *string*

<div lang=\"ja\"> アスペクト比の種類です。<br> このフィールドは、レスポンスの際に返却されますが、リクエストの際には無視されます。 </div> 

**`memberof`** GuaranteedSimulationServiceAdRequirement

___

### mediaAdFormat

• `Optional` **mediaAdFormat**: ``null`` \| *string*

<div lang=\"ja\"> メディアのフォーマットです。<br> ADD時、このフィールドは必須となります。<br> ※指定可能な値は、DictionaryServiceのgetMediaAdFormatで取得されるDictionaryServiceMediaAdFormatのadFormatフィールドをご確認ください。 </div> 

**`memberof`** GuaranteedSimulationServiceAdRequirement
