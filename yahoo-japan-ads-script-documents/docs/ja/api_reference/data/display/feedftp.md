# FeedFtp


<div lang=\"ja\">FeedFtpオブジェクトは、定期アップロード設定情報を保持します。</div> 

## Table of contents

### Properties

- [accountId](feedftp.md#accountid)
- [activeStatus](feedftp.md#activestatus)
- [feedId](feedftp.md#feedid)
- [feedUrl](feedftp.md#feedurl)
- [itemListUploadType](feedftp.md#itemlistuploadtype)
- [schedule](feedftp.md#schedule)
- [userName](feedftp.md#username)
- [userPassword](feedftp.md#userpassword)

## Properties

### accountId

• `Optional` **accountId**: ``null`` \| *number*

<div lang=\"ja\"> アカウントIDです。<br> このフィールドは、レスポンスの際に返却されますが、リクエストの際には無視されます。 </div> 

**`memberof`** FeedFtp

___

### activeStatus

• `Optional` **activeStatus**: ``null`` \| [*Inactive*](./enums/feedftpserviceactivestatus.md#inactive) \| [*Active*](./enums/feedftpserviceactivestatus.md#active) \| [*Unknown*](./enums/feedftpserviceactivestatus.md#unknown)

**`memberof`** FeedFtp

___

### feedId

• `Optional` **feedId**: ``null`` \| *number*

<div lang=\"ja\"> Feedを識別するIdです。<br> このフィールドは、リクエストの場合は必須です。 </div> 

**`memberof`** FeedFtp

___

### feedUrl

• `Optional` **feedUrl**: ``null`` \| *string*

<div lang=\"ja\"> 商品リストファイルのURLです。<br> このフィールドは、ADD時は必須となり、SET時は省略可能となります。 </div> 

**`memberof`** FeedFtp

___

### itemListUploadType

• `Optional` **itemListUploadType**: ``null`` \| [*UpdatePart*](./enums/feedftpserviceitemlistuploadtype.md#updatepart) \| [*UpdateAll*](./enums/feedftpserviceitemlistuploadtype.md#updateall) \| [*Unknown*](./enums/feedftpserviceitemlistuploadtype.md#unknown)

**`memberof`** FeedFtp

___

### schedule

• `Optional` **schedule**: ``null`` \| [*FeedFtpServiceSchedule*](feedftpserviceschedule.md)

**`memberof`** FeedFtp

___

### userName

• `Optional` **userName**: ``null`` \| *string*

<div lang=\"ja\"> ユーザー名です。<br> このフィールドは、ADD時は必須となり、SET時は省略可能となります。 </div> 

**`memberof`** FeedFtp

___

### userPassword

• `Optional` **userPassword**: ``null`` \| *string*

<div lang=\"ja\"> パスワードです。<br> このフィールドは、ADD時は必須となり、SET時は省略可能となります。 </div> 

**`memberof`** FeedFtp
