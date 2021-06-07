# SearchKeywordIdeaServiceSelector


<div lang=\"ja\">SearchKeywordIdeaServiceSelectorオブジェクトは、サーチターゲティング対象キーワードのリストを表します。</div> 

## Table of contents

### Properties

- [availabilityStatus](searchkeywordideaserviceselector.md#availabilitystatus)
- [keywordFrequency](searchkeywordideaserviceselector.md#keywordfrequency)
- [keywordIds](searchkeywordideaserviceselector.md#keywordids)
- [keywordRecency](searchkeywordideaserviceselector.md#keywordrecency)
- [keywords](searchkeywordideaserviceselector.md#keywords)
- [matchType](searchkeywordideaserviceselector.md#matchtype)
- [numberResults](searchkeywordideaserviceselector.md#numberresults)
- [sortField](searchkeywordideaserviceselector.md#sortfield)
- [sortType](searchkeywordideaserviceselector.md#sorttype)
- [startIndex](searchkeywordideaserviceselector.md#startindex)

## Properties

### availabilityStatus

• `Optional` **availabilityStatus**: ``null`` \| [*Available*](./enums/searchkeywordideaserviceavailabilitystatus.md#available) \| [*Unavailable*](./enums/searchkeywordideaserviceavailabilitystatus.md#unavailable) \| [*Unknown*](./enums/searchkeywordideaserviceavailabilitystatus.md#unknown)

**`memberof`** SearchKeywordIdeaServiceSelector

___

### keywordFrequency

• `Optional` **keywordFrequency**: ``null`` \| [*OnceOrMore*](./enums/searchkeywordideaservicekeywordfrequency.md#onceormore) \| [*TwiceOrMore*](./enums/searchkeywordideaservicekeywordfrequency.md#twiceormore) \| [*ThreeTimesOrMore*](./enums/searchkeywordideaservicekeywordfrequency.md#threetimesormore) \| [*Unknown*](./enums/searchkeywordideaservicekeywordfrequency.md#unknown)

**`memberof`** SearchKeywordIdeaServiceSelector

___

### keywordIds

• `Optional` **keywordIds**: ``null`` \| *number*[]

<div lang=\"ja\"> 検索条件：キーワードID<br> ※キーワード検索用<br> ※キーワード、キーワードIDの同時指定はできません。 </div> 

**`memberof`** SearchKeywordIdeaServiceSelector

___

### keywordRecency

• `Optional` **keywordRecency**: ``null`` \| [*Within1Day*](./enums/searchkeywordideaservicekeywordrecency.md#within1day) \| [*Within3Days*](./enums/searchkeywordideaservicekeywordrecency.md#within3days) \| [*Within7Days*](./enums/searchkeywordideaservicekeywordrecency.md#within7days) \| [*Within14Days*](./enums/searchkeywordideaservicekeywordrecency.md#within14days) \| [*Within30Days*](./enums/searchkeywordideaservicekeywordrecency.md#within30days) \| [*Unknown*](./enums/searchkeywordideaservicekeywordrecency.md#unknown)

**`memberof`** SearchKeywordIdeaServiceSelector

___

### keywords

• `Optional` **keywords**: ``null`` \| *string*[]

<div lang=\"ja\"> 検索条件：キーワード<br> ※キーワード提案用<br> ※キーワード、キーワードIDの同時指定はできません。 </div> 

**`memberof`** SearchKeywordIdeaServiceSelector

___

### matchType

• `Optional` **matchType**: ``null`` \| [*Exact*](./enums/searchkeywordideaservicematchtype.md#exact) \| [*Broad*](./enums/searchkeywordideaservicematchtype.md#broad) \| [*Unknown*](./enums/searchkeywordideaservicematchtype.md#unknown)

**`memberof`** SearchKeywordIdeaServiceSelector

___

### numberResults

• `Optional` **numberResults**: ``null`` \| *number*

<div lang=\"ja\">ページの最大件数です。このフィールドは、1以上を指定する必要があります。</div> 

**`memberof`** SearchKeywordIdeaServiceSelector

___

### sortField

• `Optional` **sortField**: ``null`` \| [*Keyword*](./enums/searchkeywordideaservicesortfield.md#keyword) \| [*KeywordId*](./enums/searchkeywordideaservicesortfield.md#keywordid) \| [*DesktopSearchVolume*](./enums/searchkeywordideaservicesortfield.md#desktopsearchvolume) \| [*SmartPhoneSearchVolume*](./enums/searchkeywordideaservicesortfield.md#smartphonesearchvolume) \| [*TabletSearchVolume*](./enums/searchkeywordideaservicesortfield.md#tabletsearchvolume) \| [*ReleaseDate*](./enums/searchkeywordideaservicesortfield.md#releasedate) \| [*Unknown*](./enums/searchkeywordideaservicesortfield.md#unknown)

**`memberof`** SearchKeywordIdeaServiceSelector

___

### sortType

• `Optional` **sortType**: ``null`` \| [*Asc*](./enums/searchkeywordideaservicesorttype.md#asc) \| [*Desc*](./enums/searchkeywordideaservicesorttype.md#desc) \| [*Unknown*](./enums/searchkeywordideaservicesorttype.md#unknown)

**`memberof`** SearchKeywordIdeaServiceSelector

___

### startIndex

• `Optional` **startIndex**: ``null`` \| *number*

<div lang=\"ja\">ページの先頭のインデックスです。このフィールドは、1以上を指定する必要があります。</div> 

**`memberof`** SearchKeywordIdeaServiceSelector
