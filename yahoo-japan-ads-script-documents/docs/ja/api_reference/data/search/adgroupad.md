# AdGroupAd


<div lang=\"ja\">AdGroupAdオブジェクトは、広告に関する操作を行うための情報を表します。</div> 

## Table of contents

### Properties

- [accountId](adgroupad.md#accountid)
- [ad](adgroupad.md#ad)
- [adGroupId](adgroupad.md#adgroupid)
- [adGroupName](adgroupad.md#adgroupname)
- [adGroupTrackId](adgroupad.md#adgrouptrackid)
- [adId](adgroupad.md#adid)
- [adName](adgroupad.md#adname)
- [adTrackId](adgroupad.md#adtrackid)
- [approvalStatus](adgroupad.md#approvalstatus)
- [campaignId](adgroupad.md#campaignid)
- [campaignName](adgroupad.md#campaignname)
- [campaignTrackId](adgroupad.md#campaigntrackid)
- [createdDate](adgroupad.md#createddate)
- [disapprovalReasonCodes](adgroupad.md#disapprovalreasoncodes)
- [feedId](adgroupad.md#feedid)
- [invalidedTrademarks](adgroupad.md#invalidedtrademarks)
- [labels](adgroupad.md#labels)
- [trademarkStatus](adgroupad.md#trademarkstatus)
- [userStatus](adgroupad.md#userstatus)

## Properties

### accountId

• `Optional` **accountId**: ``null`` \| *number*

<div lang=\"ja\">アカウントIDです。<br> このフィールドは、レスポンスの際に返却されますが、リクエストの際には無視されます。</div> 

**`memberof`** AdGroupAd

___

### ad

• `Optional` **ad**: ``null`` \| [*AdGroupAdServiceAd*](adgroupadservicead.md)

**`memberof`** AdGroupAd

___

### adGroupId

• `Optional` **adGroupId**: ``null`` \| *number*

<div lang=\"ja\">広告グループIDです。<br> このフィールドは、いずれの場合でも必須となります。</div> 

**`memberof`** AdGroupAd

___

### adGroupName

• `Optional` **adGroupName**: ``null`` \| *string*

<div lang=\"ja\">広告グループ名です。<br> このフィールドは、レスポンスの際に返却されますが、リクエストの際には無視されます。</div> 

**`memberof`** AdGroupAd

___

### adGroupTrackId

• `Optional` **adGroupTrackId**: ``null`` \| *number*

<div lang=\"ja\">トラッキング用広告グループIDです。<br> このフィールドは、レスポンスの際に返却されますが、リクエストの際には無視されます。</div> 

**`memberof`** AdGroupAd

___

### adId

• `Optional` **adId**: ``null`` \| *number*

<div lang=\"ja\">広告IDです。<br> SETおよびREMOVE時、このフィールドは必須となります。</div> 

**`memberof`** AdGroupAd

___

### adName

• `Optional` **adName**: ``null`` \| *string*

<div lang=\"ja\">広告名です。<br> このフィールドは、ADD時は必須となり、SET時は省略可能となります。</div> 

**`memberof`** AdGroupAd

___

### adTrackId

• `Optional` **adTrackId**: ``null`` \| *number*

<div lang=\"ja\">トラッキング用広告IDです。<br> このフィールドは、レスポンスの際に返却されますが、リクエストの際には無視されます。</div> 

**`memberof`** AdGroupAd

___

### approvalStatus

• `Optional` **approvalStatus**: ``null`` \| [*Approved*](./enums/adgroupadserviceapprovalstatus.md#approved) \| [*ApprovedWithReview*](./enums/adgroupadserviceapprovalstatus.md#approvedwithreview) \| [*Review*](./enums/adgroupadserviceapprovalstatus.md#review) \| [*PreDisapproved*](./enums/adgroupadserviceapprovalstatus.md#predisapproved) \| [*PostDisapproved*](./enums/adgroupadserviceapprovalstatus.md#postdisapproved) \| [*Unknown*](./enums/adgroupadserviceapprovalstatus.md#unknown)

**`memberof`** AdGroupAd

___

### campaignId

• `Optional` **campaignId**: ``null`` \| *number*

<div lang=\"ja\">キャンペーンIDです。<br> このフィールドは、いずれの場合でも必須となります。</div> 

**`memberof`** AdGroupAd

___

### campaignName

• `Optional` **campaignName**: ``null`` \| *string*

<div lang=\"ja\">キャンペーン名です。<br> このフィールドは、レスポンスの際に返却されますが、リクエストの際には無視されます。</div> 

**`memberof`** AdGroupAd

___

### campaignTrackId

• `Optional` **campaignTrackId**: ``null`` \| *number*

<div lang=\"ja\">トラッキング用キャンペーンIDです。<br> このフィールドは、レスポンスの際に返却されますが、リクエストの際には無視されます。</div> 

**`memberof`** AdGroupAd

___

### createdDate

• `Optional` **createdDate**: ``null`` \| *string*

<div lang=\"ja\">広告が作成された日です。<br>※フォーマット：yyyyMMdd</div> 

**`memberof`** AdGroupAd

___

### disapprovalReasonCodes

• `Optional` **disapprovalReasonCodes**: ``null`` \| *string*[]

<div lang=\"ja\">審査否認の理由コードです。<br> (コード詳細は、DictionaryServiceのgetDisapprovalReasonのレスポンスを参照)<br> このフィールドは、レスポンスの際に返却されますが、リクエストの際には無視されます。</div> 

**`memberof`** AdGroupAd

___

### feedId

• `Optional` **feedId**: ``null`` \| *number*

<div lang=\"ja\">フィードIDです。<br> このフィールドは、レスポンスの際に返却されますが、リクエストの際には無視されます。</div> 

**`memberof`** AdGroupAd

___

### invalidedTrademarks

• `Optional` **invalidedTrademarks**: ``null`` \| *string*[]

<div lang=\"ja\">制限された商標です。<br> このフィールドは、レスポンスの際に返却されますが、リクエストの際には無視されます。</div> 

**`memberof`** AdGroupAd

___

### labels

• `Optional` **labels**: ``null`` \| [*AdGroupAdServiceLabel*](adgroupadservicelabel.md)[]

**`memberof`** AdGroupAd

___

### trademarkStatus

• `Optional` **trademarkStatus**: ``null`` \| [*NoRestriction*](./enums/adgroupadservicetrademarkstatus.md#norestriction) \| [*ConflictWithTrademark*](./enums/adgroupadservicetrademarkstatus.md#conflictwithtrademark) \| [*ClaimInProgress*](./enums/adgroupadservicetrademarkstatus.md#claiminprogress) \| [*DisapprovedClaim*](./enums/adgroupadservicetrademarkstatus.md#disapprovedclaim) \| [*DisapprovedReviewer*](./enums/adgroupadservicetrademarkstatus.md#disapprovedreviewer) \| [*Unknown*](./enums/adgroupadservicetrademarkstatus.md#unknown)

**`memberof`** AdGroupAd

___

### userStatus

• `Optional` **userStatus**: ``null`` \| [*Active*](./enums/adgroupadserviceuserstatus.md#active) \| [*Paused*](./enums/adgroupadserviceuserstatus.md#paused) \| [*Unknown*](./enums/adgroupadserviceuserstatus.md#unknown)

**`memberof`** AdGroupAd
