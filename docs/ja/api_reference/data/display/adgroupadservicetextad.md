# AdGroupAdServiceTextAd


<div lang=\"ja\"> AdGroupAdServiceTextAdオブジェクトは、テキスト広告の情報を表します。<br> このフィールドは、省略可能となります。<br> ※ADD時、adTypeがTEXT_LONG_AD1またはTEXT_LONG_AD2の場合は必須です。 </div> 

## Table of contents

### Properties

- [description](adgroupadservicetextad.md#description)
- [description2](adgroupadservicetextad.md#description2)
- [displayUrl](adgroupadservicetextad.md#displayurl)
- [headline](adgroupadservicetextad.md#headline)
- [url](adgroupadservicetextad.md#url)

## Properties

### description

• `Optional` **description**: ``null`` \| *string*

<div lang=\"ja\"> 説明文（1行目）です。<br> このフィールドは、ADD時は必須となり、SET時は省略可能となります。 </div> 

**`memberof`** AdGroupAdServiceTextAd

___

### description2

• `Optional` **description2**: ``null`` \| *string*

<div lang=\"ja\"> 説明文（2行目）です。<br> ADDおよびSET時、このフィールドは省略可能となります。 </div> 

**`memberof`** AdGroupAdServiceTextAd

___

### displayUrl

• `Optional` **displayUrl**: ``null`` \| *string*

<div lang=\"ja\"> 表示URLです。<br> ADDおよびSET時、このフィールドは省略可能となります。<br> ただし、キャンペーン目的「アプリ訴求」の場合は、ADD、SETのどちらも指定できません。キャンペーンで指定したDeviceOsTypeに基づき、以下のいずれかのURLが自動で設定されます。<br> - iOSの場合：itunes.apple.com<br> - Androidの場合：play.google.com </div> 

**`memberof`** AdGroupAdServiceTextAd

___

### headline

• `Optional` **headline**: ``null`` \| *string*

<div lang=\"ja\"> タイトルです。<br> このフィールドは、ADD時は必須となり、SET時は省略可能となります。 </div> 

**`memberof`** AdGroupAdServiceTextAd

___

### url

• `Optional` **url**: ``null`` \| *string*

<div lang=\"ja\"> リンク先URLです。<br> アプリ訴求キャンペーンで設定可能なリンク先URLについては<a href=\"reference/ads-display-api/v5/CampaignService/get/\">こちら</a>をご参照ください。<br> このフィールドは、ADD時は必須となり、SET時は省略可能となります。 </div> 

**`memberof`** AdGroupAdServiceTextAd
