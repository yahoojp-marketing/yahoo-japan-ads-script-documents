# Video


<div lang=\"ja\">Videoオブジェクトは、動画情報を保持します。</div> 

## Table of contents

### Properties

- [accountId](video.md#accountid)
- [approvalStatus](video.md#approvalstatus)
- [createdDate](video.md#createddate)
- [creationTime](video.md#creationtime)
- [disapprovalReasonCodes](video.md#disapprovalreasoncodes)
- [mediaId](video.md#mediaid)
- [processStatus](video.md#processstatus)
- [userStatus](video.md#userstatus)
- [videoName](video.md#videoname)
- [videoSetting](video.md#videosetting)
- [videoTitle](video.md#videotitle)

## Properties

### accountId

• `Optional` **accountId**: ``null`` \| *number*

<div lang=\"ja\"> アカウントIDです。<br> このフィールドは、SETおよびREMOVE時に必須となります。 </div> 

**`memberof`** Video

___

### approvalStatus

• `Optional` **approvalStatus**: ``null`` \| [*Approved*](./enums/videoserviceapprovalstatus.md#approved) \| [*Review*](./enums/videoserviceapprovalstatus.md#review) \| [*PreDisapproved*](./enums/videoserviceapprovalstatus.md#predisapproved) \| [*PostDisapproved*](./enums/videoserviceapprovalstatus.md#postdisapproved) \| [*Unknown*](./enums/videoserviceapprovalstatus.md#unknown)

**`memberof`** Video

___

### createdDate

• `Optional` **createdDate**: ``null`` \| *string*

<div lang=\"ja\">動画の作成日です。<br>※フォーマット：yyyyMMdd</div> 

**`memberof`** Video

___

### creationTime

• `Optional` **creationTime**: ``null`` \| *string*

<div lang=\"ja\">動画の入稿日時です。</div> 

**`memberof`** Video

___

### disapprovalReasonCodes

• `Optional` **disapprovalReasonCodes**: ``null`` \| *string*[]

<div lang=\"ja\">動画の掲載拒否理由です。</div> 

**`memberof`** Video

___

### mediaId

• `Optional` **mediaId**: ``null`` \| *number*

<div lang=\"ja\"> メディアIDです。<br> このフィールドは、SETおよびREMOVE時に必須となります。 </div> 

**`memberof`** Video

___

### processStatus

• `Optional` **processStatus**: ``null`` \| [*Processing*](./enums/videoserviceprocessstatus.md#processing) \| [*Finished*](./enums/videoserviceprocessstatus.md#finished) \| [*Failed*](./enums/videoserviceprocessstatus.md#failed) \| [*Unknown*](./enums/videoserviceprocessstatus.md#unknown)

**`memberof`** Video

___

### userStatus

• `Optional` **userStatus**: ``null`` \| [*Active*](./enums/videoserviceuserstatus.md#active) \| [*Paused*](./enums/videoserviceuserstatus.md#paused) \| [*Unknown*](./enums/videoserviceuserstatus.md#unknown)

**`memberof`** Video

___

### videoName

• `Optional` **videoName**: ``null`` \| *string*

<div lang=\"ja\">動画のファイル名です。</div> 

**`memberof`** Video

___

### videoSetting

• `Optional` **videoSetting**: ``null`` \| [*VideoServiceSetting*](videoservicesetting.md)

**`memberof`** Video

___

### videoTitle

• `Optional` **videoTitle**: ``null`` \| *string*

<div lang=\"ja\"> 動画名です。<br> このフィールドは、SET時に省略可能となります。 </div> 

**`memberof`** Video
