# AdGroupAdServiceBannerVideoAd


<div lang=\"ja\"> AdGroupAdServiceBannerVideoAdオブジェクトは、動画で構成される広告の情報を表します。<br> このフィールドは、省略可能となります。<br> ※ADD時、adTypeがBANNER_VIDEO_ADの場合は必須です。 </div> 

## Table of contents

### Properties

- [displayUrl](adgroupadservicebannervideoad.md#displayurl)
- [isRemoveVideo10SecBeaconUrls](adgroupadservicebannervideoad.md#isremovevideo10secbeaconurls)
- [isRemoveVideo25PercentBeaconUrls](adgroupadservicebannervideoad.md#isremovevideo25percentbeaconurls)
- [isRemoveVideo3SecBeaconUrls](adgroupadservicebannervideoad.md#isremovevideo3secbeaconurls)
- [isRemoveVideo50PercentBeaconUrls](adgroupadservicebannervideoad.md#isremovevideo50percentbeaconurls)
- [isRemoveVideo75PercentBeaconUrls](adgroupadservicebannervideoad.md#isremovevideo75percentbeaconurls)
- [isRemoveVideoCompleteBeaconUrls](adgroupadservicebannervideoad.md#isremovevideocompletebeaconurls)
- [isRemoveVideoStartBeaconUrls](adgroupadservicebannervideoad.md#isremovevideostartbeaconurls)
- [thumbnailMediaId](adgroupadservicebannervideoad.md#thumbnailmediaid)
- [url](adgroupadservicebannervideoad.md#url)
- [video10SecBeaconUrls](adgroupadservicebannervideoad.md#video10secbeaconurls)
- [video25PercentBeaconUrls](adgroupadservicebannervideoad.md#video25percentbeaconurls)
- [video3SecBeaconUrls](adgroupadservicebannervideoad.md#video3secbeaconurls)
- [video50PercentBeaconUrls](adgroupadservicebannervideoad.md#video50percentbeaconurls)
- [video75PercentBeaconUrls](adgroupadservicebannervideoad.md#video75percentbeaconurls)
- [videoCompleteBeaconUrls](adgroupadservicebannervideoad.md#videocompletebeaconurls)
- [videoStartBeaconUrls](adgroupadservicebannervideoad.md#videostartbeaconurls)

## Properties

### displayUrl

• `Optional` **displayUrl**: ``null`` \| *string*

<div lang=\"ja\"> 表示URLです。<br> このフィールドは、ADD時は必須となり、SET時は省略可能となります。 </div> 

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

### thumbnailMediaId

• `Optional` **thumbnailMediaId**: ``null`` \| *number*

<div lang=\"ja\"> サムネイルIDです。<br> このフィールドは、ADD時は必須となり、SET時は省略可能となります。 </div> 

**`memberof`** AdGroupAdServiceBannerVideoAd

___

### url

• `Optional` **url**: ``null`` \| *string*

<div lang=\"ja\"> リンク先URLです。<br> このフィールドは、ADD時は必須となり、SET時は省略可能となります。 </div> 

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
