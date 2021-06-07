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

<div lang=\"ja\"> 表示URLです。<br> ADDおよびSET時、このフィールドは省略可能となります。<br> ・標準キャンペーンの場合<br> &nbsp;&nbsp;ADDでは入力必須です。SETでの入力は任意です。<br> ・アプリキャンペーンの場合<br> &nbsp;&nbsp;ADD、SETのどちらも指定できません。<br> &nbsp;&nbsp;※アプリキャンペーンで指定したDeviceOsTypeに基づき、以下のいずれかのURLが自動で設定されます。<br> &nbsp;&nbsp;&nbsp;&nbsp;- iOSの場合：itunes.apple.com<br> &nbsp;&nbsp;&nbsp;&nbsp;- Androidの場合：play.google.com<br> </div> 

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

<div lang=\"ja\"> リンク先URLです。<br> このフィールドは、ADD時は必須となり、SET時は省略可能となります。 </div> 

**`memberof`** AdGroupAdServiceMobileAd
