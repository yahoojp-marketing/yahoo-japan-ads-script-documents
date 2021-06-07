# FeedItem


<div lang=\"ja\">FeedItemオブジェクトは、フィードアイテム情報を格納します。</div> 

## Table of contents

### Properties

- [accountId](feeditem.md#accountid)
- [approvalStatus](feeditem.md#approvalstatus)
- [customParameters](feeditem.md#customparameters)
- [devicePreference](feeditem.md#devicepreference)
- [disapprovalReasonCodes](feeditem.md#disapprovalreasoncodes)
- [endDate](feeditem.md#enddate)
- [feedId](feeditem.md#feedid)
- [feedItemAttribute](feeditem.md#feeditemattribute)
- [feedItemId](feeditem.md#feeditemid)
- [feedItemTrackId](feeditem.md#feeditemtrackid)
- [invalidedTrademarks](feeditem.md#invalidedtrademarks)
- [location](feeditem.md#location)
- [placeholderType](feeditem.md#placeholdertype)
- [reviewCustomParameters](feeditem.md#reviewcustomparameters)
- [scheduling](feeditem.md#scheduling)
- [startDate](feeditem.md#startdate)
- [targetingAdGroup](feeditem.md#targetingadgroup)
- [targetingCampaign](feeditem.md#targetingcampaign)
- [targetingKeyword](feeditem.md#targetingkeyword)
- [trademarkStatus](feeditem.md#trademarkstatus)

## Properties

### accountId

• `Optional` **accountId**: ``null`` \| *number*

<div lang=\"ja\">アカウントIDです。<br> このフィールドは、レスポンスの際に返却されますが、リクエストの際には無視されます。</div> 

**`memberof`** FeedItem

___

### approvalStatus

• `Optional` **approvalStatus**: ``null`` \| [*Approved*](./enums/feeditemserviceapprovalstatus.md#approved) \| [*ApprovedWithReview*](./enums/feeditemserviceapprovalstatus.md#approvedwithreview) \| [*Review*](./enums/feeditemserviceapprovalstatus.md#review) \| [*PreDisapproved*](./enums/feeditemserviceapprovalstatus.md#predisapproved) \| [*PostDisapproved*](./enums/feeditemserviceapprovalstatus.md#postdisapproved) \| [*Unknown*](./enums/feeditemserviceapprovalstatus.md#unknown)

**`memberof`** FeedItem

___

### customParameters

• `Optional` **customParameters**: ``null`` \| [*FeedItemServiceCustomParameters*](feeditemservicecustomparameters.md)

**`memberof`** FeedItem

___

### devicePreference

• `Optional` **devicePreference**: ``null`` \| [*SmartPhone*](./enums/feeditemservicedevicepreference.md#smartphone) \| [*None*](./enums/feeditemservicedevicepreference.md#none) \| [*Unknown*](./enums/feeditemservicedevicepreference.md#unknown)

**`memberof`** FeedItem

___

### disapprovalReasonCodes

• `Optional` **disapprovalReasonCodes**: ``null`` \| *string*[]

<div lang=\"ja\">審査否認理由です。<br> このフィールドは、レスポンスの際に返却されますが、リクエストの際には無視されます。</div> 

**`memberof`** FeedItem

___

### endDate

• `Optional` **endDate**: ``null`` \| *string*

<div lang=\"ja\">配信終了日です。<br>※空で設定すると、既存の配信終了日は削除されます。<br> このフィールドは、ADDおよびSET時に省略可能となり、REMOVE時に無視されます。</div> 

**`memberof`** FeedItem

___

### feedId

• `Optional` **feedId**: ``null`` \| *number*

<div lang=\"ja\">フィードIDです。<br> このフィールドはレスポンスの際に返却されますが、リクエストの際には無視されます。<br> ※アドカスタマイザーの場合は、ADD時に必須となります。</div> 

**`memberof`** FeedItem

___

### feedItemAttribute

• `Optional` **feedItemAttribute**: ``null`` \| [*FeedItemServiceAttribute*](feeditemserviceattribute.md)[]

**`memberof`** FeedItem

___

### feedItemId

• `Optional` **feedItemId**: ``null`` \| *number*

<div lang=\"ja\">フィードアイテムIDです。<br> このフィールドは、SETおよびREMOVE時に必須となり、ADD時に無視されます。</div> 

**`memberof`** FeedItem

___

### feedItemTrackId

• `Optional` **feedItemTrackId**: ``null`` \| *number*

<div lang=\"ja\">トラッキング用フィードアイテムIDです。<br> このフィールドは、レスポンスの際に返却されますが、リクエストの際には無視されます。</div> 

**`memberof`** FeedItem

___

### invalidedTrademarks

• `Optional` **invalidedTrademarks**: ``null`` \| *string*[]

<div lang=\"ja\">制限された商標です。<br> このフィールドは、レスポンスの際に返却されますが、リクエストの際には無視されます。 </div> 

**`memberof`** FeedItem

___

### location

• `Optional` **location**: ``null`` \| [*FeedItemServiceLocation*](feeditemservicelocation.md)

**`memberof`** FeedItem

___

### placeholderType

• `Optional` **placeholderType**: ``null`` \| [*Quicklink*](./enums/feeditemserviceplaceholdertype.md#quicklink) \| [*Callextension*](./enums/feeditemserviceplaceholdertype.md#callextension) \| [*AdCustomizer*](./enums/feeditemserviceplaceholdertype.md#adcustomizer) \| [*Callout*](./enums/feeditemserviceplaceholdertype.md#callout) \| [*StructuredSnippet*](./enums/feeditemserviceplaceholdertype.md#structuredsnippet) \| [*Unknown*](./enums/feeditemserviceplaceholdertype.md#unknown)

**`memberof`** FeedItem

___

### reviewCustomParameters

• `Optional` **reviewCustomParameters**: ``null`` \| [*FeedItemServiceCustomParameters*](feeditemservicecustomparameters.md)

**`memberof`** FeedItem

___

### scheduling

• `Optional` **scheduling**: ``null`` \| [*FeedItemServiceScheduling*](feeditemservicescheduling.md)

**`memberof`** FeedItem

___

### startDate

• `Optional` **startDate**: ``null`` \| *string*

<div lang=\"ja\">配信開始日です。<br> ※空で設定すると、既存の配信開始日は削除されます。<br> このフィールドは、ADDおよびSET時に省略可能となり、REMOVE時に無視されます。</div> 

**`memberof`** FeedItem

___

### targetingAdGroup

• `Optional` **targetingAdGroup**: ``null`` \| [*FeedItemServiceTargetingAdGroup*](feeditemservicetargetingadgroup.md)

**`memberof`** FeedItem

___

### targetingCampaign

• `Optional` **targetingCampaign**: ``null`` \| [*FeedItemServiceTargetingCampaign*](feeditemservicetargetingcampaign.md)

**`memberof`** FeedItem

___

### targetingKeyword

• `Optional` **targetingKeyword**: ``null`` \| [*FeedItemServiceTargetingKeyword*](feeditemservicetargetingkeyword.md)

**`memberof`** FeedItem

___

### trademarkStatus

• `Optional` **trademarkStatus**: ``null`` \| [*NoRestriction*](./enums/feeditemservicetrademarkstatus.md#norestriction) \| [*ConflictWithTrademark*](./enums/feeditemservicetrademarkstatus.md#conflictwithtrademark) \| [*ClaimInProgress*](./enums/feeditemservicetrademarkstatus.md#claiminprogress) \| [*DisapprovedClaim*](./enums/feeditemservicetrademarkstatus.md#disapprovedclaim) \| [*DisapprovedReviewer*](./enums/feeditemservicetrademarkstatus.md#disapprovedreviewer) \| [*Unknown*](./enums/feeditemservicetrademarkstatus.md#unknown)

**`memberof`** FeedItem
