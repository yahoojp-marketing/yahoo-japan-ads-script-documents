# AdGroupAdServiceMobileAd


<div lang=\"ja\"> AdGroupAdServiceMobileAdオブジェクトは、モバイル広告の情報を表します。<br> このフィールドは、省略可能となります。<br> ※ADD時、adTypeがTEXT_SHORT_AD1またはTEXT_SHORT_AD2の場合は必須です。 </div> 

## Table of contents

### Properties

- [description](adgroupadservicemobilead.md#description)
- [description2](adgroupadservicemobilead.md#description2)
- [displayUrl](adgroupadservicemobilead.md#displayurl)
- [headline](adgroupadservicemobilead.md#headline)
- [mobileCarriers](adgroupadservicemobilead.md#mobilecarriers)
- [url](adgroupadservicemobilead.md#url)

## Properties

### description

• `Optional` **description**: ``null`` \| *string*

<div lang=\"ja\"> 説明文（1行目）です。<br> このフィールドは、ADD時は必須となり、SET時は省略可能となります。 </div> 

**`memberof`** AdGroupAdServiceMobileAd

___

### description2

• `Optional` **description2**: ``null`` \| *string*

<div lang=\"ja\"> 説明文（2行目）です。<br> ADDおよびSET時、このフィールドは省略可能となります。 </div> 

**`memberof`** AdGroupAdServiceMobileAd

___

### displayUrl

• `Optional` **displayUrl**: ``null`` \| *string*

<div lang=\"ja\"> 表示URLです。<br> ADDおよびSET時、このフィールドは省略可能となります。<br> ただし、キャンペーン目的「アプリ訴求」の場合は、ADD、SETのどちらも指定できません。キャンペーンで指定したDeviceOsTypeに基づき、以下のいずれかのURLが自動で設定されます。<br> - iOSの場合：itunes.apple.com<br> - Androidの場合：play.google.com </div> 

**`memberof`** AdGroupAdServiceMobileAd

___

### headline

• `Optional` **headline**: ``null`` \| *string*

<div lang=\"ja\"> タイトルです。<br> このフィールドは、ADD時は必須となり、SET時は省略可能となります。 </div> 

**`memberof`** AdGroupAdServiceMobileAd

___

### mobileCarriers

• `Optional` **mobileCarriers**: ``null`` \| [*AdGroupAdServiceCarrierName*](./enums/adgroupadservicecarriername.md)[]

**`memberof`** AdGroupAdServiceMobileAd

___

### url

• `Optional` **url**: ``null`` \| *string*

<div lang=\"ja\"> リンク先URLです。<br> アプリ訴求キャンペーンで設定可能なリンク先URLについては<a href=\"/reference/ads-display-api/v6/CampaignService/get/\">こちら</a>をご参照ください。<br> このフィールドは、ADD時は必須となり、SET時は省略可能となります。 </div> 

**`memberof`** AdGroupAdServiceMobileAd
