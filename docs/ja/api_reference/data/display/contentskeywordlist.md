# ContentsKeywordList


<div lang=\"ja\">ContentsKeywordListオブジェクトは、コンテンツキーワードリストを表します。</div> 

## Table of contents

### Properties

- [accountId](contentskeywordlist.md#accountid)
- [brandSafetyDenyListFlg](contentskeywordlist.md#brandsafetydenylistflg)
- [contentsKeyword](contentskeywordlist.md#contentskeyword)
- [contentsKeywordListDescription](contentskeywordlist.md#contentskeywordlistdescription)
- [contentsKeywordListId](contentskeywordlist.md#contentskeywordlistid)
- [contentsKeywordListName](contentskeywordlist.md#contentskeywordlistname)
- [isRemoveContentsKeywordListDescription](contentskeywordlist.md#isremovecontentskeywordlistdescription)

## Properties

### accountId

• `Optional` **accountId**: ``null`` \| *number*

<div lang=\"ja\"> アカウントIDです。<br> このフィールドは、リクエストの場合は必須です。 </div> 

**`memberof`** ContentsKeywordList

___

### brandSafetyDenyListFlg

• `Optional` **brandSafetyDenyListFlg**: ``null`` \| *boolean*

<div lang=\"ja\"> 除外専用リストかどうかのフラグです。<br> 除外専用リストには下記の制約があります。<br> ・１アカウントにつき1つ作成が可能です。<br> ・除外にのみ紐付け可能です。<br> ・YDNキャンペーンには紐付けできません。<br> このフィールドは、ADD時に省略可能(デフォルトの値はFALSE)、SET時に指定不可となります。 </div>  <dl class=term>   <dt class=\"term__item\">TRUE</dt>   <dd class=\"term__desc\"><span lang=\"ja\">除外専用リストです。</span></dd>   <dt class=\"term__item\">FALSE</dt>   <dd class=\"term__desc\"><span lang=\"ja\">通常のurlリストです。</span></dd> </dl>

**`memberof`** ContentsKeywordList

___

### contentsKeyword

• `Optional` **contentsKeyword**: ``null`` \| [*ContentsKeywordListServiceContentsKeyword*](contentskeywordlistservicecontentskeyword.md)[]

**`memberof`** ContentsKeywordList

___

### contentsKeywordListDescription

• `Optional` **contentsKeywordListDescription**: ``null`` \| *string*

<div lang=\"ja\"> コンテンツキーワードリストの説明文です。<br> このフィールドは、ADDおよびSET時に省略可能となります。 </div> 

**`memberof`** ContentsKeywordList

___

### contentsKeywordListId

• `Optional` **contentsKeywordListId**: ``null`` \| *number*

<div lang=\"ja\"> コンテンツキーワードリストIDです。<br> このフィールドは、SETおよびREMOVE時に必須となります。 </div> 

**`memberof`** ContentsKeywordList

___

### contentsKeywordListName

• `Optional` **contentsKeywordListName**: ``null`` \| *string*

<div lang=\"ja\"> コンテンツキーワードリスト名です。<br> このフィールドは、ADD時に必須となり、SET時に省略可能となります。 </div> 

**`memberof`** ContentsKeywordList

___

### isRemoveContentsKeywordListDescription

• `Optional` **isRemoveContentsKeywordListDescription**: ``null`` \| [*True*](./enums/contentskeywordlistserviceisremoveflg.md#true) \| [*False*](./enums/contentskeywordlistserviceisremoveflg.md#false) \| [*Unknown*](./enums/contentskeywordlistserviceisremoveflg.md#unknown)

**`memberof`** ContentsKeywordList
