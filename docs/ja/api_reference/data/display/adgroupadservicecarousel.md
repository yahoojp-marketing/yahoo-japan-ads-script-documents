# AdGroupAdServiceCarousel


<div lang=\"ja\"> AdGroupAdServiceCarouselオブジェクトはカルーセル広告の詳細情報を表します。<br> ※SET時には、現在のCarouselsに含まれるCarouselが全て指定したCarouselsに置き換わります。<br> ※特定のCarousel単体を指定して変更することはできません。 </div> 

## Table of contents

### Properties

- [description](adgroupadservicecarousel.md#description)
- [disapprovalReasonCodes](adgroupadservicecarousel.md#disapprovalreasoncodes)
- [displayOrder](adgroupadservicecarousel.md#displayorder)
- [finalUrl](adgroupadservicecarousel.md#finalurl)
- [headline](adgroupadservicecarousel.md#headline)
- [isRemoveSmartphoneFinalUrl](adgroupadservicecarousel.md#isremovesmartphonefinalurl)
- [mediaId](adgroupadservicecarousel.md#mediaid)
- [smartphoneFinalUrl](adgroupadservicecarousel.md#smartphonefinalurl)
- [url](adgroupadservicecarousel.md#url)

## Properties

### description

• `Optional` **description**: ``null`` \| *string*

<div lang=\"ja\"> 広告の説明文です。<br> このフィールドは、ADD時およびSET時に必須です。 </div> 

**`memberof`** AdGroupAdServiceCarousel

___

### disapprovalReasonCodes

• `Optional` **disapprovalReasonCodes**: ``null`` \| *string*[]

<div lang=\"ja\"> 掲載拒否の理由です。<br> このフィールドは、レスポンスの際に返却されますが、リクエストの際には無視されます。 </div> 

**`memberof`** AdGroupAdServiceCarousel

___

### displayOrder

• `Optional` **displayOrder**: ``null`` \| *number*

<div lang=\"ja\"> カルーセルの表示順です。<br> ADDおよびSET時、このフィールドは省略可能となります。<br> ※指定しない場合は自動で設定されます。 </div> 

**`memberof`** AdGroupAdServiceCarousel

___

### finalUrl

• `Optional` **finalUrl**: ``null`` \| *string*

<div lang=\"ja\">最終リンク先URLです。<br> ADD時、finalUrlフィールドとurlフィールドは同時に設定することはできず、どちらか片方の設定が必須となります。<br> finalUrlフィールドを設定する場合、smartphoneFinalUrl、trackingUrl、customParametersは任意になります。<br> SET時は省略可能となります。<br> SET時にurlを指定する場合、このフィールドの値はクリアされます。 <br>※現在利用できません </div> 

**`memberof`** AdGroupAdServiceCarousel

___

### headline

• `Optional` **headline**: ``null`` \| *string*

<div lang=\"ja\"> 広告のタイトルです。<br> このフィールドは、ADD時およびSET時に必須です。 </div> 

**`memberof`** AdGroupAdServiceCarousel

___

### isRemoveSmartphoneFinalUrl

• `Optional` **isRemoveSmartphoneFinalUrl**: ``null`` \| [*True*](./enums/adgroupadserviceisremoveflg.md#true) \| [*False*](./enums/adgroupadserviceisremoveflg.md#false) \| [*Unknown*](./enums/adgroupadserviceisremoveflg.md#unknown)

**`memberof`** AdGroupAdServiceCarousel

___

### mediaId

• `Optional` **mediaId**: ``null`` \| *number*

<div lang=\"ja\"> メディアIDです。<br> このフィールドは、ADD時およびSET時に必須です。 </div> 

**`memberof`** AdGroupAdServiceCarousel

___

### smartphoneFinalUrl

• `Optional` **smartphoneFinalUrl**: ``null`` \| *string*

<div lang=\"ja\">スマートフォン向けURLです。<br> finalUrlを指定するときのみ、任意で指定できます。<br> キャンペーン目的「アプリ訴求」の場合は、ADD、SETのどちらも指定できません。<br> SET時にurlを指定する場合、このフィールドの値はクリアされます。 <br>※現在利用できません </div> 

**`memberof`** AdGroupAdServiceCarousel

___

### url

• `Optional` **url**: ``null`` \| *string*

<div lang=\"ja\"> リンク先URLです。<br> ADD時、urlフィールドとfinalUrlフィールドは同時に設定することはできず、どちらか片方の設定が必須となります。<br> SET時は省略可能となります。<br> SET時にfinalUrlを指定する場合、このフィールドの値はクリアされます。 </div> 

**`memberof`** AdGroupAdServiceCarousel
