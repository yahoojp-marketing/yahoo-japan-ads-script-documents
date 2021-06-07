# AccountManagement


<div lang=\"ja\">AccountManagementオブジェクトは、アカウント情報を表します。</div> 

## Table of contents

### Properties

- [accountId](accountmanagement.md#accountid)
- [accountName](accountmanagement.md#accountname)
- [accountPayment](accountmanagement.md#accountpayment)
- [agencyPersonName](accountmanagement.md#agencypersonname)
- [agencyPrefectureCode](accountmanagement.md#agencyprefecturecode)
- [authType](accountmanagement.md#authtype)
- [autoTaggingEnabled](accountmanagement.md#autotaggingenabled)
- [client](accountmanagement.md#client)
- [clientType](accountmanagement.md#clienttype)
- [contactBizId](accountmanagement.md#contactbizid)
- [deliveryStatus](accountmanagement.md#deliverystatus)
- [endDate](accountmanagement.md#enddate)
- [isTestAccount](accountmanagement.md#istestaccount)
- [startDate](accountmanagement.md#startdate)
- [status](accountmanagement.md#status)

## Properties

### accountId

• `Optional` **accountId**: ``null`` \| *number*

<div lang=\"ja\"> アカウントIDです。<br> このフィールドは、レスポンスの際に返却されますが、リクエストの際には無視されます。 </div> 

**`memberof`** AccountManagement

___

### accountName

• `Optional` **accountName**: ``null`` \| *string*

<div lang=\"ja\">アカウント名です。<br>このフィールドは、ADD時は必須となり、SET時は省略可能となります。</div> 

**`memberof`** AccountManagement

___

### accountPayment

• `Optional` **accountPayment**: ``null`` \| [*AccountManagementServicePayment*](accountmanagementservicepayment.md)

**`memberof`** AccountManagement

___

### agencyPersonName

• `Optional` **agencyPersonName**: ``null`` \| *string*

<div lang=\"ja\"> 代理店担当者名です。<br> ADDおよびSET時、このフィールドは省略可能となります。 </div> 

**`memberof`** AccountManagement

___

### agencyPrefectureCode

• `Optional` **agencyPrefectureCode**: ``null`` \| [*Hokkaido*](./enums/accountmanagementserviceprefecturecode.md#hokkaido) \| [*Aomori*](./enums/accountmanagementserviceprefecturecode.md#aomori) \| [*Iwate*](./enums/accountmanagementserviceprefecturecode.md#iwate) \| [*Miyagi*](./enums/accountmanagementserviceprefecturecode.md#miyagi) \| [*Akita*](./enums/accountmanagementserviceprefecturecode.md#akita) \| [*Yamagata*](./enums/accountmanagementserviceprefecturecode.md#yamagata) \| [*Fukushima*](./enums/accountmanagementserviceprefecturecode.md#fukushima) \| [*Ibaraki*](./enums/accountmanagementserviceprefecturecode.md#ibaraki) \| [*Tochigi*](./enums/accountmanagementserviceprefecturecode.md#tochigi) \| [*Gunma*](./enums/accountmanagementserviceprefecturecode.md#gunma) \| [*Saitama*](./enums/accountmanagementserviceprefecturecode.md#saitama) \| [*Chiba*](./enums/accountmanagementserviceprefecturecode.md#chiba) \| [*Tokyo*](./enums/accountmanagementserviceprefecturecode.md#tokyo) \| [*Kanagawa*](./enums/accountmanagementserviceprefecturecode.md#kanagawa) \| [*Niigata*](./enums/accountmanagementserviceprefecturecode.md#niigata) \| [*Toyama*](./enums/accountmanagementserviceprefecturecode.md#toyama) \| [*Ishikawa*](./enums/accountmanagementserviceprefecturecode.md#ishikawa) \| [*Fukui*](./enums/accountmanagementserviceprefecturecode.md#fukui) \| [*Yamanashi*](./enums/accountmanagementserviceprefecturecode.md#yamanashi) \| [*Nagano*](./enums/accountmanagementserviceprefecturecode.md#nagano) \| [*Gifu*](./enums/accountmanagementserviceprefecturecode.md#gifu) \| [*Shizuoka*](./enums/accountmanagementserviceprefecturecode.md#shizuoka) \| [*Aichi*](./enums/accountmanagementserviceprefecturecode.md#aichi) \| [*Mie*](./enums/accountmanagementserviceprefecturecode.md#mie) \| [*Siga*](./enums/accountmanagementserviceprefecturecode.md#siga) \| [*Kyoto*](./enums/accountmanagementserviceprefecturecode.md#kyoto) \| [*Osaka*](./enums/accountmanagementserviceprefecturecode.md#osaka) \| [*Hyogo*](./enums/accountmanagementserviceprefecturecode.md#hyogo) \| [*Nara*](./enums/accountmanagementserviceprefecturecode.md#nara) \| [*Wakayama*](./enums/accountmanagementserviceprefecturecode.md#wakayama) \| [*Tottori*](./enums/accountmanagementserviceprefecturecode.md#tottori) \| [*Shimane*](./enums/accountmanagementserviceprefecturecode.md#shimane) \| [*Okayama*](./enums/accountmanagementserviceprefecturecode.md#okayama) \| [*Hiroshima*](./enums/accountmanagementserviceprefecturecode.md#hiroshima) \| [*Yamaguchi*](./enums/accountmanagementserviceprefecturecode.md#yamaguchi) \| [*Tokushima*](./enums/accountmanagementserviceprefecturecode.md#tokushima) \| [*Kagawa*](./enums/accountmanagementserviceprefecturecode.md#kagawa) \| [*Ehime*](./enums/accountmanagementserviceprefecturecode.md#ehime) \| [*Kochi*](./enums/accountmanagementserviceprefecturecode.md#kochi) \| [*Fukuoka*](./enums/accountmanagementserviceprefecturecode.md#fukuoka) \| [*Saga*](./enums/accountmanagementserviceprefecturecode.md#saga) \| [*Nagasaki*](./enums/accountmanagementserviceprefecturecode.md#nagasaki) \| [*Kumamoto*](./enums/accountmanagementserviceprefecturecode.md#kumamoto) \| [*Oita*](./enums/accountmanagementserviceprefecturecode.md#oita) \| [*Miyazaki*](./enums/accountmanagementserviceprefecturecode.md#miyazaki) \| [*Kagoshima*](./enums/accountmanagementserviceprefecturecode.md#kagoshima) \| [*Okinawa*](./enums/accountmanagementserviceprefecturecode.md#okinawa) \| [*None*](./enums/accountmanagementserviceprefecturecode.md#none) \| [*Unknown*](./enums/accountmanagementserviceprefecturecode.md#unknown)

**`memberof`** AccountManagement

___

### authType

• `Optional` **authType**: ``null`` \| [*Referable*](./enums/accountmanagementserviceauthtype.md#referable) \| [*Updatable*](./enums/accountmanagementserviceauthtype.md#updatable) \| [*Unknown*](./enums/accountmanagementserviceauthtype.md#unknown)

**`memberof`** AccountManagement

___

### autoTaggingEnabled

• `Optional` **autoTaggingEnabled**: ``null`` \| [*False*](./enums/accountmanagementserviceautotaggingenabled.md#false) \| [*True*](./enums/accountmanagementserviceautotaggingenabled.md#true) \| [*Unknown*](./enums/accountmanagementserviceautotaggingenabled.md#unknown)

**`memberof`** AccountManagement

___

### client

• `Optional` **client**: ``null`` \| [*AccountManagementServiceClient*](accountmanagementserviceclient.md)

**`memberof`** AccountManagement

___

### clientType

• `Optional` **clientType**: ``null`` \| [*Agent*](./enums/accountmanagementserviceclienttype.md#agent) \| [*Self*](./enums/accountmanagementserviceclienttype.md#self) \| [*Unknown*](./enums/accountmanagementserviceclienttype.md#unknown)

**`memberof`** AccountManagement

___

### contactBizId

• `Optional` **contactBizId**: ``null`` \| *string*

<div lang=\"ja\"> アカウント管理者のYahoo! JAPANビジネスIDです。<br> このフィールドは、レスポンスの際に返却されますが、リクエストの際には無視されます。 </div> 

**`memberof`** AccountManagement

___

### deliveryStatus

• `Optional` **deliveryStatus**: ``null`` \| [*Active*](./enums/accountmanagementservicedeliverystatus.md#active) \| [*Paused*](./enums/accountmanagementservicedeliverystatus.md#paused) \| [*Unknown*](./enums/accountmanagementservicedeliverystatus.md#unknown)

**`memberof`** AccountManagement

___

### endDate

• `Optional` **endDate**: ``null`` \| *string*

<div lang=\"ja\"> 終了日<br> YYYYMMDD形式で指定 </div> 

**`memberof`** AccountManagement

___

### isTestAccount

• `Optional` **isTestAccount**: ``null`` \| [*True*](./enums/accountmanagementserviceistestaccount.md#true) \| [*False*](./enums/accountmanagementserviceistestaccount.md#false) \| [*Unknown*](./enums/accountmanagementserviceistestaccount.md#unknown)

**`memberof`** AccountManagement

___

### startDate

• `Optional` **startDate**: ``null`` \| *string*

<div lang=\"ja\"> 開始日（YYYYMMDD形式）<br> 自動でADD時の日付が登録される。 </div> 

**`memberof`** AccountManagement

___

### status

• `Optional` **status**: ``null`` \| [*Inprogress*](./enums/accountmanagementservicestatus.md#inprogress) \| [*WaitDecide*](./enums/accountmanagementservicestatus.md#waitdecide) \| [*Suspended*](./enums/accountmanagementservicestatus.md#suspended) \| [*Serving*](./enums/accountmanagementservicestatus.md#serving) \| [*Ended*](./enums/accountmanagementservicestatus.md#ended) \| [*Canceled*](./enums/accountmanagementservicestatus.md#canceled) \| [*Unknown*](./enums/accountmanagementservicestatus.md#unknown)

**`memberof`** AccountManagement
