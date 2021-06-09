# GuaranteedAdGroupAdServiceCarousel


<div lang=\"ja\"> GuaranteedAdGroupAdServiceCarouselオブジェクトはカルーセル広告の詳細情報を表します。<br> ※SET時には、現在のCarouselsに含まれるCarouselが全て指定したCarouselsに置き換わります。<br> ※特定のCarousel単体を指定して変更することはできません。 </div> 

## Table of contents

### Properties

- [description](guaranteedadgroupadservicecarousel.md#description)
- [disapprovalReasonCodes](guaranteedadgroupadservicecarousel.md#disapprovalreasoncodes)
- [displayOrder](guaranteedadgroupadservicecarousel.md#displayorder)
- [headline](guaranteedadgroupadservicecarousel.md#headline)
- [mediaId](guaranteedadgroupadservicecarousel.md#mediaid)
- [url](guaranteedadgroupadservicecarousel.md#url)

## Properties

### description

• `Optional` **description**: ``null`` \| *string*

<div lang=\"ja\"> 広告の説明文です。<br> このフィールドは、レスポンスの際に返却されますが、リクエストの際には無視されます。 </div> 

**`memberof`** GuaranteedAdGroupAdServiceCarousel

___

### disapprovalReasonCodes

• `Optional` **disapprovalReasonCodes**: ``null`` \| *string*[]

<div lang=\"ja\"> 掲載拒否の理由です。<br> このフィールドは、レスポンスの際に返却されますが、リクエストの際には無視されます。 </div> 

**`memberof`** GuaranteedAdGroupAdServiceCarousel

___

### displayOrder

• `Optional` **displayOrder**: ``null`` \| *number*

<div lang=\"ja\"> カルーセルの表示順です。<br> ADDおよびSET時、このフィールドは省略可能となります。<br> ※指定しない場合は自動で設定されます。 </div> 

**`memberof`** GuaranteedAdGroupAdServiceCarousel

___

### headline

• `Optional` **headline**: ``null`` \| *string*

<div lang=\"ja\"> 広告のタイトルです。<br> このフィールドは、ADD時およびSET時に必須です。 </div> 

**`memberof`** GuaranteedAdGroupAdServiceCarousel

___

### mediaId

• `Optional` **mediaId**: ``null`` \| *number*

<div lang=\"ja\"> メディアIDです。<br> このフィールドは、ADD時およびSET時に指定不可です。 </div> 

**`memberof`** GuaranteedAdGroupAdServiceCarousel

___

### url

• `Optional` **url**: ``null`` \| *string*

<div lang=\"ja\"> リンク先URLです。<br> このフィールドは、ADD時およびSET時に必須です。 </div> 

**`memberof`** GuaranteedAdGroupAdServiceCarousel
