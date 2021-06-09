# ContentsKeywordIdeaServiceSelector


<div lang=\"ja\">ContentsKeywordIdeaServiceSelectorオブジェクトは、コンテンツターゲティング対象キーワードのリストを表します。</div> 

## Table of contents

### Properties

- [keyword](contentskeywordideaserviceselector.md#keyword)
- [keywordIds](contentskeywordideaserviceselector.md#keywordids)
- [numberResults](contentskeywordideaserviceselector.md#numberresults)
- [sortField](contentskeywordideaserviceselector.md#sortfield)
- [sortType](contentskeywordideaserviceselector.md#sorttype)
- [startIndex](contentskeywordideaserviceselector.md#startindex)

## Properties

### keyword

• `Optional` **keyword**: ``null`` \| [*ContentsKeywordIdeaServiceKeyword*](contentskeywordideaservicekeyword.md)

**`memberof`** ContentsKeywordIdeaServiceSelector

___

### keywordIds

• `Optional` **keywordIds**: ``null`` \| *number*[]

<div lang=\"ja\"> 検索条件：キーワードID<br> ※キーワード検索用<br> ※キーワード、キーワードIDの同時指定はできません。 </div> 

**`memberof`** ContentsKeywordIdeaServiceSelector

___

### numberResults

• `Optional` **numberResults**: ``null`` \| *number*

<div lang=\"ja\">ページの最大件数です。このフィールドは、1以上を指定する必要があります。</div> 

**`memberof`** ContentsKeywordIdeaServiceSelector

___

### sortField

• `Optional` **sortField**: ``null`` \| [*Keyword*](./enums/contentskeywordideaservicesortfield.md#keyword) \| [*KeywordId*](./enums/contentskeywordideaservicesortfield.md#keywordid) \| [*SearchVolume*](./enums/contentskeywordideaservicesortfield.md#searchvolume) \| [*CreatedDate*](./enums/contentskeywordideaservicesortfield.md#createddate) \| [*Unknown*](./enums/contentskeywordideaservicesortfield.md#unknown)

**`memberof`** ContentsKeywordIdeaServiceSelector

___

### sortType

• `Optional` **sortType**: ``null`` \| [*Asc*](./enums/contentskeywordideaservicesorttype.md#asc) \| [*Desc*](./enums/contentskeywordideaservicesorttype.md#desc) \| [*Unknown*](./enums/contentskeywordideaservicesorttype.md#unknown)

**`memberof`** ContentsKeywordIdeaServiceSelector

___

### startIndex

• `Optional` **startIndex**: ``null`` \| *number*

<div lang=\"ja\">ページの先頭のインデックスです。このフィールドは、1以上を指定する必要があります。</div> 

**`memberof`** ContentsKeywordIdeaServiceSelector
