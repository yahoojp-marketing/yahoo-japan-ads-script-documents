# SearchKeywordIdea


<div lang=\"ja\">SearchKeywordIdeaオブジェクトは、サーチターゲティング対象キーワードです。</div> 

## Table of contents

### Properties

- [availabilityStatus](searchkeywordidea.md#availabilitystatus)
- [closeDate](searchkeywordidea.md#closedate)
- [desktopSearchVolume](searchkeywordidea.md#desktopsearchvolume)
- [releaseDate](searchkeywordidea.md#releasedate)
- [searchKeyword](searchkeywordidea.md#searchkeyword)
- [searchKeywordId](searchkeywordidea.md#searchkeywordid)
- [smartPhoneSearchVolume](searchkeywordidea.md#smartphonesearchvolume)
- [tabletSearchVolume](searchkeywordidea.md#tabletsearchvolume)

## Properties

### availabilityStatus

• `Optional` **availabilityStatus**: ``null`` \| [*Available*](./enums/searchkeywordideaserviceavailabilitystatus.md#available) \| [*Unavailable*](./enums/searchkeywordideaserviceavailabilitystatus.md#unavailable) \| [*Unknown*](./enums/searchkeywordideaserviceavailabilitystatus.md#unknown)

**`memberof`** SearchKeywordIdea

___

### closeDate

• `Optional` **closeDate**: ``null`` \| *string*

<div lang=\"ja\">サーチキーワード停止日です。<br> ※フォーマット：yyyyMMdd</div> 

**`memberof`** SearchKeywordIdea

___

### desktopSearchVolume

• `Optional` **desktopSearchVolume**: ``null`` \| *number*

<div lang=\"ja\"> PCでのリーチ数です。<br> ※1000件未満の場合は<br> 0が取得されます。<br> ※サーチキーワードの停止日以降はnullが返却されます。 </div> 

**`memberof`** SearchKeywordIdea

___

### releaseDate

• `Optional` **releaseDate**: ``null`` \| *string*

<div lang=\"ja\">サーチキーワード追加日です。<br> ※フォーマット：yyyyMMdd</div> 

**`memberof`** SearchKeywordIdea

___

### searchKeyword

• `Optional` **searchKeyword**: ``null`` \| *string*

<div lang=\"ja\">サーチキーワードです。</div> 

**`memberof`** SearchKeywordIdea

___

### searchKeywordId

• `Optional` **searchKeywordId**: ``null`` \| *number*

<div lang=\"ja\">サーチキーワードIDです。</div> 

**`memberof`** SearchKeywordIdea

___

### smartPhoneSearchVolume

• `Optional` **smartPhoneSearchVolume**: ``null`` \| *number*

<div lang=\"ja\"> スマートフォンでのリーチ数です。<br> ※1000件未満の場合は<br> 0が取得されます。<br> ※サーチキーワードの停止日以降はnullが返却されます。 </div> 

**`memberof`** SearchKeywordIdea

___

### tabletSearchVolume

• `Optional` **tabletSearchVolume**: ``null`` \| *number*

<div lang=\"ja\"> タブレットでのリーチ数です。<br> ※1000件未満の場合は<br> 0が取得されます。<br> ※サーチキーワードの停止日以降はnullが返却されます。 </div> 

**`memberof`** SearchKeywordIdea
