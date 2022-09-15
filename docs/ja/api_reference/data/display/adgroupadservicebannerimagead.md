# AdGroupAdServiceBannerImageAd


<div lang=\"ja\"> AdGroupAdServiceBannerImageAdオブジェクトは、画像で構成される広告の情報を表します。<br> このフィールドは、省略可能となります。<br> ※ADD時、adTypeがBANNER_IMAGE_ADの場合は必須です。 </div> 

## Table of contents

### Properties

- [customParameters](adgroupadservicebannerimagead.md#customparameters)
- [displayUrl](adgroupadservicebannerimagead.md#displayurl)
- [displayUrlLevel](adgroupadservicebannerimagead.md#displayurllevel)
- [finalUrl](adgroupadservicebannerimagead.md#finalurl)
- [isRemoveSmartphoneFinalUrl](adgroupadservicebannerimagead.md#isremovesmartphonefinalurl)
- [isRemoveTrackingUrl](adgroupadservicebannerimagead.md#isremovetrackingurl)
- [smartphoneFinalUrl](adgroupadservicebannerimagead.md#smartphonefinalurl)
- [trackingUrl](adgroupadservicebannerimagead.md#trackingurl)
- [url](adgroupadservicebannerimagead.md#url)

## Properties

### customParameters

• `Optional` **customParameters**: ``null`` \| [*AdGroupAdServiceCustomParameters*](adgroupadservicecustomparameters.md)

**`memberof`** AdGroupAdServiceBannerImageAd

___

### displayUrl

• `Optional` **displayUrl**: ``null`` \| *string*

<div lang=\"ja\"> 表示URLです。<br> SET時、このフィールドは省略可能となります。<br> ADD時にurlを指定する場合、このフィールドは必須です。<br> ADD時にfinalUrlを指定する場合、このフィールドを指定することはできません。代わりにfinalUrlから生成された値が自動で設定されます。<br> ただし、キャンペーン目的「アプリ訴求」の場合は、ADD、SETのどちらも指定できません。キャンペーンで指定したDeviceOsTypeに基づき、以下のいずれかのURLが自動で設定されます。<br> - iOSの場合：itunes.apple.com<br> - Androidの場合：play.google.com </div> 

**`memberof`** AdGroupAdServiceBannerImageAd

___

### displayUrlLevel

• `Optional` **displayUrlLevel**: ``null`` \| [*Domain*](./enums/adgroupadservicedisplayurllevel.md#domain) \| [*FirstLevel*](./enums/adgroupadservicedisplayurllevel.md#firstlevel) \| [*Unknown*](./enums/adgroupadservicedisplayurllevel.md#unknown)

**`memberof`** AdGroupAdServiceBannerImageAd

___

### finalUrl

• `Optional` **finalUrl**: ``null`` \| *string*

<div lang=\"ja\">最終リンク先URLです。<br> ADD時、finalUrlフィールドとurlフィールドは同時に設定することはできず、どちらか片方の設定が必須となります。<br> finalUrlフィールドを設定する場合、smartphoneFinalUrl、trackingUrl、customParametersは任意になります。<br> SET時は省略可能となります。<br> SET時にurlを指定する場合、このフィールドの値はクリアされます。<br> キャンペーン目的「アプリ訴求」の場合は、このフィールドには以下のURLのみ設定できます。<br> - iOSの場合：itunes.apple.com, apps.apple.com<br> - Androidの場合：play.google.com </div> 

**`memberof`** AdGroupAdServiceBannerImageAd

___

### isRemoveSmartphoneFinalUrl

• `Optional` **isRemoveSmartphoneFinalUrl**: ``null`` \| [*True*](./enums/adgroupadserviceisremoveflg.md#true) \| [*False*](./enums/adgroupadserviceisremoveflg.md#false) \| [*Unknown*](./enums/adgroupadserviceisremoveflg.md#unknown)

**`memberof`** AdGroupAdServiceBannerImageAd

___

### isRemoveTrackingUrl

• `Optional` **isRemoveTrackingUrl**: ``null`` \| [*True*](./enums/adgroupadserviceisremoveflg.md#true) \| [*False*](./enums/adgroupadserviceisremoveflg.md#false) \| [*Unknown*](./enums/adgroupadserviceisremoveflg.md#unknown)

**`memberof`** AdGroupAdServiceBannerImageAd

___

### smartphoneFinalUrl

• `Optional` **smartphoneFinalUrl**: ``null`` \| *string*

<div lang=\"ja\">スマートフォン向けURLです。<br> finalUrlを指定するときのみ、任意で指定できます。<br> キャンペーン目的「アプリ訴求」の場合は、ADD、SETのどちらも指定できません。<br> SET時にurlを指定する場合、このフィールドの値はクリアされます。 </div> 

**`memberof`** AdGroupAdServiceBannerImageAd

___

### trackingUrl

• `Optional` **trackingUrl**: ``null`` \| *string*

<div lang=\"ja\">トラッキングURLです。<br> ADD時、このフィールドは省略可能となります。<br> ※SET時、こちらが審査中の場合、編集はできません。<br> finalUrlを指定するときのみ、任意で指定できます。<br> SET時にurlを指定する場合、このフィールドの値はクリアされます。 </div> 

**`memberof`** AdGroupAdServiceBannerImageAd

___

### url

• `Optional` **url**: ``null`` \| *string*

<div lang=\"ja\"> リンク先URLです。<br> アプリ訴求キャンペーンで設定可能なリンク先URLについては<a href=\"/reference/ads-display-api/v6/CampaignService/get/\">こちら</a>をご参照ください。<br> ADD時、urlフィールドとfinalUrlフィールドは同時に設定することはできず、どちらか片方の設定が必須となります。<br> urlフィールドを設定する場合、displayUrlの指定が必須になります。またその際は、finalUrl、smartphoneFinalUrl、trackingUrl、customParametersは指定不可です。<br> SET時は省略可能となります。<br> SET時にfinalUrlを指定する場合、このフィールドの値はクリアされます。 </div> 

**`memberof`** AdGroupAdServiceBannerImageAd
