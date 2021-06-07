# VideoServiceSetting


<div lang=\"ja\">VideoServiceSettingオブジェクトは、動画の設定内容を保持します。</div> 

## Table of contents

### Properties

- [fileSize](videoservicesetting.md#filesize)
- [fileType](videoservicesetting.md#filetype)
- [height](videoservicesetting.md#height)
- [playbackTime](videoservicesetting.md#playbacktime)
- [videoAdFormat](videoservicesetting.md#videoadformat)
- [videoAspectRatio](videoservicesetting.md#videoaspectratio)
- [width](videoservicesetting.md#width)

## Properties

### fileSize

• `Optional` **fileSize**: ``null`` \| *number*

<div lang=\"ja\">動画のファイルサイズです。</div> 

**`memberof`** VideoServiceSetting

___

### fileType

• `Optional` **fileType**: ``null`` \| [*Mp4*](./enums/videoservicefiletype.md#mp4) \| [*Unknown*](./enums/videoservicefiletype.md#unknown)

**`memberof`** VideoServiceSetting

___

### height

• `Optional` **height**: ``null`` \| *number*

<div lang=\"ja\">動画の高さ（縦の長さ）です。</div> 

**`memberof`** VideoServiceSetting

___

### playbackTime

• `Optional` **playbackTime**: ``null`` \| *number*

<div lang=\"ja\">動画再生時間（秒）です。</div> 

**`memberof`** VideoServiceSetting

___

### videoAdFormat

• `Optional` **videoAdFormat**: ``null`` \| *string*

<div lang=\"ja\">動画広告の種類です。</div> 

**`memberof`** VideoServiceSetting

___

### videoAspectRatio

• `Optional` **videoAspectRatio**: ``null`` \| *string*

<div lang=\"ja\"> 動画アスペクト比の種類です。<br> ※指定可能な値は、DictionaryServiceのgetMediaAdFormatで取得されるDictionaryServiceMediaAdFormatのaspectRatioフィールドをご確認ください。 </div> 

**`memberof`** VideoServiceSetting

___

### width

• `Optional` **width**: ``null`` \| *number*

<div lang=\"ja\">動画の横幅です。</div> 

**`memberof`** VideoServiceSetting
