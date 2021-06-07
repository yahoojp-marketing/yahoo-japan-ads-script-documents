# MediaServiceRecord


<div lang=\"ja\">MediaServiceRecordオブジェクトは、画像の情報を表します。</div> 

## Table of contents

### Properties

- [accountId](mediaservicerecord.md#accountid)
- [approvalStatus](mediaservicerecord.md#approvalstatus)
- [campaignBannerFlg](mediaservicerecord.md#campaignbannerflg)
- [createdDate](mediaservicerecord.md#createddate)
- [creationTime](mediaservicerecord.md#creationtime)
- [disapprovalReasonCodes](mediaservicerecord.md#disapprovalreasoncodes)
- [imageMedia](mediaservicerecord.md#imagemedia)
- [logoFlg](mediaservicerecord.md#logoflg)
- [mediaId](mediaservicerecord.md#mediaid)
- [mediaName](mediaservicerecord.md#medianame)
- [mediaRichFormatFlg](mediaservicerecord.md#mediarichformatflg)
- [mediaTitle](mediaservicerecord.md#mediatitle)
- [thumbnailFlg](mediaservicerecord.md#thumbnailflg)
- [userStatus](mediaservicerecord.md#userstatus)

## Properties

### accountId

• `Optional` **accountId**: ``null`` \| *number*

<div lang=\"ja\">アカウントIDです。<br> このフィールドは、リクエストの場合は必須です。 </div> 

**`memberof`** MediaServiceRecord

___

### approvalStatus

• `Optional` **approvalStatus**: ``null`` \| [*Approved*](./enums/mediaserviceapprovalstatus.md#approved) \| [*Review*](./enums/mediaserviceapprovalstatus.md#review) \| [*PreDisapproved*](./enums/mediaserviceapprovalstatus.md#predisapproved) \| [*PostDisapproved*](./enums/mediaserviceapprovalstatus.md#postdisapproved) \| [*Unknown*](./enums/mediaserviceapprovalstatus.md#unknown)

**`memberof`** MediaServiceRecord

___

### campaignBannerFlg

• `Optional` **campaignBannerFlg**: ``null`` \| [*False*](./enums/mediaservicecampaignbannerflg.md#false) \| [*True*](./enums/mediaservicecampaignbannerflg.md#true) \| [*Unknown*](./enums/mediaservicecampaignbannerflg.md#unknown)

**`memberof`** MediaServiceRecord

___

### createdDate

• `Optional` **createdDate**: ``null`` \| *string*

<div lang=\"ja\">データが作成された日です。<br>※フォーマット：yyyyMMdd</div> 

**`memberof`** MediaServiceRecord

___

### creationTime

• `Optional` **creationTime**: ``null`` \| *string*

<div lang=\"ja\">入稿日時です。</div> 

**`memberof`** MediaServiceRecord

___

### disapprovalReasonCodes

• `Optional` **disapprovalReasonCodes**: ``null`` \| *string*[]

<div lang=\"ja\">掲載拒否の理由です。</div> 

**`memberof`** MediaServiceRecord

___

### imageMedia

• `Optional` **imageMedia**: ``null`` \| [*MediaServiceImageMedia*](mediaserviceimagemedia.md)

**`memberof`** MediaServiceRecord

___

### logoFlg

• `Optional` **logoFlg**: ``null`` \| [*False*](./enums/mediaservicelogoflg.md#false) \| [*True*](./enums/mediaservicelogoflg.md#true) \| [*Unknown*](./enums/mediaservicelogoflg.md#unknown)

**`memberof`** MediaServiceRecord

___

### mediaId

• `Optional` **mediaId**: ``null`` \| *number*

<div lang=\"ja\">画像IDです。<br> このフィールドは、SETおよびREMOVE時に必須となります。 </div> 

**`memberof`** MediaServiceRecord

___

### mediaName

• `Optional` **mediaName**: ``null`` \| *string*

<div lang=\"ja\"> 実ファイル名です。<br> このフィールドは、ADD時に必須となります。 </div> 

**`memberof`** MediaServiceRecord

___

### mediaRichFormatFlg

• `Optional` **mediaRichFormatFlg**: ``null`` \| [*False*](./enums/mediaservicerichformatflg.md#false) \| [*True*](./enums/mediaservicerichformatflg.md#true) \| [*Unknown*](./enums/mediaservicerichformatflg.md#unknown)

**`memberof`** MediaServiceRecord

___

### mediaTitle

• `Optional` **mediaTitle**: ``null`` \| *string*

<div lang=\"ja\">画像名です。<br> このフィールドは、ADD時に必須となり、SET時に省略可能となります。 </div> 

**`memberof`** MediaServiceRecord

___

### thumbnailFlg

• `Optional` **thumbnailFlg**: ``null`` \| [*False*](./enums/mediaservicethumbnailflg.md#false) \| [*True*](./enums/mediaservicethumbnailflg.md#true) \| [*Unknown*](./enums/mediaservicethumbnailflg.md#unknown)

**`memberof`** MediaServiceRecord

___

### userStatus

• `Optional` **userStatus**: ``null`` \| [*Active*](./enums/mediaserviceuserstatus.md#active) \| [*Paused*](./enums/mediaserviceuserstatus.md#paused) \| [*Unknown*](./enums/mediaserviceuserstatus.md#unknown)

**`memberof`** MediaServiceRecord
