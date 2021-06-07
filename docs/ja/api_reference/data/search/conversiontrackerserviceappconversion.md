# ConversionTrackerServiceAppConversion


<div lang=\"ja\">ConversionTrackerServiceAppConversionオブジェクトは、アプリコンバージョン測定タグやタグごとのパフォーマンスデータなどのアプリコンバージョントラッカー情報を表します。<br> このフィールドは、ADDおよびSET時に省略可能となります。<br> ※ADD時、conversionTrackerTypeがAPP_CONVERSIONの場合は必須です。</div> 

## Table of contents

### Properties

- [appConversionType](conversiontrackerserviceappconversion.md#appconversiontype)
- [appId](conversiontrackerserviceappconversion.md#appid)
- [appPlatform](conversiontrackerserviceappconversion.md#appplatform)
- [appPostbackUrl](conversiontrackerserviceappconversion.md#apppostbackurl)
- [snippetId](conversiontrackerserviceappconversion.md#snippetid)
- [snippetLabel](conversiontrackerserviceappconversion.md#snippetlabel)

## Properties

### appConversionType

• `Optional` **appConversionType**: ``null`` \| [*Download*](./enums/conversiontrackerserviceappconversiontype.md#download) \| [*InAppPurchase*](./enums/conversiontrackerserviceappconversiontype.md#inapppurchase) \| [*FirstOpen*](./enums/conversiontrackerserviceappconversiontype.md#firstopen) \| [*Unknown*](./enums/conversiontrackerserviceappconversiontype.md#unknown)

**`memberof`** ConversionTrackerServiceAppConversion

___

### appId

• `Optional` **appId**: ``null`` \| *string*

<div lang=\"ja\">アプリケーションIDです。<br> このフィールドは、いずれの場合でも省略可能となります。</div> 

**`memberof`** ConversionTrackerServiceAppConversion

___

### appPlatform

• `Optional` **appPlatform**: ``null`` \| [*AndroidMarket*](./enums/conversiontrackerserviceappplatform.md#androidmarket) \| [*Unknown*](./enums/conversiontrackerserviceappplatform.md#unknown)

**`memberof`** ConversionTrackerServiceAppConversion

___

### appPostbackUrl

• `Optional` **appPostbackUrl**: ``null`` \| [*ConversionTrackerServiceAppPostbackUrl*](conversiontrackerserviceapppostbackurl.md)

**`memberof`** ConversionTrackerServiceAppConversion

___

### snippetId

• `Optional` **snippetId**: ``null`` \| *number*

<div lang=\"ja\">コンバージョンIDです。</div> 

**`memberof`** ConversionTrackerServiceAppConversion

___

### snippetLabel

• `Optional` **snippetLabel**: ``null`` \| *string*

<div lang=\"ja\">コンバージョントラッカーラベルです。</div> 

**`memberof`** ConversionTrackerServiceAppConversion
