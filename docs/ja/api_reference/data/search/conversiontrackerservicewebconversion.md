# ConversionTrackerServiceWebConversion


<div lang=\"ja\">ConversionTrackerServiceWebConversionオブジェクトは、ウェブページのコンバージョン測定タグやタグごとのパフォーマンスデータなどのコンバージョントラッカー情報を表します。<br> このフィールドは、ADDおよびSET時に省略可能となります。<br> ※ADD時、conversionTrackerTypeがWEB_CONVERSIONの場合、このフィールドは必須となります。</div> 

## Table of contents

### Properties

- [advancedSnippet](conversiontrackerservicewebconversion.md#advancedsnippet)
- [markupLanguage](conversiontrackerservicewebconversion.md#markuplanguage)
- [snippet](conversiontrackerservicewebconversion.md#snippet)
- [trackingCodeType](conversiontrackerservicewebconversion.md#trackingcodetype)

## Properties

### advancedSnippet

• `Optional` **advancedSnippet**: ``null`` \| *string*

<div lang=\"ja\">   リニューアル版のコンバージョンタグは、従来のタグよりもブラウザーなどの環境の影響を受けづらい新しいフォーマットです。<br>   詳細は以下のヘルプを参照してください。<br>   ・<a href=\"https://ads-help.yahoo.co.jp/yahooads/ss/articledetail?lan=ja&aid=1159\">コンバージョン測定とは</a><br>   このフィールドは、レスポンスの際に返却されますが、リクエストの際には無視されます。 </div> 

**`memberof`** ConversionTrackerServiceWebConversion

___

### markupLanguage

• `Optional` **markupLanguage**: ``null`` \| [*Html*](./enums/conversiontrackerservicemarkuplanguage.md#html) \| [*Chtml*](./enums/conversiontrackerservicemarkuplanguage.md#chtml) \| [*Xhtml*](./enums/conversiontrackerservicemarkuplanguage.md#xhtml) \| [*Wml*](./enums/conversiontrackerservicemarkuplanguage.md#wml) \| [*Unknown*](./enums/conversiontrackerservicemarkuplanguage.md#unknown)

**`memberof`** ConversionTrackerServiceWebConversion

___

### snippet

• `Optional` **snippet**: ``null`` \| *string*

<div lang=\"ja\">トラッキングスクリプトです。<br> このフィールドは、レスポンスの際に返却されますが、リクエストの際には無視されます。</div> 

**`memberof`** ConversionTrackerServiceWebConversion

___

### trackingCodeType

• `Optional` **trackingCodeType**: ``null`` \| [*Webpage*](./enums/conversiontrackerservicetrackingcodetype.md#webpage) \| [*ClickToCall*](./enums/conversiontrackerservicetrackingcodetype.md#clicktocall) \| [*Import*](./enums/conversiontrackerservicetrackingcodetype.md#import) \| [*Unknown*](./enums/conversiontrackerservicetrackingcodetype.md#unknown)

**`memberof`** ConversionTrackerServiceWebConversion
