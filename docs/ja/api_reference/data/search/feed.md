# Feed


<div lang=\"ja\">Feedオブジェクトは、自動データ挿入のリストを格納します。</div> 

## Table of contents

### Properties

- [accountId](feed.md#accountid)
- [domain](feed.md#domain)
- [feedAttribute](feed.md#feedattribute)
- [feedId](feed.md#feedid)
- [feedName](feed.md#feedname)
- [feedTrackId](feed.md#feedtrackid)
- [placeholderType](feed.md#placeholdertype)

## Properties

### accountId

• `Optional` **accountId**: ``null`` \| *number*

<div lang=\"ja\">アカウントIDです。<br> ※入稿の仕様変更により不要になりました。<br> このフィールドは、レスポンスの際に返却されますが、リクエストの際には無視されます。</div> 

**`memberof`** Feed

___

### domain

• `Optional` **domain**: ``null`` \| *string*

<div lang=\"ja\">ドメインです。<br> このフィールドは、ADD時に省略可能となり、SETおよびREMOVE時に無視されます。</div> 

**`memberof`** Feed

___

### feedAttribute

• `Optional` **feedAttribute**: ``null`` \| [*FeedServiceAttribute*](feedserviceattribute.md)[]

**`memberof`** Feed

___

### feedId

• `Optional` **feedId**: ``null`` \| *number*

<div lang=\"ja\">FeedIDです。<br> このフィールドは、SETおよびREMOVE時に必須となり、ADD時は無視されます。</div> 

**`memberof`** Feed

___

### feedName

• `Optional` **feedName**: ``null`` \| *string*

<div lang=\"ja\">Feedのリスト名です。<br> このフィールドは、ADD時に必須となり、SETおよびREMOVE時に無視されます。</div> 

**`memberof`** Feed

___

### feedTrackId

• `Optional` **feedTrackId**: ``null`` \| *number*

<div lang=\"ja\">Feedのトラッキング用IDです。<br> このフィールドは、レスポンスの際に返却されますが、リクエストの際には無視されます。</div> 

**`memberof`** Feed

___

### placeholderType

• `Optional` **placeholderType**: ``null`` \| [*AdCustomizer*](./enums/feedserviceplaceholdertype.md#adcustomizer) \| [*DynamicAdForSearchPageFeeds*](./enums/feedserviceplaceholdertype.md#dynamicadforsearchpagefeeds) \| [*Unknown*](./enums/feedserviceplaceholdertype.md#unknown)

**`memberof`** Feed
