# MediaServiceImageMedia


<div lang=\"ja\"> MediaServiceImageMediaオブジェクトは、画像を格納するコンテナです。<br> このフィールドは、SET時に必須となります。 </div> 

## Table of contents

### Properties

- [aspectRatio](mediaserviceimagemedia.md#aspectratio)
- [data](mediaserviceimagemedia.md#data)
- [fileSize](mediaserviceimagemedia.md#filesize)
- [height](mediaserviceimagemedia.md#height)
- [mediaAdFormat](mediaserviceimagemedia.md#mediaadformat)
- [mediaFileType](mediaserviceimagemedia.md#mediafiletype)
- [mediaType](mediaserviceimagemedia.md#mediatype)
- [width](mediaserviceimagemedia.md#width)

## Properties

### aspectRatio

• `Optional` **aspectRatio**: ``null`` \| *string*

<div lang=\"ja\"> 画像アスペクト比の種類です。<br> このフィールドは、レスポンスの際に返却されますが、リクエストの際には無視されます。<br> ※指定可能な値は、DictionaryServiceのgetMediaAdFormatで取得されるDictionaryServiceMediaAdFormatのaspectRatioフィールドをご確認ください。 </div> 

**`memberof`** MediaServiceImageMedia

___

### data

• `Optional` **data**: ``null`` \| *string*

<div lang=\"ja\">画像ファイルのbase64エンコードです。ADD時のみ指定可能で、GET時のレスポンスでは値は取得されません。</div> 

**`memberof`** MediaServiceImageMedia

___

### fileSize

• `Optional` **fileSize**: ``null`` \| *number*

<div lang=\"ja\"> ファイルサイズです。<br> このフィールドは、レスポンスの際に返却されますが、リクエストの際には無視されます。 </div> 

**`memberof`** MediaServiceImageMedia

___

### height

• `Optional` **height**: ``null`` \| *number*

<div lang=\"ja\"> 縦の長さです。<br> このフィールドは、レスポンスの際に返却されますが、リクエストの際には無視されます。 </div> 

**`memberof`** MediaServiceImageMedia

___

### mediaAdFormat

• `Optional` **mediaAdFormat**: ``null`` \| *string*

<div lang=\"ja\"> 画像フォーマットの種類です。<br> このフィールドは、レスポンスの際に返却されますが、リクエストの際には無視されます。<br> ※指定可能な値は、DictionaryServiceのgetMediaAdFormatで取得されるDictionaryServiceMediaAdFormatのadFormatフィールドをご確認ください。 </div> 

**`memberof`** MediaServiceImageMedia

___

### mediaFileType

• `Optional` **mediaFileType**: ``null`` \| [*Jpeg*](./enums/mediaservicefiletype.md#jpeg) \| [*Gif*](./enums/mediaservicefiletype.md#gif) \| [*Png*](./enums/mediaservicefiletype.md#png) \| [*Unknown*](./enums/mediaservicefiletype.md#unknown)

**`memberof`** MediaServiceImageMedia

___

### mediaType

• `Optional` **mediaType**: ``null`` \| [*Image*](./enums/mediaservicetype.md#image) \| [*AnimationImage*](./enums/mediaservicetype.md#animationimage) \| [*Unknown*](./enums/mediaservicetype.md#unknown)

**`memberof`** MediaServiceImageMedia

___

### width

• `Optional` **width**: ``null`` \| *number*

<div lang=\"ja\"> 横幅です。<br> このフィールドは、レスポンスの際に返却されますが、リクエストの際には無視されます。 </div> 

**`memberof`** MediaServiceImageMedia
