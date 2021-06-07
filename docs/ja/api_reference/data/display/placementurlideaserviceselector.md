# PlacementUrlIdeaServiceSelector


<div lang=\"ja\">PlacementUrlIdeaServiceSelectorオブジェクトは、getメソッドの検索条件（実行パラメータ）を保持するオブジェクトです。</div> 

## Table of contents

### Properties

- [adFormats](placementurlideaserviceselector.md#adformats)
- [keyword](placementurlideaserviceselector.md#keyword)
- [numberResults](placementurlideaserviceselector.md#numberresults)
- [siteCategories](placementurlideaserviceselector.md#sitecategories)
- [startIndex](placementurlideaserviceselector.md#startindex)

## Properties

### adFormats

• `Optional` **adFormats**: ``null`` \| [*PlacementUrlIdeaServiceAdFormatConditions*](placementurlideaserviceadformatconditions.md)[]

**`memberof`** PlacementUrlIdeaServiceSelector

___

### keyword

• `Optional` **keyword**: ``null`` \| *string*

<div lang=\"ja\"> 検索キーワードの配列です。<br> ・URLを検索するためのキーワードです。<br> ・部分一致です。<br> ・スペース区切りでAND検索です。<br> ・最大文字数250です。<br> ・スペース区切りでの単語数は最大10個です。 </div> 

**`memberof`** PlacementUrlIdeaServiceSelector

___

### numberResults

• `Optional` **numberResults**: ``null`` \| *number*

<div lang=\"ja\">ページの最大件数です。このフィールドは、1以上を指定する必要があります。</div> 

**`memberof`** PlacementUrlIdeaServiceSelector

___

### siteCategories

• `Optional` **siteCategories**: ``null`` \| *string*[]

<div lang=\"ja\"> カテゴリの配列です。<br> ・URLのカテゴリです。<br> ・完全一致です。<br> ・複数指定でOR検索です。<br> ・TC-SC-xxxxxxで現される規定値です。<br> ・DicitonaryServiceから返ってくるTC-SC-xxxxxxをそのまま指定です。<br> ・最大50件です。 </div> 

**`memberof`** PlacementUrlIdeaServiceSelector

___

### startIndex

• `Optional` **startIndex**: ``null`` \| *number*

<div lang=\"ja\">ページの先頭のインデックスです。このフィールドは、1以上を指定する必要があります。</div> 

**`memberof`** PlacementUrlIdeaServiceSelector
