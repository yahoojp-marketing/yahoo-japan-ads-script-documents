# AdGroupAdServiceCarousel


<div lang=\"ja\"> AdGroupAdServiceCarouselオブジェクトはカルーセル広告の詳細情報を表します。<br> ※SET時には、現在のCarouselsに含まれるCarouselが全て指定したCarouselsに置き換わります。<br> ※特定のCarousel単体を指定して変更することはできません。 </div> 

## Table of contents

### Properties

- [description](adgroupadservicecarousel.md#description)
- [disapprovalReasonCodes](adgroupadservicecarousel.md#disapprovalreasoncodes)
- [displayOrder](adgroupadservicecarousel.md#displayorder)
- [headline](adgroupadservicecarousel.md#headline)
- [mediaId](adgroupadservicecarousel.md#mediaid)
- [url](adgroupadservicecarousel.md#url)

## Properties

### description

• `Optional` **description**: ``null`` \| *string*

<div lang=\"ja\"> 広告の説明文です。<br> このフィールドは、SET時は必須となり、ADD時は省略可能となります。 </div> 

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

### headline

• `Optional` **headline**: ``null`` \| *string*

<div lang=\"ja\"> 広告のタイトルです。<br> このフィールドは、ADD時およびSET時に必須です。 </div> 

**`memberof`** AdGroupAdServiceCarousel

___

### mediaId

• `Optional` **mediaId**: ``null`` \| *number*

<div lang=\"ja\"> メディアIDです。<br> このフィールドは、ADD時およびSET時に指定不可です。 </div> 

**`memberof`** AdGroupAdServiceCarousel

___

### url

• `Optional` **url**: ``null`` \| *string*

<div lang=\"ja\"> リンク先URLです。<br> このフィールドは、ADD時およびSET時に必須です。 </div> 

**`memberof`** AdGroupAdServiceCarousel
