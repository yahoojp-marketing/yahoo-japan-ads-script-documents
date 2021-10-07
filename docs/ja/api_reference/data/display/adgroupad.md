# AdGroupAd


<div lang=\"ja\">AdGroupAdオブジェクトは、広告の情報を格納するコンテナです。</div> 

## Table of contents

### Properties

- [accountId](adgroupad.md#accountid)
- [ad](adgroupad.md#ad)
- [adGroupId](adgroupad.md#adgroupid)
- [adGroupName](adgroupad.md#adgroupname)
- [adId](adgroupad.md#adid)
- [adName](adgroupad.md#adname)
- [adStyle](adgroupad.md#adstyle)
- [approvalStatus](adgroupad.md#approvalstatus)
- [campaignId](adgroupad.md#campaignid)
- [campaignName](adgroupad.md#campaignname)
- [createdDate](adgroupad.md#createddate)
- [disapprovalReasonCodes](adgroupad.md#disapprovalreasoncodes)
- [disapprovalReasonDescription](adgroupad.md#disapprovalreasondescription)
- [impressionBeaconUrls](adgroupad.md#impressionbeaconurls)
- [isRemoveImpressionBeaconUrls](adgroupad.md#isremoveimpressionbeaconurls)
- [isRemoveThirdPartyTrackingScriptUrl](adgroupad.md#isremovethirdpartytrackingscripturl)
- [isRemoveViewableImpressionBeaconUrls](adgroupad.md#isremoveviewableimpressionbeaconurls)
- [labels](adgroupad.md#labels)
- [mediaId](adgroupad.md#mediaid)
- [thirdPartyTrackingScriptUrl](adgroupad.md#thirdpartytrackingscripturl)
- [thirdPartyTrackingVendor](adgroupad.md#thirdpartytrackingvendor)
- [userStatus](adgroupad.md#userstatus)
- [viewableImpressionBeaconUrls](adgroupad.md#viewableimpressionbeaconurls)

## Properties

### accountId

• `Optional` **accountId**: ``null`` \| *number*

<div lang=\"ja\"> アカウントIDです。<br> このフィールドは、リクエストの場合は必須です。 </div> 

**`memberof`** AdGroupAd

___

### ad

• `Optional` **ad**: ``null`` \| [*AdGroupAdServiceAd*](adgroupadservicead.md)

**`memberof`** AdGroupAd

___

### adGroupId

• `Optional` **adGroupId**: ``null`` \| *number*

<div lang=\"ja\"> 広告グループIDです。<br> このフィールドは、リクエストの場合は必須です。 </div> 

**`memberof`** AdGroupAd

___

### adGroupName

• `Optional` **adGroupName**: ``null`` \| *string*

<div lang=\"ja\"> 広告グループ名です。<br> このフィールドは、レスポンスの際に返却されますが、リクエストの際には無視されます。 </div> 

**`memberof`** AdGroupAd

___

### adId

• `Optional` **adId**: ``null`` \| *number*

<div lang=\"ja\"> 広告IDです。<br> このフィールドは、ADD時は無視され、SETおよびREMOVE時に必須となります。 </div> 

**`memberof`** AdGroupAd

___

### adName

• `Optional` **adName**: ``null`` \| *string*

<div lang=\"ja\"> 広告名です。<br> このフィールドは、ADD時は必須となり、SET時は省略可能となります。 </div> 

**`memberof`** AdGroupAd

___

### adStyle

• `Optional` **adStyle**: ``null`` \| [*Text*](./enums/adgroupadserviceadstyle.md#text) \| [*Image*](./enums/adgroupadserviceadstyle.md#image) \| [*AnimationImage*](./enums/adgroupadserviceadstyle.md#animationimage) \| [*Video*](./enums/adgroupadserviceadstyle.md#video) \| [*Unknown*](./enums/adgroupadserviceadstyle.md#unknown)

**`memberof`** AdGroupAd

___

### approvalStatus

• `Optional` **approvalStatus**: ``null`` \| [*Approved*](./enums/adgroupadserviceapprovalstatus.md#approved) \| [*ApprovedWithReview*](./enums/adgroupadserviceapprovalstatus.md#approvedwithreview) \| [*Review*](./enums/adgroupadserviceapprovalstatus.md#review) \| [*PreDisapproved*](./enums/adgroupadserviceapprovalstatus.md#predisapproved) \| [*PostDisapproved*](./enums/adgroupadserviceapprovalstatus.md#postdisapproved) \| [*Unknown*](./enums/adgroupadserviceapprovalstatus.md#unknown)

**`memberof`** AdGroupAd

___

### campaignId

• `Optional` **campaignId**: ``null`` \| *number*

<div lang=\"ja\"> キャンペーンIDです。<br> このフィールドは、リクエストの場合は必須です。 </div> 

**`memberof`** AdGroupAd

___

### campaignName

• `Optional` **campaignName**: ``null`` \| *string*

<div lang=\"ja\"> キャンペーン名です。<br> このフィールドは、レスポンスの際に返却されますが、リクエストの際には無視されます。 </div> 

**`memberof`** AdGroupAd

___

### createdDate

• `Optional` **createdDate**: ``null`` \| *string*

<div lang=\"ja\">広告が作成された日時です。<br>※フォーマット：yyyyMMdd</div> 

**`memberof`** AdGroupAd

___

### disapprovalReasonCodes

• `Optional` **disapprovalReasonCodes**: ``null`` \| *string*[]

<div lang=\"ja\"> 掲載拒否の理由です。<br> このフィールドは、レスポンスの際に返却されますが、リクエストの際には無視されます。 </div> 

**`memberof`** AdGroupAd

___

### disapprovalReasonDescription

• `Optional` **disapprovalReasonDescription**: ``null`` \| *string*

<div lang=\"ja\"> 掲載拒否の理由詳細です。<br> このフィールドは、レスポンスの際に返却されますが、リクエストの際には無視されます。 </div> 

**`memberof`** AdGroupAd

___

### impressionBeaconUrls

• `Optional` **impressionBeaconUrls**: ``null`` \| *string*[]

<div lang=\"ja\"> インプレッションビーコンURLです。<br> ADDおよびSET時、このフィールドは省略可能となります。 </div> 

**`memberof`** AdGroupAd

___

### isRemoveImpressionBeaconUrls

• `Optional` **isRemoveImpressionBeaconUrls**: ``null`` \| [*True*](./enums/adgroupadserviceisremoveflg.md#true) \| [*False*](./enums/adgroupadserviceisremoveflg.md#false) \| [*Unknown*](./enums/adgroupadserviceisremoveflg.md#unknown)

**`memberof`** AdGroupAd

___

### isRemoveThirdPartyTrackingScriptUrl

• `Optional` **isRemoveThirdPartyTrackingScriptUrl**: ``null`` \| [*True*](./enums/adgroupadserviceisremoveflg.md#true) \| [*False*](./enums/adgroupadserviceisremoveflg.md#false) \| [*Unknown*](./enums/adgroupadserviceisremoveflg.md#unknown)

**`memberof`** AdGroupAd

___

### isRemoveViewableImpressionBeaconUrls

• `Optional` **isRemoveViewableImpressionBeaconUrls**: ``null`` \| [*True*](./enums/adgroupadserviceisremoveflg.md#true) \| [*False*](./enums/adgroupadserviceisremoveflg.md#false) \| [*Unknown*](./enums/adgroupadserviceisremoveflg.md#unknown)

**`memberof`** AdGroupAd

___

### labels

• `Optional` **labels**: ``null`` \| [*AdGroupAdServiceLabel*](adgroupadservicelabel.md)[]

**`memberof`** AdGroupAd

___

### mediaId

• `Optional` **mediaId**: ``null`` \| *number*

<div lang=\"ja\"> メディアIDです。<br> ADDおよびSET時、このフィールドは省略可能となります。 </div> 

**`memberof`** AdGroupAd

___

### thirdPartyTrackingScriptUrl

• `Optional` **thirdPartyTrackingScriptUrl**: ``null`` \| *string*

<div lang=\"ja\"> 第三者計測スクリプトURLです。<br> ADDおよびSET時、このフィールドは省略可能となります。 </div> 

**`memberof`** AdGroupAd

___

### thirdPartyTrackingVendor

• `Optional` **thirdPartyTrackingVendor**: ``null`` \| *string*

<div lang=\"ja\"> 第三者計測ベンダー（ReadOnly）です。<br> thirdPartyTrackingScriptUrlのドメインに基づく第三者計測ベンダーが設定されます。<br> このフィールドは、レスポンスの際に返却されますが、リクエストの際には無視されます。 </div> 

**`memberof`** AdGroupAd

___

### userStatus

• `Optional` **userStatus**: ``null`` \| [*Active*](./enums/adgroupadserviceuserstatus.md#active) \| [*Paused*](./enums/adgroupadserviceuserstatus.md#paused) \| [*Unknown*](./enums/adgroupadserviceuserstatus.md#unknown)

**`memberof`** AdGroupAd

___

### viewableImpressionBeaconUrls

• `Optional` **viewableImpressionBeaconUrls**: ``null`` \| *string*[]

<div lang=\"ja\"> ビューアブルインプレッションビーコンURLです。<br> ADDおよびSET時、このフィールドは省略可能となります。 </div> 

**`memberof`** AdGroupAd
