# GuaranteedAdGroupAdServiceCarouselAd


<div lang=\"ja\"> GuaranteedAdGroupAdServiceCarouselAdオブジェクトはカルーセル広告の情報を表します。<br> このフィールドは、省略可能となります。<br> ※ADD時、adTypeがCAROUSEL_ADの場合は必須です。 </div> 

## Table of contents

### Properties

- [carousels](guaranteedadgroupadservicecarouselad.md#carousels)
- [displayUrl](guaranteedadgroupadservicecarouselad.md#displayurl)
- [logoMediaId](guaranteedadgroupadservicecarouselad.md#logomediaid)
- [principal](guaranteedadgroupadservicecarouselad.md#principal)
- [url](guaranteedadgroupadservicecarouselad.md#url)

## Properties

### carousels

• `Optional` **carousels**: ``null`` \| [*GuaranteedAdGroupAdServiceCarousel*](guaranteedadgroupadservicecarousel.md)[]

**`memberof`** GuaranteedAdGroupAdServiceCarouselAd

___

### displayUrl

• `Optional` **displayUrl**: ``null`` \| *string*

<div lang=\"ja\"> 表示URLです。<br> ADDおよびSET時、このフィールドは省略可能となります。<br> ・標準キャンペーンの場合<br> &nbsp;&nbsp;ADDでは入力必須です。SETでの入力は任意です。<br> ・アプリキャンペーンの場合<br> &nbsp;&nbsp;ADD、SETのどちらも指定できません。<br> &nbsp;&nbsp;※アプリキャンペーンで指定したDeviceOsTypeに基づき、以下のいずれかのURLが自動で設定されます。<br> &nbsp;&nbsp;&nbsp;&nbsp;- iOSの場合：itunes.apple.com<br> &nbsp;&nbsp;&nbsp;&nbsp;- Androidの場合：play.google.com </div> 

**`memberof`** GuaranteedAdGroupAdServiceCarouselAd

___

### logoMediaId

• `Optional` **logoMediaId**: ``null`` \| *number*

<div lang=\"ja\"> ロゴの画像IDです。<br> ADDおよびSET時、このフィールドは省略可能となります。 </div> 

**`memberof`** GuaranteedAdGroupAdServiceCarouselAd

___

### principal

• `Optional` **principal**: ``null`` \| *string*

<div lang=\"ja\"> 広告の主体者表記です。<br> このフィールドは、ADD時は必須となり、SET時は省略可能となります。 </div> 

**`memberof`** GuaranteedAdGroupAdServiceCarouselAd

___

### url

• `Optional` **url**: ``null`` \| *string*

<div lang=\"ja\"> リンク先URLです。<br> このフィールドは、ADD時は必須となり、SET時は省略可能となります。 </div> 

**`memberof`** GuaranteedAdGroupAdServiceCarouselAd
