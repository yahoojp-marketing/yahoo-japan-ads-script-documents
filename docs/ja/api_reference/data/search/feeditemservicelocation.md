# FeedItemServiceLocation


<div lang=\"ja\">FeedItemServiceLocationオブジェクトは、地域設定情報を格納します。<br> このフィールドは、レスポンスの際に返却されますが、リクエストの際には無視されます。<br> ※アドカスタマイザーの場合は、ADD時に省略可能となります。</div> 

## Table of contents

### Properties

- [criterionTypeFeedItem](feeditemservicelocation.md#criteriontypefeeditem)
- [geoRestriction](feeditemservicelocation.md#georestriction)
- [isRemove](feeditemservicelocation.md#isremove)
- [targetId](feeditemservicelocation.md#targetid)

## Properties

### criterionTypeFeedItem

• `Optional` **criterionTypeFeedItem**: ``null`` \| [*Location*](./enums/feeditemservicecriteriontypefeeditem.md#location) \| [*Unknown*](./enums/feeditemservicecriteriontypefeeditem.md#unknown)

**`memberof`** FeedItemServiceLocation

___

### geoRestriction

• `Optional` **geoRestriction**: ``null`` \| [*None*](./enums/feeditemservicegeorestriction.md#none) \| [*LocationOfPresence*](./enums/feeditemservicegeorestriction.md#locationofpresence) \| [*Unknown*](./enums/feeditemservicegeorestriction.md#unknown)

**`memberof`** FeedItemServiceLocation

___

### isRemove

• `Optional` **isRemove**: ``null`` \| [*True*](./enums/feeditemserviceisremove.md#true) \| [*False*](./enums/feeditemserviceisremove.md#false) \| [*Unknown*](./enums/feeditemserviceisremove.md#unknown)

**`memberof`** FeedItemServiceLocation

___

### targetId

• `Optional` **targetId**: ``null`` \| *string*

<div lang=\"ja\">地域種別コードです。<br> このフィールドは、ADD時に必須となり、SET時に省略可能となり、REMOVE時に無視されます。</div> 

**`memberof`** FeedItemServiceLocation
