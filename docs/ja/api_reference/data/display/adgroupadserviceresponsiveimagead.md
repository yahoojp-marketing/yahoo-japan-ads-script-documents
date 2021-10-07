# AdGroupAdServiceResponsiveImageAd


<div lang=\"ja\"> AdGroupAdServiceResponsiveImageAdオブジェクトは、レスポンシブ広告の情報を表します。<br> このフィールドは、省略可能となります。<br> ※ADD時、adTypeがRESPONSIVE_IMAGE_ADの場合は必須です。 </div> 

## Table of contents

### Properties

- [buttonText](adgroupadserviceresponsiveimagead.md#buttontext)
- [customParameters](adgroupadserviceresponsiveimagead.md#customparameters)
- [description](adgroupadserviceresponsiveimagead.md#description)
- [displayUrl](adgroupadserviceresponsiveimagead.md#displayurl)
- [displayUrlLevel](adgroupadserviceresponsiveimagead.md#displayurllevel)
- [finalUrl](adgroupadserviceresponsiveimagead.md#finalurl)
- [headline](adgroupadserviceresponsiveimagead.md#headline)
- [isRemoveLogoMediaId](adgroupadserviceresponsiveimagead.md#isremovelogomediaid)
- [isRemoveSmartphoneFinalUrl](adgroupadserviceresponsiveimagead.md#isremovesmartphonefinalurl)
- [isRemoveTrackingUrl](adgroupadserviceresponsiveimagead.md#isremovetrackingurl)
- [logoMediaId](adgroupadserviceresponsiveimagead.md#logomediaid)
- [principal](adgroupadserviceresponsiveimagead.md#principal)
- [smartphoneFinalUrl](adgroupadserviceresponsiveimagead.md#smartphonefinalurl)
- [trackingUrl](adgroupadserviceresponsiveimagead.md#trackingurl)
- [url](adgroupadserviceresponsiveimagead.md#url)

## Properties

### buttonText

• `Optional` **buttonText**: ``null`` \| [*ForMoreInfo*](./enums/adgroupadservicebuttontext.md#formoreinfo) \| [*ConfirmNow*](./enums/adgroupadservicebuttontext.md#confirmnow) \| [*ApplyHere*](./enums/adgroupadservicebuttontext.md#applyhere) \| [*Purchase*](./enums/adgroupadservicebuttontext.md#purchase) \| [*Experience*](./enums/adgroupadservicebuttontext.md#experience) \| [*ConfirmProperty*](./enums/adgroupadservicebuttontext.md#confirmproperty) \| [*RequestInfo*](./enums/adgroupadservicebuttontext.md#requestinfo) \| [*Download*](./enums/adgroupadservicebuttontext.md#download) \| [*Install*](./enums/adgroupadservicebuttontext.md#install) \| [*MoreDetail*](./enums/adgroupadservicebuttontext.md#moredetail) \| [*ReserveHere*](./enums/adgroupadservicebuttontext.md#reservehere) \| [*Register*](./enums/adgroupadservicebuttontext.md#register) \| [*ApplyNow*](./enums/adgroupadservicebuttontext.md#applynow) \| [*PurchaseNow*](./enums/adgroupadservicebuttontext.md#purchasenow) \| [*ReserveNow*](./enums/adgroupadservicebuttontext.md#reservenow) \| [*RegisterNow*](./enums/adgroupadservicebuttontext.md#registernow) \| [*ContactUs*](./enums/adgroupadservicebuttontext.md#contactus) \| [*Unknown*](./enums/adgroupadservicebuttontext.md#unknown)

**`memberof`** AdGroupAdServiceResponsiveImageAd

___

### customParameters

• `Optional` **customParameters**: ``null`` \| [*AdGroupAdServiceCustomParameters*](adgroupadservicecustomparameters.md)

**`memberof`** AdGroupAdServiceResponsiveImageAd

___

### description

• `Optional` **description**: ``null`` \| *string*

<div lang=\"ja\"> 説明文です。<br> このフィールドは、ADD時は必須となり、SET時は省略可能となります。 </div> 

**`memberof`** AdGroupAdServiceResponsiveImageAd

___

### displayUrl

• `Optional` **displayUrl**: ``null`` \| *string*

<div lang=\"ja\"> 表示URLです。<br> SET時、このフィールドは省略可能となります。<br> ADD時にurlを指定する場合、このフィールドは必須です。<br> ADD時にfinalUrlを指定する場合、このフィールドを指定することはできません。代わりにfinalUrlから生成された値が自動で設定されます。<br> ただし、キャンペーン目的「アプリ訴求」の場合は、ADD、SETのどちらも指定できません。キャンペーンで指定したDeviceOsTypeに基づき、以下のいずれかのURLが自動で設定されます。<br> - iOSの場合：itunes.apple.com<br> - Androidの場合：play.google.com </div> 

**`memberof`** AdGroupAdServiceResponsiveImageAd

___

### displayUrlLevel

• `Optional` **displayUrlLevel**: ``null`` \| [*Domain*](./enums/adgroupadservicedisplayurllevel.md#domain) \| [*FirstLevel*](./enums/adgroupadservicedisplayurllevel.md#firstlevel) \| [*Unknown*](./enums/adgroupadservicedisplayurllevel.md#unknown)

**`memberof`** AdGroupAdServiceResponsiveImageAd

___

### finalUrl

• `Optional` **finalUrl**: ``null`` \| *string*

<div lang=\"ja\">最終リンク先URLです。<br> ADD時、finalUrlフィールドとurlフィールドは同時に設定することはできず、どちらか片方の設定が必須となります。<br> finalUrlフィールドを設定する場合、smartphoneFinalUrl、trackingUrl、customParametersは任意になります。<br> SET時は省略可能となります。<br> SET時にurlを指定する場合、このフィールドの値はクリアされます。 <br>※現在利用できません</div> 

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

### isRemoveSmartphoneFinalUrl

• `Optional` **isRemoveSmartphoneFinalUrl**: ``null`` \| [*True*](./enums/adgroupadserviceisremoveflg.md#true) \| [*False*](./enums/adgroupadserviceisremoveflg.md#false) \| [*Unknown*](./enums/adgroupadserviceisremoveflg.md#unknown)

**`memberof`** AdGroupAdServiceResponsiveImageAd

___

### isRemoveTrackingUrl

• `Optional` **isRemoveTrackingUrl**: ``null`` \| [*True*](./enums/adgroupadserviceisremoveflg.md#true) \| [*False*](./enums/adgroupadserviceisremoveflg.md#false) \| [*Unknown*](./enums/adgroupadserviceisremoveflg.md#unknown)

**`memberof`** AdGroupAdServiceResponsiveImageAd

___

### logoMediaId

• `Optional` **logoMediaId**: ``null`` \| *number*

<div lang=\"ja\"> ロゴ画像のメディアIDです。<br> ADDおよびSET時、このフィールドは省略可能となります。 </div> 

**`memberof`** AdGroupAdServiceResponsiveImageAd

___

### principal

• `Optional` **principal**: ``null`` \| *string*

<div lang=\"ja\"> 広告の主体者表記です。<br> このフィールドは、ADD時は必須となり、SET時は省略可能となります。<br> ただし、キャンペーン目的「アプリ訴求」の場合は、キャンペーンのアプリ名と同一の値が自動的に設定され、アプリ名以外の値には変更できません。 </div> 

**`memberof`** AdGroupAdServiceResponsiveImageAd

___

### smartphoneFinalUrl

• `Optional` **smartphoneFinalUrl**: ``null`` \| *string*

<div lang=\"ja\">スマートフォン向けURLです。<br> finalUrlを指定するときのみ、任意で指定できます。<br> キャンペーン目的「アプリ訴求」の場合は、ADD、SETのどちらも指定できません。<br> SET時にurlを指定する場合、このフィールドの値はクリアされます。 <br>※現在利用できません</div> 

**`memberof`** AdGroupAdServiceResponsiveImageAd

___

### trackingUrl

• `Optional` **trackingUrl**: ``null`` \| *string*

<div lang=\"ja\">トラッキングURLです。<br> ADD時、このフィールドは省略可能となります。<br> ※SET時、こちらが審査中の場合、編集はできません。<br> finalUrlを指定するときのみ、任意で指定できます。<br> SET時にurlを指定する場合、このフィールドの値はクリアされます。 <br>※現在利用できません </div> 

**`memberof`** AdGroupAdServiceResponsiveImageAd

___

### url

• `Optional` **url**: ``null`` \| *string*

<div lang=\"ja\"> リンク先URLです。<br> アプリ訴求キャンペーンで設定可能なリンク先URLについては<a href=\"/reference/ads-display-api/v6/CampaignService/get/\">こちら</a>をご参照ください。<br> SET時、このフィールドは省略可能となります。<br> ADD時、urlフィールドとfinalUrlフィールドは同時に設定することはできず、どちらか片方の設定が必須となります。<br> urlフィールドを設定する場合、displayUrlの指定が必須になります。またその際は、finalUrl、smartphoneFinalUrl、trackingUrl、customParametersは指定不可です。<br> SET時にfinalUrlを指定する場合、このフィールドの値はクリアされます。 </div> 

**`memberof`** AdGroupAdServiceResponsiveImageAd
