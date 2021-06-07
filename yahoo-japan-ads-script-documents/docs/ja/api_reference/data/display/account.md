# Account


<div lang=\"ja\">Accountオブジェクトは、アカウント情報を示します。<br> </div> 

## Table of contents

### Properties

- [accountId](account.md#accountid)
- [accountName](account.md#accountname)
- [accountStatus](account.md#accountstatus)
- [accountType](account.md#accounttype)
- [authType](account.md#authtype)
- [autoTaggingEnabled](account.md#autotaggingenabled)
- [contactBizId](account.md#contactbizid)
- [deliveryStatus](account.md#deliverystatus)
- [endDate](account.md#enddate)
- [isManagerAccount](account.md#ismanageraccount)
- [isTestAccount](account.md#istestaccount)
- [startDate](account.md#startdate)

## Properties

### accountId

• `Optional` **accountId**: ``null`` \| *number*

<div lang=\"ja\"> アカウントIDです。<br> SET時、このフィールドは必須となります。 </div> 

**`memberof`** Account

___

### accountName

• `Optional` **accountName**: ``null`` \| *string*

<div lang=\"ja\"> アカウント名です。<br> SET時、このフィールドは省略可能となります。 </div> 

**`memberof`** Account

___

### accountStatus

• `Optional` **accountStatus**: ``null`` \| [*Inprogress*](./enums/accountservicestatus.md#inprogress) \| [*WaitDecide*](./enums/accountservicestatus.md#waitdecide) \| [*Suspended*](./enums/accountservicestatus.md#suspended) \| [*Serving*](./enums/accountservicestatus.md#serving) \| [*Ended*](./enums/accountservicestatus.md#ended) \| [*Unknown*](./enums/accountservicestatus.md#unknown)

**`memberof`** Account

___

### accountType

• `Optional` **accountType**: ``null`` \| [*Prepay*](./enums/accountservicetype.md#prepay) \| [*Invoice*](./enums/accountservicetype.md#invoice) \| [*Unknown*](./enums/accountservicetype.md#unknown)

**`memberof`** Account

___

### authType

• `Optional` **authType**: ``null`` \| [*Referable*](./enums/accountserviceauthtype.md#referable) \| [*Updatable*](./enums/accountserviceauthtype.md#updatable) \| [*Unknown*](./enums/accountserviceauthtype.md#unknown)

**`memberof`** Account

___

### autoTaggingEnabled

• `Optional` **autoTaggingEnabled**: ``null`` \| [*False*](./enums/accountserviceautotaggingenabled.md#false) \| [*True*](./enums/accountserviceautotaggingenabled.md#true) \| [*Unknown*](./enums/accountserviceautotaggingenabled.md#unknown)

**`memberof`** Account

___

### contactBizId

• `Optional` **contactBizId**: ``null`` \| *string*

<div lang=\"ja\">アカウント管理者のYahoo! JAPANビジネスIDです。<br> MCCアカウントの場合、このフィールドは返却されず、リクエストの際も無視されます。<br> テストアカウントの場合、このフィールドは更新できません。</div> 

**`memberof`** Account

___

### deliveryStatus

• `Optional` **deliveryStatus**: ``null`` \| [*Active*](./enums/accountservicedeliverystatus.md#active) \| [*Paused*](./enums/accountservicedeliverystatus.md#paused) \| [*Unknown*](./enums/accountservicedeliverystatus.md#unknown)

**`memberof`** Account

___

### endDate

• `Optional` **endDate**: ``null`` \| *string*

<div lang=\"ja\"> 掲載終了日です。<br> このフィールドは、レスポンスの際に返却されますが、リクエストの際には無視されます。 </div> 

**`memberof`** Account

___

### isManagerAccount

• `Optional` **isManagerAccount**: ``null`` \| [*False*](./enums/accountserviceismanageraccount.md#false) \| [*True*](./enums/accountserviceismanageraccount.md#true) \| [*Unknown*](./enums/accountserviceismanageraccount.md#unknown)

**`memberof`** Account

___

### isTestAccount

• `Optional` **isTestAccount**: ``null`` \| [*True*](./enums/accountserviceistestaccount.md#true) \| [*False*](./enums/accountserviceistestaccount.md#false) \| [*Unknown*](./enums/accountserviceistestaccount.md#unknown)

**`memberof`** Account

___

### startDate

• `Optional` **startDate**: ``null`` \| *string*

<div lang=\"ja\"> 掲載開始日です。<br> このフィールドは、レスポンスの際に返却されますが、リクエストの際には無視されます。 </div> 

**`memberof`** Account
