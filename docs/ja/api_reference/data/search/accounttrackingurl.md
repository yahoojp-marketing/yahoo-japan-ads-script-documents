# AccountTrackingUrl


<div lang=\"ja\">AccountTrackingUrlオブジェクトは、アカウントトラッキングの情報を表します。</div> 

## Table of contents

### Properties

- [accountId](accounttrackingurl.md#accountid)
- [accountName](accounttrackingurl.md#accountname)
- [disapprovalReasonCodes](accounttrackingurl.md#disapprovalreasoncodes)
- [disapprovalReviewUrl](accounttrackingurl.md#disapprovalreviewurl)
- [inReviewUrl](accounttrackingurl.md#inreviewurl)
- [trackingUrl](accounttrackingurl.md#trackingurl)
- [urlApprovalStatus](accounttrackingurl.md#urlapprovalstatus)

## Properties

### accountId

• `Optional` **accountId**: ``null`` \| *number*

<div lang=\"ja\">アカウントIDです。<br> SET時、このフィールドは必須となります。</div> 

**`memberof`** AccountTrackingUrl

___

### accountName

• `Optional` **accountName**: ``null`` \| *string*

<div lang=\"ja\">アカウント名です。</div> 

**`memberof`** AccountTrackingUrl

___

### disapprovalReasonCodes

• `Optional` **disapprovalReasonCodes**: ``null`` \| *string*[]

<div lang=\"ja\">審査否認理由コードです。</div> 

**`memberof`** AccountTrackingUrl

___

### disapprovalReviewUrl

• `Optional` **disapprovalReviewUrl**: ``null`` \| *string*

<div lang=\"ja\">審査否認されたトラッキングURLです。</div> 

**`memberof`** AccountTrackingUrl

___

### inReviewUrl

• `Optional` **inReviewUrl**: ``null`` \| *string*

<div lang=\"ja\">審査中のトラッキングURLです。</div> 

**`memberof`** AccountTrackingUrl

___

### trackingUrl

• `Optional` **trackingUrl**: ``null`` \| *string*

<div lang=\"ja\">トラッキングURLです。<br> SET時、このフィールドは省略可能となります。<br> ※空で設定すると、既存のトラッキングURLは削除されます。</div> 

**`memberof`** AccountTrackingUrl

___

### urlApprovalStatus

• `Optional` **urlApprovalStatus**: ``null`` \| [*None*](./enums/accounttrackingurlserviceurlapprovalstatus.md#none) \| [*Approved*](./enums/accounttrackingurlserviceurlapprovalstatus.md#approved) \| [*ApprovedWithReview*](./enums/accounttrackingurlserviceurlapprovalstatus.md#approvedwithreview) \| [*Review*](./enums/accounttrackingurlserviceurlapprovalstatus.md#review) \| [*Disapproved*](./enums/accounttrackingurlserviceurlapprovalstatus.md#disapproved) \| [*Unknown*](./enums/accounttrackingurlserviceurlapprovalstatus.md#unknown)

**`memberof`** AccountTrackingUrl
