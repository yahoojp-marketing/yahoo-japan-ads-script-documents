# AdGroupAdServiceBannerVideoAd


<div lang=\"ja\"> AdGroupAdServiceBannerVideoAdオブジェクトは、動画で構成される広告の情報を表します。<br> このフィールドは、省略可能となります。<br> ※ADD時、adTypeがBANNER_VIDEO_ADの場合は必須です。 </div> 

## Table of contents

### Properties

- [customParameters](adgroupadservicebannervideoad.md#customparameters)
- [displayUrl](adgroupadservicebannervideoad.md#displayurl)
- [displayUrlLevel](adgroupadservicebannervideoad.md#displayurllevel)
- [finalUrl](adgroupadservicebannervideoad.md#finalurl)
- [isRemoveSmartphoneFinalUrl](adgroupadservicebannervideoad.md#isremovesmartphonefinalurl)
- [isRemoveTrackingUrl](adgroupadservicebannervideoad.md#isremovetrackingurl)
- [isRemoveVideo10SecBeaconUrls](adgroupadservicebannervideoad.md#isremovevideo10secbeaconurls)
- [isRemoveVideo25PercentBeaconUrls](adgroupadservicebannervideoad.md#isremovevideo25percentbeaconurls)
- [isRemoveVideo3SecBeaconUrls](adgroupadservicebannervideoad.md#isremovevideo3secbeaconurls)
- [isRemoveVideo50PercentBeaconUrls](adgroupadservicebannervideoad.md#isremovevideo50percentbeaconurls)
- [isRemoveVideo75PercentBeaconUrls](adgroupadservicebannervideoad.md#isremovevideo75percentbeaconurls)
- [isRemoveVideoCompleteBeaconUrls](adgroupadservicebannervideoad.md#isremovevideocompletebeaconurls)
- [isRemoveVideoStartBeaconUrls](adgroupadservicebannervideoad.md#isremovevideostartbeaconurls)
- [smartphoneFinalUrl](adgroupadservicebannervideoad.md#smartphonefinalurl)
- [thumbnailMediaId](adgroupadservicebannervideoad.md#thumbnailmediaid)
- [trackingUrl](adgroupadservicebannervideoad.md#trackingurl)
- [url](adgroupadservicebannervideoad.md#url)
- [video10SecBeaconUrls](adgroupadservicebannervideoad.md#video10secbeaconurls)
- [video25PercentBeaconUrls](adgroupadservicebannervideoad.md#video25percentbeaconurls)
- [video3SecBeaconUrls](adgroupadservicebannervideoad.md#video3secbeaconurls)
- [video50PercentBeaconUrls](adgroupadservicebannervideoad.md#video50percentbeaconurls)
- [video75PercentBeaconUrls](adgroupadservicebannervideoad.md#video75percentbeaconurls)
- [videoCompleteBeaconUrls](adgroupadservicebannervideoad.md#videocompletebeaconurls)
- [videoStartBeaconUrls](adgroupadservicebannervideoad.md#videostartbeaconurls)

## Properties

### customParameters

• `Optional` **customParameters**: ``null`` \| [*AdGroupAdServiceCustomParameters*](adgroupadservicecustomparameters.md)

**`memberof`** AdGroupAdServiceBannerVideoAd

___

### displayUrl

• `Optional` **displayUrl**: ``null`` \| *string*

<div lang=\"ja\"> 表示URLです。<br> SET時、このフィールドは省略可能となります。<br> ADD時にurlを指定する場合、このフィールドは必須です。<br> ADD時にfinalUrlを指定する場合、このフィールドを指定することはできません。代わりにfinalUrlから生成された値が自動で設定されます。 </div> 

**`memberof`** AdGroupAdServiceBannerVideoAd

___

### displayUrlLevel

• `Optional` **displayUrlLevel**: ``null`` \| [*Domain*](./enums/adgroupadservicedisplayurllevel.md#domain) \| [*FirstLevel*](./enums/adgroupadservicedisplayurllevel.md#firstlevel) \| [*Unknown*](./enums/adgroupadservicedisplayurllevel.md#unknown)

**`memberof`** AdGroupAdServiceBannerVideoAd

___

### finalUrl

• `Optional` **finalUrl**: ``null`` \| *string*

<div lang=\"ja\">最終リンク先URLです。<br> SET時、このフィールドは省略可能となります。<br> ADD時、finalUrlフィールドとurlフィールドは同時に設定することはできず、どちらか片方の設定が必須となります。<br> finalUrlフィールドを設定する場合、smartphoneFinalUrl、trackingUrl、customParametersは任意になります。<br> SET時にurlを指定する場合、このフィールドの値はクリアされます。 <br>※現在利用できません</div> 

**`memberof`** AdGroupAdServiceBannerVideoAd

___

### isRemoveSmartphoneFinalUrl

• `Optional` **isRemoveSmartphoneFinalUrl**: ``null`` \| [*True*](./enums/adgroupadserviceisremoveflg.md#true) \| [*False*](./enums/adgroupadserviceisremoveflg.md#false) \| [*Unknown*](./enums/adgroupadserviceisremoveflg.md#unknown)

**`memberof`** AdGroupAdServiceBannerVideoAd

___

### isRemoveTrackingUrl

• `Optional` **isRemoveTrackingUrl**: ``null`` \| [*True*](./enums/adgroupadserviceisremoveflg.md#true) \| [*False*](./enums/adgroupadserviceisremoveflg.md#false) \| [*Unknown*](./enums/adgroupadserviceisremoveflg.md#unknown)

**`memberof`** AdGroupAdServiceBannerVideoAd

___

### isRemoveVideo10SecBeaconUrls

• `Optional` **isRemoveVideo10SecBeaconUrls**: ``null`` \| [*True*](./enums/adgroupadserviceisremoveflg.md#true) \| [*False*](./enums/adgroupadserviceisremoveflg.md#false) \| [*Unknown*](./enums/adgroupadserviceisremoveflg.md#unknown)

**`memberof`** AdGroupAdServiceBannerVideoAd

___

### isRemoveVideo25PercentBeaconUrls

• `Optional` **isRemoveVideo25PercentBeaconUrls**: ``null`` \| [*True*](./enums/adgroupadserviceisremoveflg.md#true) \| [*False*](./enums/adgroupadserviceisremoveflg.md#false) \| [*Unknown*](./enums/adgroupadserviceisremoveflg.md#unknown)

**`memberof`** AdGroupAdServiceBannerVideoAd

___

### isRemoveVideo3SecBeaconUrls

• `Optional` **isRemoveVideo3SecBeaconUrls**: ``null`` \| [*True*](./enums/adgroupadserviceisremoveflg.md#true) \| [*False*](./enums/adgroupadserviceisremoveflg.md#false) \| [*Unknown*](./enums/adgroupadserviceisremoveflg.md#unknown)

**`memberof`** AdGroupAdServiceBannerVideoAd

___

### isRemoveVideo50PercentBeaconUrls

• `Optional` **isRemoveVideo50PercentBeaconUrls**: ``null`` \| [*True*](./enums/adgroupadserviceisremoveflg.md#true) \| [*False*](./enums/adgroupadserviceisremoveflg.md#false) \| [*Unknown*](./enums/adgroupadserviceisremoveflg.md#unknown)

**`memberof`** AdGroupAdServiceBannerVideoAd

___

### isRemoveVideo75PercentBeaconUrls

• `Optional` **isRemoveVideo75PercentBeaconUrls**: ``null`` \| [*True*](./enums/adgroupadserviceisremoveflg.md#true) \| [*False*](./enums/adgroupadserviceisremoveflg.md#false) \| [*Unknown*](./enums/adgroupadserviceisremoveflg.md#unknown)

**`memberof`** AdGroupAdServiceBannerVideoAd

___

### isRemoveVideoCompleteBeaconUrls

• `Optional` **isRemoveVideoCompleteBeaconUrls**: ``null`` \| [*True*](./enums/adgroupadserviceisremoveflg.md#true) \| [*False*](./enums/adgroupadserviceisremoveflg.md#false) \| [*Unknown*](./enums/adgroupadserviceisremoveflg.md#unknown)

**`memberof`** AdGroupAdServiceBannerVideoAd

___

### isRemoveVideoStartBeaconUrls

• `Optional` **isRemoveVideoStartBeaconUrls**: ``null`` \| [*True*](./enums/adgroupadserviceisremoveflg.md#true) \| [*False*](./enums/adgroupadserviceisremoveflg.md#false) \| [*Unknown*](./enums/adgroupadserviceisremoveflg.md#unknown)

**`memberof`** AdGroupAdServiceBannerVideoAd

___

### smartphoneFinalUrl

• `Optional` **smartphoneFinalUrl**: ``null`` \| *string*

<div lang=\"ja\">スマートフォン向けURLです。<br> finalUrlを指定するときのみ、任意で指定できます。<br> キャンペーン目的「アプリ訴求」の場合は、ADD、SETのどちらも指定できません。<br> SET時にurlを指定する場合、このフィールドの値はクリアされます。 <br>※現在利用できません</div> 

**`memberof`** AdGroupAdServiceBannerVideoAd

___

### thumbnailMediaId

• `Optional` **thumbnailMediaId**: ``null`` \| *number*

<div lang=\"ja\"> サムネイルIDです。<br> このフィールドは、ADD時は必須となり、SET時は省略可能となります。 </div> 

**`memberof`** AdGroupAdServiceBannerVideoAd

___

### trackingUrl

• `Optional` **trackingUrl**: ``null`` \| *string*

<div lang=\"ja\">トラッキングURLです。<br> ADD時、このフィールドは省略可能となります。<br> ※SET時、こちらが審査中の場合、編集はできません。<br> finalUrlを指定するときのみ、任意で指定できます。<br> SET時にurlを指定する場合、このフィールドの値はクリアされます。 <br>※現在利用できません</div> 

**`memberof`** AdGroupAdServiceBannerVideoAd

___

### url

• `Optional` **url**: ``null`` \| *string*

<div lang=\"ja\"> リンク先URLです。<br> アプリ訴求キャンペーンで設定可能なリンク先URLについては<a href=\"/reference/ads-display-api/v6/CampaignService/get/\">こちら</a>をご参照ください。<br> SET時、このフィールドは省略可能となります。<br> ADD時、urlフィールドとfinalUrlフィールドは同時に設定することはできず、どちらか片方の設定が必須となります。<br> urlフィールドを設定する場合、displayUrlの指定が必須になります。またその際は、finalUrl、smartphoneFinalUrl、trackingUrl、customParametersは指定不可です。<br> SET時にfinalUrlを指定する場合、このフィールドの値はクリアされます。 </div> 

**`memberof`** AdGroupAdServiceBannerVideoAd

___

### video10SecBeaconUrls

• `Optional` **video10SecBeaconUrls**: ``null`` \| *string*[]

<div lang=\"ja\"> 10秒視聴ビーコンURLです。<br> ADDおよびSET時、このフィールドは省略可能となります。<br> ※SET時はすべて上書きされます。<br> ※httpsのURLのみ設定可能です。 </div> 

**`memberof`** AdGroupAdServiceBannerVideoAd

___

### video25PercentBeaconUrls

• `Optional` **video25PercentBeaconUrls**: ``null`` \| *string*[]

<div lang=\"ja\"> 25％再生視聴ビーコンURLです。<br> ADDおよびSET時、このフィールドは省略可能となります。<br> ※SET時はすべて上書きされます。<br> ※httpsのURLのみ設定可能です。 </div> 

**`memberof`** AdGroupAdServiceBannerVideoAd

___

### video3SecBeaconUrls

• `Optional` **video3SecBeaconUrls**: ``null`` \| *string*[]

<div lang=\"ja\"> 3秒視聴ビーコンURLです。<br> ADDおよびSET時、このフィールドは省略可能となります。<br> ※SET時はすべて上書きされます。<br> ※httpsのURLのみ設定可能です。 </div> 

**`memberof`** AdGroupAdServiceBannerVideoAd

___

### video50PercentBeaconUrls

• `Optional` **video50PercentBeaconUrls**: ``null`` \| *string*[]

<div lang=\"ja\"> 50％再生視聴ビーコンURLです。<br> ADDおよびSET時、このフィールドは省略可能となります。<br> ※SET時はすべて上書きされます。<br> ※httpsのURLのみ設定可能です。 </div> 

**`memberof`** AdGroupAdServiceBannerVideoAd

___

### video75PercentBeaconUrls

• `Optional` **video75PercentBeaconUrls**: ``null`` \| *string*[]

<div lang=\"ja\"> 75％再生視聴ビーコンURLです。<br> ADDおよびSET時、このフィールドは省略可能となります。<br> ※SET時はすべて上書きされます。<br> ※httpsのURLのみ設定可能です。 </div> 

**`memberof`** AdGroupAdServiceBannerVideoAd

___

### videoCompleteBeaconUrls

• `Optional` **videoCompleteBeaconUrls**: ``null`` \| *string*[]

<div lang=\"ja\"> 再生完了ビーコンURLです。<br> ADDおよびSET時、このフィールドは省略可能となります。<br> ※SET時はすべて上書きされます。<br> ※httpsのURLのみ設定可能です。 </div> 

**`memberof`** AdGroupAdServiceBannerVideoAd

___

### videoStartBeaconUrls

• `Optional` **videoStartBeaconUrls**: ``null`` \| *string*[]

<div lang=\"ja\"> 再生開始ビーコンURLです。<br> ADDおよびSET時、このフィールドは省略可能となります。<br> ※SET時はすべて上書きされます。<br> ※httpsのURLのみ設定可能です。 </div> 

**`memberof`** AdGroupAdServiceBannerVideoAd
