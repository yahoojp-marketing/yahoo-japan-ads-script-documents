# ConversionGroupServiceConversion


<div lang=\"ja\">ConversionGroupServiceConversionオブジェクトは、コンバージョン測定タグなどのコンバージョントラッカー情報を表します。</div> 

## Table of contents

### Properties

- [conversionTagId](conversiongroupserviceconversion.md#conversiontagid)
- [conversionTagName](conversiongroupserviceconversion.md#conversiontagname)
- [conversionTrackerId](conversiongroupserviceconversion.md#conversiontrackerid)
- [conversionTrackerType](conversiongroupserviceconversion.md#conversiontrackertype)
- [status](conversiongroupserviceconversion.md#status)

## Properties

### conversionTagId

• `Optional` **conversionTagId**: ``null`` \| *number*

<div lang=\"ja\"> コンバージョンタグIDです。<br> このフィールドは、レスポンスの際に返却されますが、リクエストの際には無視されます。 </div> 

**`memberof`** ConversionGroupServiceConversion

___

### conversionTagName

• `Optional` **conversionTagName**: ``null`` \| *string*

<div lang=\"ja\"> コンバージョンタグ名です。<br> このフィールドは、レスポンスの際に返却されますが、リクエストの際には無視されます。 </div> 

**`memberof`** ConversionGroupServiceConversion

___

### conversionTrackerId

• `Optional` **conversionTrackerId**: ``null`` \| *number*

<div lang=\"ja\"> コンバージョントラッカーIDです。<br> このフィールドは、ADD時は必須となり、SET時は省略可能となります。 </div> 

**`memberof`** ConversionGroupServiceConversion

___

### conversionTrackerType

• `Optional` **conversionTrackerType**: ``null`` \| [*WebConversion*](./enums/conversiontrackerservicetype.md#webconversion) \| [*AppConversion*](./enums/conversiontrackerservicetype.md#appconversion) \| [*Unknown*](./enums/conversiontrackerservicetype.md#unknown)

**`memberof`** ConversionGroupServiceConversion

___

### status

• `Optional` **status**: ``null`` \| [*Enabled*](./enums/conversiontrackerservicestatus.md#enabled) \| [*Disabled*](./enums/conversiontrackerservicestatus.md#disabled) \| [*Unknown*](./enums/conversiontrackerservicestatus.md#unknown)

**`memberof`** ConversionGroupServiceConversion
