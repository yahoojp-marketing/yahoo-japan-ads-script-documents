# GuaranteedAdGroupAd


<div lang=\"ja\"> GuaranteedAdGroupAdオブジェクトは、予約型の広告の情報を格納するコンテナです。<br> 各広告で設定可能な項目については、<a href=\"https://ads-help.yahoo.co.jp/yahooads/rf/articledetail?lan=ja&aid=103055&o=default\">予約型の広告の種類</a>をご参照ください。 </div> 

## Table of contents

### Properties

- [accountId](guaranteedadgroupad.md#accountid)
- [ad](guaranteedadgroupad.md#ad)
- [adGroupId](guaranteedadgroupad.md#adgroupid)
- [adGroupName](guaranteedadgroupad.md#adgroupname)
- [adId](guaranteedadgroupad.md#adid)
- [adName](guaranteedadgroupad.md#adname)
- [adStyle](guaranteedadgroupad.md#adstyle)
- [approvalStatus](guaranteedadgroupad.md#approvalstatus)
- [campaignId](guaranteedadgroupad.md#campaignid)
- [campaignName](guaranteedadgroupad.md#campaignname)
- [disapprovalReasonCodes](guaranteedadgroupad.md#disapprovalreasoncodes)
- [disapprovalReasonDescription](guaranteedadgroupad.md#disapprovalreasondescription)
- [impressionBeaconUrls](guaranteedadgroupad.md#impressionbeaconurls)
- [isRemoveBeaconUrls](guaranteedadgroupad.md#isremovebeaconurls)
- [isRemoveImpressionBeaconUrls](guaranteedadgroupad.md#isremoveimpressionbeaconurls)
- [isRemoveThirdPartyTrackingScriptUrl](guaranteedadgroupad.md#isremovethirdpartytrackingscripturl)
- [isRemoveViewableImpressionBeaconUrls](guaranteedadgroupad.md#isremoveviewableimpressionbeaconurls)
- [labels](guaranteedadgroupad.md#labels)
- [landingPageStatus](guaranteedadgroupad.md#landingpagestatus)
- [landingPageUpdateScheduledTime](guaranteedadgroupad.md#landingpageupdatescheduledtime)
- [mediaId](guaranteedadgroupad.md#mediaid)
- [preApprovalId](guaranteedadgroupad.md#preapprovalid)
- [thirdPartyTrackingScriptUrl](guaranteedadgroupad.md#thirdpartytrackingscripturl)
- [thirdPartyTrackingVendor](guaranteedadgroupad.md#thirdpartytrackingvendor)
- [userStatus](guaranteedadgroupad.md#userstatus)
- [viewableImpressionBeaconUrls](guaranteedadgroupad.md#viewableimpressionbeaconurls)

## Properties

### accountId

• `Optional` **accountId**: ``null`` \| *number*

<div lang=\"ja\"> アカウントIDです。<br> このフィールドは、レスポンスの際に返却されますが、リクエストの際には無視されます。 </div> 

**`memberof`** GuaranteedAdGroupAd

___

### ad

• `Optional` **ad**: ``null`` \| [*GuaranteedAdGroupAdServiceAd*](guaranteedadgroupadservicead.md)

**`memberof`** GuaranteedAdGroupAd

___

### adGroupId

• `Optional` **adGroupId**: ``null`` \| *number*

<div lang=\"ja\"> 広告グループIDです。<br> このフィールドは、リクエストの場合は必須です。 </div> 

**`memberof`** GuaranteedAdGroupAd

___

### adGroupName

• `Optional` **adGroupName**: ``null`` \| *string*

<div lang=\"ja\"> 広告グループ名です。<br> このフィールドは、レスポンスの際に返却されますが、リクエストの際には無視されます。 </div> 

**`memberof`** GuaranteedAdGroupAd

___

### adId

• `Optional` **adId**: ``null`` \| *number*

<div lang=\"ja\"> 広告IDです。<br> このフィールドは、ADD時は無視され、SET時に必須となります。 </div> 

**`memberof`** GuaranteedAdGroupAd

___

### adName

• `Optional` **adName**: ``null`` \| *string*

<div lang=\"ja\"> 広告名です。<br> このフィールドは、ADD時は必須となり、SET時は省略可能となります。 </div> 

**`memberof`** GuaranteedAdGroupAd

___

### adStyle

• `Optional` **adStyle**: ``null`` \| [*Image*](./enums/guaranteedadgroupadserviceadstyle.md#image) \| [*Video*](./enums/guaranteedadgroupadserviceadstyle.md#video) \| [*Unknown*](./enums/guaranteedadgroupadserviceadstyle.md#unknown)

**`memberof`** GuaranteedAdGroupAd

___

### approvalStatus

• `Optional` **approvalStatus**: ``null`` \| [*Approved*](./enums/guaranteedadgroupadserviceapprovalstatus.md#approved) \| [*ApprovedWithReview*](./enums/guaranteedadgroupadserviceapprovalstatus.md#approvedwithreview) \| [*Review*](./enums/guaranteedadgroupadserviceapprovalstatus.md#review) \| [*PreDisapproved*](./enums/guaranteedadgroupadserviceapprovalstatus.md#predisapproved) \| [*PostDisapproved*](./enums/guaranteedadgroupadserviceapprovalstatus.md#postdisapproved) \| [*Unknown*](./enums/guaranteedadgroupadserviceapprovalstatus.md#unknown)

**`memberof`** GuaranteedAdGroupAd

___

### campaignId

• `Optional` **campaignId**: ``null`` \| *number*

<div lang=\"ja\"> キャンペーンIDです。<br> このフィールドは、リクエストの場合は必須です。 </div> 

**`memberof`** GuaranteedAdGroupAd

___

### campaignName

• `Optional` **campaignName**: ``null`` \| *string*

<div lang=\"ja\"> キャンペーン名です。<br> このフィールドは、レスポンスの際に返却されますが、リクエストの際には無視されます。 </div> 

**`memberof`** GuaranteedAdGroupAd

___

### disapprovalReasonCodes

• `Optional` **disapprovalReasonCodes**: ``null`` \| *string*[]

<div lang=\"ja\"> 掲載拒否の理由です。<br> このフィールドは、レスポンスの際に返却されますが、リクエストの際には無視されます。 </div> 

**`memberof`** GuaranteedAdGroupAd

___

### disapprovalReasonDescription

• `Optional` **disapprovalReasonDescription**: ``null`` \| *string*

<div lang=\"ja\"> 掲載拒否の理由詳細です。<br> このフィールドは、レスポンスの際に返却されますが、リクエストの際には無視されます。 </div> 

**`memberof`** GuaranteedAdGroupAd

___

### impressionBeaconUrls

• `Optional` **impressionBeaconUrls**: ``null`` \| *string*[]

<div lang=\"ja\"> インプレッションビーコンURLです。<br> ADDおよびSET時、このフィールドは省略可能となります。 </div> 

**`memberof`** GuaranteedAdGroupAd

___

### isRemoveBeaconUrls

• `Optional` **isRemoveBeaconUrls**: ``null`` \| [*True*](./enums/guaranteedadgroupadserviceisremoveflg.md#true) \| [*False*](./enums/guaranteedadgroupadserviceisremoveflg.md#false) \| [*Unknown*](./enums/guaranteedadgroupadserviceisremoveflg.md#unknown)

**`memberof`** GuaranteedAdGroupAd

___

### isRemoveImpressionBeaconUrls

• `Optional` **isRemoveImpressionBeaconUrls**: ``null`` \| [*True*](./enums/guaranteedadgroupadserviceisremoveflg.md#true) \| [*False*](./enums/guaranteedadgroupadserviceisremoveflg.md#false) \| [*Unknown*](./enums/guaranteedadgroupadserviceisremoveflg.md#unknown)

**`memberof`** GuaranteedAdGroupAd

___

### isRemoveThirdPartyTrackingScriptUrl

• `Optional` **isRemoveThirdPartyTrackingScriptUrl**: ``null`` \| [*True*](./enums/guaranteedadgroupadserviceisremoveflg.md#true) \| [*False*](./enums/guaranteedadgroupadserviceisremoveflg.md#false) \| [*Unknown*](./enums/guaranteedadgroupadserviceisremoveflg.md#unknown)

**`memberof`** GuaranteedAdGroupAd

___

### isRemoveViewableImpressionBeaconUrls

• `Optional` **isRemoveViewableImpressionBeaconUrls**: ``null`` \| [*True*](./enums/guaranteedadgroupadserviceisremoveflg.md#true) \| [*False*](./enums/guaranteedadgroupadserviceisremoveflg.md#false) \| [*Unknown*](./enums/guaranteedadgroupadserviceisremoveflg.md#unknown)

**`memberof`** GuaranteedAdGroupAd

___

### labels

• `Optional` **labels**: ``null`` \| [*GuaranteedAdGroupAdServiceLabel*](guaranteedadgroupadservicelabel.md)[]

**`memberof`** GuaranteedAdGroupAd

___

### landingPageStatus

• `Optional` **landingPageStatus**: ``null`` \| [*Completed*](./enums/guaranteedadgroupadlandingpagestatus.md#completed) \| [*SpecifiedUpdateScheduledTime*](./enums/guaranteedadgroupadlandingpagestatus.md#specifiedupdatescheduledtime) \| [*Unknown*](./enums/guaranteedadgroupadlandingpagestatus.md#unknown)

**`memberof`** GuaranteedAdGroupAd

___

### landingPageUpdateScheduledTime

• `Optional` **landingPageUpdateScheduledTime**: ``null`` \| *string*

<div lang=\"ja\"> リンク先更新予定日時です。<br> ※フォーマット：yyyyMMddHHmm<br> ※landingPageStatusがSPECIFIED_UPDATE_SCHEDULED_TIMEの場合は必須です。 </div> 

**`memberof`** GuaranteedAdGroupAd

___

### mediaId

• `Optional` **mediaId**: ``null`` \| *number*

<div lang=\"ja\"> メディアIDです。<br> ADDおよびSET時、このフィールドは省略可能となります。 </div> 

**`memberof`** GuaranteedAdGroupAd

___

### preApprovalId

• `Optional` **preApprovalId**: ``null`` \| *string*

<div lang=\"ja\"> 事前承認ID（数字のみ）です。<br> </div> 

**`memberof`** GuaranteedAdGroupAd

___

### thirdPartyTrackingScriptUrl

• `Optional` **thirdPartyTrackingScriptUrl**: ``null`` \| *string*

<div lang=\"ja\"> 第三者計測スクリプトURLです。<br> ADDおよびSET時、このフィールドは省略可能となります。 </div> 

**`memberof`** GuaranteedAdGroupAd

___

### thirdPartyTrackingVendor

• `Optional` **thirdPartyTrackingVendor**: ``null`` \| *string*

<div lang=\"ja\"> 第三者計測ベンダー（ReadOnly）です。<br> thirdPartyTrackingScriptUrlのドメインに基づく第三者計測ベンダーが設定されます。<br> このフィールドは、レスポンスの際に返却されますが、リクエストの際には無視されます。 </div> 

**`memberof`** GuaranteedAdGroupAd

___

### userStatus

• `Optional` **userStatus**: ``null`` \| [*Active*](./enums/guaranteedadgroupadserviceuserstatus.md#active) \| [*Paused*](./enums/guaranteedadgroupadserviceuserstatus.md#paused) \| [*Unknown*](./enums/guaranteedadgroupadserviceuserstatus.md#unknown)

**`memberof`** GuaranteedAdGroupAd

___

### viewableImpressionBeaconUrls

• `Optional` **viewableImpressionBeaconUrls**: ``null`` \| *string*[]

<div lang=\"ja\"> ビューアブルインプレッションビーコンURLです。<br> ADDおよびSET時、このフィールドは省略可能となります。 </div> 

**`memberof`** GuaranteedAdGroupAd
