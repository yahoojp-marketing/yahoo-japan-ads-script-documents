# AdGroupAdServiceResponsiveImageAd


<div lang=\"ja\"> AdGroupAdServiceResponsiveImageAdオブジェクトは、レスポンシブ広告の情報を表します。<br> このフィールドは、省略可能となります。<br> ※ADD時、adTypeがRESPONSIVE_IMAGE_ADの場合は必須です。 </div> 

## Table of contents

### Properties

- [buttonText](adgroupadserviceresponsiveimagead.md#buttontext)
- [description](adgroupadserviceresponsiveimagead.md#description)
- [displayUrl](adgroupadserviceresponsiveimagead.md#displayurl)
- [headline](adgroupadserviceresponsiveimagead.md#headline)
- [isRemoveLogoMediaId](adgroupadserviceresponsiveimagead.md#isremovelogomediaid)
- [logoMediaId](adgroupadserviceresponsiveimagead.md#logomediaid)
- [principal](adgroupadserviceresponsiveimagead.md#principal)
- [url](adgroupadserviceresponsiveimagead.md#url)

## Properties

### buttonText

• `Optional` **buttonText**: ``null`` \| [*ForMoreInfo*](./enums/adgroupadservicebuttontext.md#formoreinfo) \| [*ConfirmNow*](./enums/adgroupadservicebuttontext.md#confirmnow) \| [*ApplyHere*](./enums/adgroupadservicebuttontext.md#applyhere) \| [*Purchase*](./enums/adgroupadservicebuttontext.md#purchase) \| [*Experience*](./enums/adgroupadservicebuttontext.md#experience) \| [*ConfirmProperty*](./enums/adgroupadservicebuttontext.md#confirmproperty) \| [*RequestInfo*](./enums/adgroupadservicebuttontext.md#requestinfo) \| [*Download*](./enums/adgroupadservicebuttontext.md#download) \| [*Install*](./enums/adgroupadservicebuttontext.md#install) \| [*MoreDetail*](./enums/adgroupadservicebuttontext.md#moredetail) \| [*ReserveHere*](./enums/adgroupadservicebuttontext.md#reservehere) \| [*Register*](./enums/adgroupadservicebuttontext.md#register) \| [*ApplyNow*](./enums/adgroupadservicebuttontext.md#applynow) \| [*PurchaseNow*](./enums/adgroupadservicebuttontext.md#purchasenow) \| [*ReserveNow*](./enums/adgroupadservicebuttontext.md#reservenow) \| [*RegisterNow*](./enums/adgroupadservicebuttontext.md#registernow) \| [*ContactUs*](./enums/adgroupadservicebuttontext.md#contactus) \| [*Unknown*](./enums/adgroupadservicebuttontext.md#unknown)

**`memberof`** AdGroupAdServiceResponsiveImageAd

___

### description

• `Optional` **description**: ``null`` \| *string*

<div lang=\"ja\"> 説明文です。<br> このフィールドは、ADD時は必須となり、SET時は省略可能となります。 </div> 

**`memberof`** AdGroupAdServiceResponsiveImageAd

___

### displayUrl

• `Optional` **displayUrl**: ``null`` \| *string*

<div lang=\"ja\"> 表示URLです。<br> ADDおよびSET時、このフィールドは省略可能となります。<br> ・標準キャンペーンの場合<br> &nbsp;&nbsp;ADDでは入力必須です。SETでの入力は任意です。<br> ・アプリキャンペーンの場合<br> &nbsp;&nbsp;ADD、SETのどちらも指定できません。<br> &nbsp;&nbsp;※アプリキャンペーンで指定したDeviceOsTypeに基づき、以下のいずれかのURLが自動で設定されます。<br> &nbsp;&nbsp;&nbsp;&nbsp;- iOSの場合：itunes.apple.com<br> &nbsp;&nbsp;&nbsp;&nbsp;- Androidの場合：play.google.com<br> </div> 

**`memberof`** AdGroupAdServiceResponsiveImageAd

___

### headline

• `Optional` **headline**: ``null`` \| *string*

<div lang=\"ja\"> タイトルです。<br> このフィールドは、ADD時は必須となり、SET時は省略可能となります。 </div> 

**`memberof`** AdGroupAdServiceResponsiveImageAd

___

### isRemoveLogoMediaId

• `Optional` **isRemoveLogoMediaId**: ``null`` \| [*True*](./enums/adgroupadserviceisremoveflg.md#true) \| [*False*](./enums/adgroupadserviceisremoveflg.md#false) \| [*Unknown*](./enums/adgroupadserviceisremoveflg.md#unknown)

**`memberof`** AdGroupAdServiceResponsiveImageAd

___

### logoMediaId

• `Optional` **logoMediaId**: ``null`` \| *number*

<div lang=\"ja\"> ロゴ画像のメディアIDです。<br> ADDおよびSET時、このフィールドは省略可能となります。 </div> 

**`memberof`** AdGroupAdServiceResponsiveImageAd

___

### principal

• `Optional` **principal**: ``null`` \| *string*

<div lang=\"ja\"> 広告の主体者表記です。<br> このフィールドは、ADD時は必須となり、SET時は省略可能となります。 </div> 

**`memberof`** AdGroupAdServiceResponsiveImageAd

___

### url

• `Optional` **url**: ``null`` \| *string*

<div lang=\"ja\"> リンク先URLです。<br> このフィールドは、ADD時は必須となり、SET時は省略可能となります。 </div> 

**`memberof`** AdGroupAdServiceResponsiveImageAd
