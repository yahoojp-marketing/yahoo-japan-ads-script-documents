# ConversionTrackerServiceAppLinkConversion


<div lang=\"ja\">ConversionTrackerServiceAppLinkConversionオブジェクトは、アプリコンバージョン測定タグやタグごとのパフォーマンスデータなどのアプリコンバージョントラッカー情報を表します。<br> ADD時、このフィールドは省略可能となります。</div> 

## Table of contents

### Properties

- [advancedSnippet](conversiontrackerserviceapplinkconversion.md#advancedsnippet)
- [appEventType](conversiontrackerserviceapplinkconversion.md#appeventtype)
- [appId](conversiontrackerserviceapplinkconversion.md#appid)
- [appLinkPlatform](conversiontrackerserviceapplinkconversion.md#applinkplatform)
- [appVendorId](conversiontrackerserviceapplinkconversion.md#appvendorid)
- [snippet](conversiontrackerserviceapplinkconversion.md#snippet)

## Properties

### advancedSnippet

• `Optional` **advancedSnippet**: ``null`` \| *string*

<div lang=\"ja\">リニューアル版のコンバージョンタグは、従来のタグよりもブラウザーなどの環境の影響を受けづらい新しいフォーマットです。<br/> 詳細は[ヘルプ](https://support-marketing.yahoo.co.jp/promotionalads/ss/articledetail?lan=ja&aid=1159)をご参照ください。<br> このフィールドは、レスポンスの際に返却されますが、リクエストの際には無視されます。</div> 

**`memberof`** ConversionTrackerServiceAppLinkConversion

___

### appEventType

• `Optional` **appEventType**: ``null`` \| *string*

<div lang=\"ja\">アプリイベントタイプです。<br> このフィールドは、レスポンスの際に返却されますが、リクエストの際には無視されます。</div> 

**`memberof`** ConversionTrackerServiceAppLinkConversion

___

### appId

• `Optional` **appId**: ``null`` \| *string*

<div lang=\"ja\">アプリケーションIDです。<br> このフィールドは、レスポンスの際に返却されますが、リクエストの際には無視されます。</div> 

**`memberof`** ConversionTrackerServiceAppLinkConversion

___

### appLinkPlatform

• `Optional` **appLinkPlatform**: ``null`` \| [*Android*](./enums/conversiontrackerserviceapplinkplatform.md#android) \| [*Unknown*](./enums/conversiontrackerserviceapplinkplatform.md#unknown)

**`memberof`** ConversionTrackerServiceAppLinkConversion

___

### appVendorId

• `Optional` **appVendorId**: ``null`` \| *string*

<div lang=\"ja\">アプリ計測ベンダー識別子です。<br> このフィールドは、レスポンスの際に返却されますが、リクエストの際には無視されます。</div> 

**`memberof`** ConversionTrackerServiceAppLinkConversion

___

### snippet

• `Optional` **snippet**: ``null`` \| *string*

<div lang=\"ja\">トラッキングスクリプトです。<br> このフィールドは、レスポンスの際に返却されますが、リクエストの際には無視されます。</div> 

**`memberof`** ConversionTrackerServiceAppLinkConversion
