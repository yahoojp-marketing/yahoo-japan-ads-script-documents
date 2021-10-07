# AdGroupAdServiceResponsiveVideoAd


<div lang=\"ja\"> AdGroupAdServiceResponsiveVideoAdオブジェクトは、動画広告の情報を表します。<br> このフィールドは、省略可能となります。<br> ※ADD時、adTypeがRESPONSIVE_VIDEO_ADの場合は必須です。 </div> 

## Table of contents

### Properties

- [buttonText](adgroupadserviceresponsivevideoad.md#buttontext)
- [customParameters](adgroupadserviceresponsivevideoad.md#customparameters)
- [description](adgroupadserviceresponsivevideoad.md#description)
- [displayUrl](adgroupadserviceresponsivevideoad.md#displayurl)
- [displayUrlLevel](adgroupadserviceresponsivevideoad.md#displayurllevel)
- [finalUrl](adgroupadserviceresponsivevideoad.md#finalurl)
- [headline](adgroupadserviceresponsivevideoad.md#headline)
- [isRemoveLogoMediaId](adgroupadserviceresponsivevideoad.md#isremovelogomediaid)
- [isRemoveSmartphoneFinalUrl](adgroupadserviceresponsivevideoad.md#isremovesmartphonefinalurl)
- [isRemoveTrackingUrl](adgroupadserviceresponsivevideoad.md#isremovetrackingurl)
- [isRemoveVideo10SecBeaconUrls](adgroupadserviceresponsivevideoad.md#isremovevideo10secbeaconurls)
- [isRemoveVideo25PercentBeaconUrls](adgroupadserviceresponsivevideoad.md#isremovevideo25percentbeaconurls)
- [isRemoveVideo3SecBeaconUrls](adgroupadserviceresponsivevideoad.md#isremovevideo3secbeaconurls)
- [isRemoveVideo50PercentBeaconUrls](adgroupadserviceresponsivevideoad.md#isremovevideo50percentbeaconurls)
- [isRemoveVideo75PercentBeaconUrls](adgroupadserviceresponsivevideoad.md#isremovevideo75percentbeaconurls)
- [isRemoveVideoCompleteBeaconUrls](adgroupadserviceresponsivevideoad.md#isremovevideocompletebeaconurls)
- [isRemoveVideoStartBeaconUrls](adgroupadserviceresponsivevideoad.md#isremovevideostartbeaconurls)
- [logoMediaId](adgroupadserviceresponsivevideoad.md#logomediaid)
- [principal](adgroupadserviceresponsivevideoad.md#principal)
- [smartphoneFinalUrl](adgroupadserviceresponsivevideoad.md#smartphonefinalurl)
- [thumbnailMediaId](adgroupadserviceresponsivevideoad.md#thumbnailmediaid)
- [trackingUrl](adgroupadserviceresponsivevideoad.md#trackingurl)
- [url](adgroupadserviceresponsivevideoad.md#url)
- [video10SecBeaconUrls](adgroupadserviceresponsivevideoad.md#video10secbeaconurls)
- [video25PercentBeaconUrls](adgroupadserviceresponsivevideoad.md#video25percentbeaconurls)
- [video3SecBeaconUrls](adgroupadserviceresponsivevideoad.md#video3secbeaconurls)
- [video50PercentBeaconUrls](adgroupadserviceresponsivevideoad.md#video50percentbeaconurls)
- [video75PercentBeaconUrls](adgroupadserviceresponsivevideoad.md#video75percentbeaconurls)
- [videoCompleteBeaconUrls](adgroupadserviceresponsivevideoad.md#videocompletebeaconurls)
- [videoStartBeaconUrls](adgroupadserviceresponsivevideoad.md#videostartbeaconurls)

## Properties

### buttonText

• `Optional` **buttonText**: ``null`` \| [*ForMoreInfo*](./enums/adgroupadservicebuttontext.md#formoreinfo) \| [*ConfirmNow*](./enums/adgroupadservicebuttontext.md#confirmnow) \| [*ApplyHere*](./enums/adgroupadservicebuttontext.md#applyhere) \| [*Purchase*](./enums/adgroupadservicebuttontext.md#purchase) \| [*Experience*](./enums/adgroupadservicebuttontext.md#experience) \| [*ConfirmProperty*](./enums/adgroupadservicebuttontext.md#confirmproperty) \| [*RequestInfo*](./enums/adgroupadservicebuttontext.md#requestinfo) \| [*Download*](./enums/adgroupadservicebuttontext.md#download) \| [*Install*](./enums/adgroupadservicebuttontext.md#install) \| [*MoreDetail*](./enums/adgroupadservicebuttontext.md#moredetail) \| [*ReserveHere*](./enums/adgroupadservicebuttontext.md#reservehere) \| [*Register*](./enums/adgroupadservicebuttontext.md#register) \| [*ApplyNow*](./enums/adgroupadservicebuttontext.md#applynow) \| [*PurchaseNow*](./enums/adgroupadservicebuttontext.md#purchasenow) \| [*ReserveNow*](./enums/adgroupadservicebuttontext.md#reservenow) \| [*RegisterNow*](./enums/adgroupadservicebuttontext.md#registernow) \| [*ContactUs*](./enums/adgroupadservicebuttontext.md#contactus) \| [*Unknown*](./enums/adgroupadservicebuttontext.md#unknown)

**`memberof`** AdGroupAdServiceResponsiveVideoAd

___

### customParameters

• `Optional` **customParameters**: ``null`` \| [*AdGroupAdServiceCustomParameters*](adgroupadservicecustomparameters.md)

**`memberof`** AdGroupAdServiceResponsiveVideoAd

___

### description

• `Optional` **description**: ``null`` \| *string*

<div lang=\"ja\"> 広告の説明文です。<br> このフィールドは、ADD時は必須となり、SET時は省略可能となります。 </div> 

**`memberof`** AdGroupAdServiceResponsiveVideoAd

___

### displayUrl

• `Optional` **displayUrl**: ``null`` \| *string*

<div lang=\"ja\"> 表示URLです。<br> SET時、このフィールドは省略可能となります。<br> ADD時にurlを指定する場合、このフィールドは必須です。<br> ADD時にfinalUrlを指定する場合、このフィールドを指定することはできません。代わりにfinalUrlから生成された値が自動で設定されます。<br> ただし、キャンペーン目的「アプリ訴求」の場合は、ADD、SETのどちらも指定できません。キャンペーンで指定したDeviceOsTypeに基づき、以下のいずれかのURLが自動で設定されます。<br> - iOSの場合：itunes.apple.com<br> - Androidの場合：play.google.com </div> 

**`memberof`** AdGroupAdServiceResponsiveVideoAd

___

### displayUrlLevel

• `Optional` **displayUrlLevel**: ``null`` \| [*Domain*](./enums/adgroupadservicedisplayurllevel.md#domain) \| [*FirstLevel*](./enums/adgroupadservicedisplayurllevel.md#firstlevel) \| [*Unknown*](./enums/adgroupadservicedisplayurllevel.md#unknown)

**`memberof`** AdGroupAdServiceResponsiveVideoAd

___

### finalUrl

• `Optional` **finalUrl**: ``null`` \| *string*

<div lang=\"ja\">最終リンク先URLです。<br> ADD時、finalUrlフィールドとurlフィールドは同時に設定することはできず、どちらか片方の設定が必須となります。<br> finalUrlフィールドを設定する場合、smartphoneFinalUrl、trackingUrl、customParametersは任意になります。<br> SET時は省略可能となります。<br> SET時にurlを指定する場合、このフィールドの値はクリアされます。 <br>※現在利用できません </div> 

**`memberof`** AdGroupAdServiceResponsiveVideoAd

___

### headline

• `Optional` **headline**: ``null`` \| *string*

<div lang=\"ja\"> 広告のタイトルです。<br> このフィールドは、ADD時は必須となり、SET時は省略可能となります。 </div> 

**`memberof`** AdGroupAdServiceResponsiveVideoAd

___

### isRemoveLogoMediaId

• `Optional` **isRemoveLogoMediaId**: ``null`` \| [*True*](./enums/adgroupadserviceisremoveflg.md#true) \| [*False*](./enums/adgroupadserviceisremoveflg.md#false) \| [*Unknown*](./enums/adgroupadserviceisremoveflg.md#unknown)

**`memberof`** AdGroupAdServiceResponsiveVideoAd

___

### isRemoveSmartphoneFinalUrl

• `Optional` **isRemoveSmartphoneFinalUrl**: ``null`` \| [*True*](./enums/adgroupadserviceisremoveflg.md#true) \| [*False*](./enums/adgroupadserviceisremoveflg.md#false) \| [*Unknown*](./enums/adgroupadserviceisremoveflg.md#unknown)

**`memberof`** AdGroupAdServiceResponsiveVideoAd

___

### isRemoveTrackingUrl

• `Optional` **isRemoveTrackingUrl**: ``null`` \| [*True*](./enums/adgroupadserviceisremoveflg.md#true) \| [*False*](./enums/adgroupadserviceisremoveflg.md#false) \| [*Unknown*](./enums/adgroupadserviceisremoveflg.md#unknown)

**`memberof`** AdGroupAdServiceResponsiveVideoAd

___

### isRemoveVideo10SecBeaconUrls

• `Optional` **isRemoveVideo10SecBeaconUrls**: ``null`` \| [*True*](./enums/adgroupadserviceisremoveflg.md#true) \| [*False*](./enums/adgroupadserviceisremoveflg.md#false) \| [*Unknown*](./enums/adgroupadserviceisremoveflg.md#unknown)

**`memberof`** AdGroupAdServiceResponsiveVideoAd

___

### isRemoveVideo25PercentBeaconUrls

• `Optional` **isRemoveVideo25PercentBeaconUrls**: ``null`` \| [*True*](./enums/adgroupadserviceisremoveflg.md#true) \| [*False*](./enums/adgroupadserviceisremoveflg.md#false) \| [*Unknown*](./enums/adgroupadserviceisremoveflg.md#unknown)

**`memberof`** AdGroupAdServiceResponsiveVideoAd

___

### isRemoveVideo3SecBeaconUrls

• `Optional` **isRemoveVideo3SecBeaconUrls**: ``null`` \| [*True*](./enums/adgroupadserviceisremoveflg.md#true) \| [*False*](./enums/adgroupadserviceisremoveflg.md#false) \| [*Unknown*](./enums/adgroupadserviceisremoveflg.md#unknown)

**`memberof`** AdGroupAdServiceResponsiveVideoAd

___

### isRemoveVideo50PercentBeaconUrls

• `Optional` **isRemoveVideo50PercentBeaconUrls**: ``null`` \| [*True*](./enums/adgroupadserviceisremoveflg.md#true) \| [*False*](./enums/adgroupadserviceisremoveflg.md#false) \| [*Unknown*](./enums/adgroupadserviceisremoveflg.md#unknown)

**`memberof`** AdGroupAdServiceResponsiveVideoAd

___

### isRemoveVideo75PercentBeaconUrls

• `Optional` **isRemoveVideo75PercentBeaconUrls**: ``null`` \| [*True*](./enums/adgroupadserviceisremoveflg.md#true) \| [*False*](./enums/adgroupadserviceisremoveflg.md#false) \| [*Unknown*](./enums/adgroupadserviceisremoveflg.md#unknown)

**`memberof`** AdGroupAdServiceResponsiveVideoAd

___

### isRemoveVideoCompleteBeaconUrls

• `Optional` **isRemoveVideoCompleteBeaconUrls**: ``null`` \| [*True*](./enums/adgroupadserviceisremoveflg.md#true) \| [*False*](./enums/adgroupadserviceisremoveflg.md#false) \| [*Unknown*](./enums/adgroupadserviceisremoveflg.md#unknown)

**`memberof`** AdGroupAdServiceResponsiveVideoAd

___

### isRemoveVideoStartBeaconUrls

• `Optional` **isRemoveVideoStartBeaconUrls**: ``null`` \| [*True*](./enums/adgroupadserviceisremoveflg.md#true) \| [*False*](./enums/adgroupadserviceisremoveflg.md#false) \| [*Unknown*](./enums/adgroupadserviceisremoveflg.md#unknown)

**`memberof`** AdGroupAdServiceResponsiveVideoAd

___

### logoMediaId

• `Optional` **logoMediaId**: ``null`` \| *number*

<div lang=\"ja\"> ロゴの画像IDです。<br> ADDおよびSET時、このフィールドは省略可能となります。 </div> 

**`memberof`** AdGroupAdServiceResponsiveVideoAd

___

### principal

• `Optional` **principal**: ``null`` \| *string*

<div lang=\"ja\"> 広告の主体者表記です。<br> このフィールドは、ADD時は必須となり、SET時は省略可能となります。<br> ただし、キャンペーン目的「アプリ訴求」の場合は、キャンペーンのアプリ名と同一の値が自動的に設定され、アプリ名以外の値には変更できません。 </div> 

**`memberof`** AdGroupAdServiceResponsiveVideoAd

___

### smartphoneFinalUrl

• `Optional` **smartphoneFinalUrl**: ``null`` \| *string*

<div lang=\"ja\">スマートフォン向けURLです。<br> finalUrlを指定するときのみ、任意で指定できます。<br> キャンペーン目的「アプリ訴求」の場合は、ADD、SETのどちらも指定できません。<br> SET時にurlを指定する場合、このフィールドの値はクリアされます。 <br>※現在利用できません </div> 

**`memberof`** AdGroupAdServiceResponsiveVideoAd

___

### thumbnailMediaId

• `Optional` **thumbnailMediaId**: ``null`` \| *number*

<div lang=\"ja\"> サムネイルIDです。<br> このフィールドは、ADD時は必須となり、SET時は省略可能となります。 </div> 

**`memberof`** AdGroupAdServiceResponsiveVideoAd

___

### trackingUrl

• `Optional` **trackingUrl**: ``null`` \| *string*

<div lang=\"ja\">トラッキングURLです。<br> ADD時、このフィールドは省略可能となります。<br> ※SET時、こちらが審査中の場合、編集はできません。<br> finalUrlを指定するときのみ、任意で指定できます。<br> SET時にurlを指定する場合、このフィールドの値はクリアされます。 <br>※現在利用できません </div> 

**`memberof`** AdGroupAdServiceResponsiveVideoAd

___

### url

• `Optional` **url**: ``null`` \| *string*

<div lang=\"ja\"> リンク先URLです。<br> アプリ訴求キャンペーンで設定可能なリンク先URLについては<a href=\"/reference/ads-display-api/v6/CampaignService/get/\">こちら</a>をご参照ください。<br> SET時、このフィールドは省略可能となります。<br> ADD時、urlフィールドとfinalUrlフィールドは同時に設定することはできず、どちらか片方の設定が必須となります。<br> urlフィールドを設定する場合、displayUrlの指定が必須になります。またその際は、finalUrl、smartphoneFinalUrl、trackingUrl、customParametersは指定不可です。<br> SET時にfinalUrlを指定する場合、このフィールドの値はクリアされます。 </div> 

**`memberof`** AdGroupAdServiceResponsiveVideoAd

___

### video10SecBeaconUrls

• `Optional` **video10SecBeaconUrls**: ``null`` \| *string*[]

<div lang=\"ja\"> 10秒視聴ビーコンURLです。<br> ADDおよびSET時、このフィールドは省略可能となります。<br> ※SET時はすべて上書きされます。<br> ※httpsのURLのみ設定可能です。 </div> 

**`memberof`** AdGroupAdServiceResponsiveVideoAd

___

### video25PercentBeaconUrls

• `Optional` **video25PercentBeaconUrls**: ``null`` \| *string*[]

<div lang=\"ja\"> 25％再生視聴ビーコンURLです。<br> ADDおよびSET時、このフィールドは省略可能となります。<br> ※SET時はすべて上書きされます。<br> ※httpsのURLのみ設定可能です。 </div> 

**`memberof`** AdGroupAdServiceResponsiveVideoAd

___

### video3SecBeaconUrls

• `Optional` **video3SecBeaconUrls**: ``null`` \| *string*[]

<div lang=\"ja\"> 3秒視聴ビーコンURLです。<br> ADDおよびSET時、このフィールドは省略可能となります。<br> ※SET時はすべて上書きされます。<br> ※httpsのURLのみ設定可能です。 </div> 

**`memberof`** AdGroupAdServiceResponsiveVideoAd

___

### video50PercentBeaconUrls

• `Optional` **video50PercentBeaconUrls**: ``null`` \| *string*[]

<div lang=\"ja\"> 50％再生視聴ビーコンURLです。<br> ADDおよびSET時、このフィールドは省略可能となります。<br> ※SET時はすべて上書きされます。<br> ※httpsのURLのみ設定可能です。 </div> 

**`memberof`** AdGroupAdServiceResponsiveVideoAd

___

### video75PercentBeaconUrls

• `Optional` **video75PercentBeaconUrls**: ``null`` \| *string*[]

<div lang=\"ja\"> 75％再生視聴ビーコンURLです。<br> ADDおよびSET時、このフィールドは省略可能となります。<br> ※SET時はすべて上書きされます。<br> ※httpsのURLのみ設定可能です。 </div> 

**`memberof`** AdGroupAdServiceResponsiveVideoAd

___

### videoCompleteBeaconUrls

• `Optional` **videoCompleteBeaconUrls**: ``null`` \| *string*[]

<div lang=\"ja\"> 再生完了ビーコンURLです。<br> ADDおよびSET時、このフィールドは省略可能となります。<br> ※SET時はすべて上書きされます。<br> ※httpsのURLのみ設定可能です。 </div> 

**`memberof`** AdGroupAdServiceResponsiveVideoAd

___

### videoStartBeaconUrls

• `Optional` **videoStartBeaconUrls**: ``null`` \| *string*[]

<div lang=\"ja\"> 再生開始ビーコンURLです。<br> ADDおよびSET時、このフィールドは省略可能となります。<br> ※SET時はすべて上書きされます。<br> ※httpsのURLのみ設定可能です。 </div> 

**`memberof`** AdGroupAdServiceResponsiveVideoAd
