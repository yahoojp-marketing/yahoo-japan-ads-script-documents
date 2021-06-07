# AdGroupAdServiceDynamicAd


<div lang=\"ja\"> AdGroupAdServiceDynamicAdオブジェクトは、動的ディスプレイ広告の情報を表します。<br> このフィールドは、省略可能となります。<br> ※ADD時、adTypeがDYNAMIC_ADの場合は必須です。 </div> 

## Table of contents

### Properties

- [brandColor](adgroupadservicedynamicad.md#brandcolor)
- [buttonText](adgroupadservicedynamicad.md#buttontext)
- [campaignBannerMediaId](adgroupadservicedynamicad.md#campaignbannermediaid)
- [campaignBannerMediaId2](adgroupadservicedynamicad.md#campaignbannermediaid2)
- [campaignBannerMediaId3](adgroupadservicedynamicad.md#campaignbannermediaid3)
- [campaignBannerMediaId4](adgroupadservicedynamicad.md#campaignbannermediaid4)
- [campaignBannerUrl](adgroupadservicedynamicad.md#campaignbannerurl)
- [displayUrl](adgroupadservicedynamicad.md#displayurl)
- [isRemoveBrandColor](adgroupadservicedynamicad.md#isremovebrandcolor)
- [isRemoveCampaignBannerMediaId](adgroupadservicedynamicad.md#isremovecampaignbannermediaid)
- [isRemoveCampaignBannerMediaId2](adgroupadservicedynamicad.md#isremovecampaignbannermediaid2)
- [isRemoveCampaignBannerMediaId3](adgroupadservicedynamicad.md#isremovecampaignbannermediaid3)
- [isRemoveCampaignBannerMediaId4](adgroupadservicedynamicad.md#isremovecampaignbannermediaid4)
- [isRemoveCampaignBannerUrl](adgroupadservicedynamicad.md#isremovecampaignbannerurl)
- [isRemovePrefix](adgroupadservicedynamicad.md#isremoveprefix)
- [isRemoveSuffix](adgroupadservicedynamicad.md#isremovesuffix)
- [logoMediaId](adgroupadservicedynamicad.md#logomediaid)
- [logoMediaId2](adgroupadservicedynamicad.md#logomediaid2)
- [logoMediaId3](adgroupadservicedynamicad.md#logomediaid3)
- [prefix](adgroupadservicedynamicad.md#prefix)
- [principal](adgroupadservicedynamicad.md#principal)
- [suffix](adgroupadservicedynamicad.md#suffix)
- [url](adgroupadservicedynamicad.md#url)

## Properties

### brandColor

• `Optional` **brandColor**: ``null`` \| *string*

<div lang=\"ja\"> ブランドカラーです。<br> ※RGB、HEX指定です。<br> 設定例：#FFFFFF<br> ADDおよびSET時、このフィールドは省略可能となります。 </div> 

**`memberof`** AdGroupAdServiceDynamicAd

___

### buttonText

• `Optional` **buttonText**: ``null`` \| [*ForMoreInfo*](./enums/adgroupadservicebuttontext.md#formoreinfo) \| [*ConfirmNow*](./enums/adgroupadservicebuttontext.md#confirmnow) \| [*ApplyHere*](./enums/adgroupadservicebuttontext.md#applyhere) \| [*Purchase*](./enums/adgroupadservicebuttontext.md#purchase) \| [*Experience*](./enums/adgroupadservicebuttontext.md#experience) \| [*ConfirmProperty*](./enums/adgroupadservicebuttontext.md#confirmproperty) \| [*RequestInfo*](./enums/adgroupadservicebuttontext.md#requestinfo) \| [*Download*](./enums/adgroupadservicebuttontext.md#download) \| [*Install*](./enums/adgroupadservicebuttontext.md#install) \| [*MoreDetail*](./enums/adgroupadservicebuttontext.md#moredetail) \| [*ReserveHere*](./enums/adgroupadservicebuttontext.md#reservehere) \| [*Register*](./enums/adgroupadservicebuttontext.md#register) \| [*ApplyNow*](./enums/adgroupadservicebuttontext.md#applynow) \| [*PurchaseNow*](./enums/adgroupadservicebuttontext.md#purchasenow) \| [*ReserveNow*](./enums/adgroupadservicebuttontext.md#reservenow) \| [*RegisterNow*](./enums/adgroupadservicebuttontext.md#registernow) \| [*ContactUs*](./enums/adgroupadservicebuttontext.md#contactus) \| [*Unknown*](./enums/adgroupadservicebuttontext.md#unknown)

**`memberof`** AdGroupAdServiceDynamicAd

___

### campaignBannerMediaId

• `Optional` **campaignBannerMediaId**: ``null`` \| *number*

<div lang=\"ja\"> キャンペーンバナー画像のメディアIDです。<br> ADDおよびSET時、このフィールドは省略可能となります。 </div> 

**`memberof`** AdGroupAdServiceDynamicAd

___

### campaignBannerMediaId2

• `Optional` **campaignBannerMediaId2**: ``null`` \| *number*

<div lang=\"ja\"> キャンペーンバナー画像のメディアID 2です。<br> ADDおよびSET時、このフィールドは省略可能となります。 </div> 

**`memberof`** AdGroupAdServiceDynamicAd

___

### campaignBannerMediaId3

• `Optional` **campaignBannerMediaId3**: ``null`` \| *number*

<div lang=\"ja\"> キャンペーンバナー画像のメディアID 3です。<br> ADDおよびSET時、このフィールドは省略可能となります。 </div> 

**`memberof`** AdGroupAdServiceDynamicAd

___

### campaignBannerMediaId4

• `Optional` **campaignBannerMediaId4**: ``null`` \| *number*

<div lang=\"ja\"> キャンペーンバナー画像のメディアID 4です。<br> ADDおよびSET時、このフィールドは省略可能となります。 </div> 

**`memberof`** AdGroupAdServiceDynamicAd

___

### campaignBannerUrl

• `Optional` **campaignBannerUrl**: ``null`` \| *string*

<div lang=\"ja\"> キャンペーンバナーURLです。<br> このフィールドは省略可能となります。<br> ADD時、設定する場合は以下のいずれかの指定が必要となります。<br> - campaignBannerMediaId<br> - campaignBannerMediaId2<br> - campaignBannerMediaId3<br> - campaignBannerMediaId4 </div> 

**`memberof`** AdGroupAdServiceDynamicAd

___

### displayUrl

• `Optional` **displayUrl**: ``null`` \| *string*

<div lang=\"ja\"> 表示URLです。<br> このフィールドは、ADD時は必須となり、SET時は省略可能となります。 </div> 

**`memberof`** AdGroupAdServiceDynamicAd

___

### isRemoveBrandColor

• `Optional` **isRemoveBrandColor**: ``null`` \| [*True*](./enums/adgroupadserviceisremoveflg.md#true) \| [*False*](./enums/adgroupadserviceisremoveflg.md#false) \| [*Unknown*](./enums/adgroupadserviceisremoveflg.md#unknown)

**`memberof`** AdGroupAdServiceDynamicAd

___

### isRemoveCampaignBannerMediaId

• `Optional` **isRemoveCampaignBannerMediaId**: ``null`` \| [*True*](./enums/adgroupadserviceisremoveflg.md#true) \| [*False*](./enums/adgroupadserviceisremoveflg.md#false) \| [*Unknown*](./enums/adgroupadserviceisremoveflg.md#unknown)

**`memberof`** AdGroupAdServiceDynamicAd

___

### isRemoveCampaignBannerMediaId2

• `Optional` **isRemoveCampaignBannerMediaId2**: ``null`` \| [*True*](./enums/adgroupadserviceisremoveflg.md#true) \| [*False*](./enums/adgroupadserviceisremoveflg.md#false) \| [*Unknown*](./enums/adgroupadserviceisremoveflg.md#unknown)

**`memberof`** AdGroupAdServiceDynamicAd

___

### isRemoveCampaignBannerMediaId3

• `Optional` **isRemoveCampaignBannerMediaId3**: ``null`` \| [*True*](./enums/adgroupadserviceisremoveflg.md#true) \| [*False*](./enums/adgroupadserviceisremoveflg.md#false) \| [*Unknown*](./enums/adgroupadserviceisremoveflg.md#unknown)

**`memberof`** AdGroupAdServiceDynamicAd

___

### isRemoveCampaignBannerMediaId4

• `Optional` **isRemoveCampaignBannerMediaId4**: ``null`` \| [*True*](./enums/adgroupadserviceisremoveflg.md#true) \| [*False*](./enums/adgroupadserviceisremoveflg.md#false) \| [*Unknown*](./enums/adgroupadserviceisremoveflg.md#unknown)

**`memberof`** AdGroupAdServiceDynamicAd

___

### isRemoveCampaignBannerUrl

• `Optional` **isRemoveCampaignBannerUrl**: ``null`` \| [*True*](./enums/adgroupadserviceisremoveflg.md#true) \| [*False*](./enums/adgroupadserviceisremoveflg.md#false) \| [*Unknown*](./enums/adgroupadserviceisremoveflg.md#unknown)

**`memberof`** AdGroupAdServiceDynamicAd

___

### isRemovePrefix

• `Optional` **isRemovePrefix**: ``null`` \| [*True*](./enums/adgroupadserviceisremoveflg.md#true) \| [*False*](./enums/adgroupadserviceisremoveflg.md#false) \| [*Unknown*](./enums/adgroupadserviceisremoveflg.md#unknown)

**`memberof`** AdGroupAdServiceDynamicAd

___

### isRemoveSuffix

• `Optional` **isRemoveSuffix**: ``null`` \| [*True*](./enums/adgroupadserviceisremoveflg.md#true) \| [*False*](./enums/adgroupadserviceisremoveflg.md#false) \| [*Unknown*](./enums/adgroupadserviceisremoveflg.md#unknown)

**`memberof`** AdGroupAdServiceDynamicAd

___

### logoMediaId

• `Optional` **logoMediaId**: ``null`` \| *number*

<div lang=\"ja\"> ロゴ画像のメディアIDです。<br> このフィールドは、ADD時は必須となり、SET時は省略可能となります。 </div> 

**`memberof`** AdGroupAdServiceDynamicAd

___

### logoMediaId2

• `Optional` **logoMediaId2**: ``null`` \| *number*

<div lang=\"ja\"> ロゴ画像のメディアID 2です。<br> このフィールドは、ADD時は必須となり、SET時は省略可能となります。 </div> 

**`memberof`** AdGroupAdServiceDynamicAd

___

### logoMediaId3

• `Optional` **logoMediaId3**: ``null`` \| *number*

<div lang=\"ja\"> ロゴ画像のメディアID 3です。<br> このフィールドは、ADD時は必須となり、SET時は省略可能となります。 </div> 

**`memberof`** AdGroupAdServiceDynamicAd

___

### prefix

• `Optional` **prefix**: ``null`` \| *string*

<div lang=\"ja\"> プレフィックスです。<br> ADDおよびSET時、このフィールドは省略可能となります。 </div> 

**`memberof`** AdGroupAdServiceDynamicAd

___

### principal

• `Optional` **principal**: ``null`` \| *string*

<div lang=\"ja\"> 広告の主体者表記です。<br> このフィールドは、ADD時は必須となり、SET時は省略可能となります。 </div> 

**`memberof`** AdGroupAdServiceDynamicAd

___

### suffix

• `Optional` **suffix**: ``null`` \| *string*

<div lang=\"ja\"> サフィックスです。<br> ADDおよびSET時、このフィールドは省略可能となります。 </div> 

**`memberof`** AdGroupAdServiceDynamicAd

___

### url

• `Optional` **url**: ``null`` \| *string*

<div lang=\"ja\"> リンク先URLです。<br> このフィールドは、ADD時は必須となり、SET時は省略可能となります。 </div> 

**`memberof`** AdGroupAdServiceDynamicAd
