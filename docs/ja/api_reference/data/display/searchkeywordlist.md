# SearchKeywordList


<div lang=\"ja\">SearchKeywordListオブジェクトは、サーチキーワードリストを表します。</div> 

## Table of contents

### Properties

- [accountId](searchkeywordlist.md#accountid)
- [deliveryStatus](searchkeywordlist.md#deliverystatus)
- [isRemoveSearchKeywordListDescription](searchkeywordlist.md#isremovesearchkeywordlistdescription)
- [keywordFrequency](searchkeywordlist.md#keywordfrequency)
- [keywordRecency](searchkeywordlist.md#keywordrecency)
- [searchKeyword](searchkeywordlist.md#searchkeyword)
- [searchKeywordListDescription](searchkeywordlist.md#searchkeywordlistdescription)
- [searchKeywordListId](searchkeywordlist.md#searchkeywordlistid)
- [searchKeywordListName](searchkeywordlist.md#searchkeywordlistname)

## Properties

### accountId

• `Optional` **accountId**: ``null`` \| *number*

<div lang=\"ja\"> アカウントIDです。<br> このフィールドは、リクエストの場合は必須です。 </div> 

**`memberof`** SearchKeywordList

___

### deliveryStatus

• `Optional` **deliveryStatus**: ``null`` \| [*Paused*](./enums/searchkeywordlistservicedeliverystatus.md#paused) \| [*Active*](./enums/searchkeywordlistservicedeliverystatus.md#active) \| [*Unknown*](./enums/searchkeywordlistservicedeliverystatus.md#unknown)

**`memberof`** SearchKeywordList

___

### isRemoveSearchKeywordListDescription

• `Optional` **isRemoveSearchKeywordListDescription**: ``null`` \| [*True*](./enums/searchkeywordlistserviceisremoveflg.md#true) \| [*False*](./enums/searchkeywordlistserviceisremoveflg.md#false) \| [*Unknown*](./enums/searchkeywordlistserviceisremoveflg.md#unknown)

**`memberof`** SearchKeywordList

___

### keywordFrequency

• `Optional` **keywordFrequency**: ``null`` \| [*OnceOrMore*](./enums/searchkeywordlistservicekeywordfrequency.md#onceormore) \| [*TwiceOrMore*](./enums/searchkeywordlistservicekeywordfrequency.md#twiceormore) \| [*ThreeTimesOrMore*](./enums/searchkeywordlistservicekeywordfrequency.md#threetimesormore) \| [*Unknown*](./enums/searchkeywordlistservicekeywordfrequency.md#unknown)

**`memberof`** SearchKeywordList

___

### keywordRecency

• `Optional` **keywordRecency**: ``null`` \| [*Within1Day*](./enums/searchkeywordlistservicekeywordrecency.md#within1day) \| [*Within3Days*](./enums/searchkeywordlistservicekeywordrecency.md#within3days) \| [*Within7Days*](./enums/searchkeywordlistservicekeywordrecency.md#within7days) \| [*Within14Days*](./enums/searchkeywordlistservicekeywordrecency.md#within14days) \| [*Within30Days*](./enums/searchkeywordlistservicekeywordrecency.md#within30days) \| [*Unknown*](./enums/searchkeywordlistservicekeywordrecency.md#unknown)

**`memberof`** SearchKeywordList

___

### searchKeyword

• `Optional` **searchKeyword**: ``null`` \| [*SearchKeywordListServiceSearchKeyword*](searchkeywordlistservicesearchkeyword.md)[]

**`memberof`** SearchKeywordList

___

### searchKeywordListDescription

• `Optional` **searchKeywordListDescription**: ``null`` \| *string*

<div lang=\"ja\"> サーチキーワードリストの説明文です。<br> このフィールドは、ADDおよびSET時に省略可能となります。 </div> 

**`memberof`** SearchKeywordList

___

### searchKeywordListId

• `Optional` **searchKeywordListId**: ``null`` \| *number*

<div lang=\"ja\"> サーチキーワードリストIDです。<br> このフィールドは、SETおよびREMOVE時に必須となります。 </div> 

**`memberof`** SearchKeywordList

___

### searchKeywordListName

• `Optional` **searchKeywordListName**: ``null`` \| *string*

<div lang=\"ja\"> サーチキーワードリスト名です。<br> このフィールドは、ADD時に必須となり、SET時に省略可能となります。 </div> 

**`memberof`** SearchKeywordList
