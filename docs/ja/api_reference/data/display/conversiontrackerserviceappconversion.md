# ConversionTrackerServiceAppConversion


<div lang=\"ja\"> ConversionTrackerServiceAppConversionオブジェクトは、アプリコンバージョントラッカーの情報を保持します。<br> このフィールドは、ADD時は省略可能となり、SET時は無視されます。ADD時、conversionTrackerTypeがAPP_CONVERSIONの場合、必須です。 </div> 

## Table of contents

### Properties

- [appConversionPlatform](conversiontrackerserviceappconversion.md#appconversionplatform)
- [appConversionType](conversiontrackerserviceappconversion.md#appconversiontype)
- [appId](conversiontrackerserviceappconversion.md#appid)

## Properties

### appConversionPlatform

• `Optional` **appConversionPlatform**: ``null`` \| [*Itunes*](./enums/conversiontrackerserviceappconversionplatform.md#itunes) \| [*AndroidMarket*](./enums/conversiontrackerserviceappconversionplatform.md#androidmarket) \| [*Unknown*](./enums/conversiontrackerserviceappconversionplatform.md#unknown)

**`memberof`** ConversionTrackerServiceAppConversion

___

### appConversionType

• `Optional` **appConversionType**: ``null`` \| [*FirstOpen*](./enums/conversiontrackerserviceappconversiontype.md#firstopen) \| [*Unknown*](./enums/conversiontrackerserviceappconversiontype.md#unknown)

**`memberof`** ConversionTrackerServiceAppConversion

___

### appId

• `Optional` **appId**: ``null`` \| *string*

<div lang=\"ja\"> 計測対象のアプリIDです。<br> このフィールドは、ADD時は必須となり、SET時は無視されます。 </div> 

**`memberof`** ConversionTrackerServiceAppConversion
