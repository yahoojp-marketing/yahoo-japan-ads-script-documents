# AccountManagementServiceClient


<div lang=\"ja\">AccountManagementServiceClientオブジェクトは、広告主情報を表します。<br> このフィールドは、ADD時に必須となり、SET時に無視されます。</div> 

## Table of contents

### Properties

- [building](accountmanagementserviceclient.md#building)
- [city](accountmanagementserviceclient.md#city)
- [clientPersonName](accountmanagementserviceclient.md#clientpersonname)
- [companyName](accountmanagementserviceclient.md#companyname)
- [companyNameKana](accountmanagementserviceclient.md#companynamekana)
- [enterpriseType](accountmanagementserviceclient.md#enterprisetype)
- [enterpriseTypePosition](accountmanagementserviceclient.md#enterprisetypeposition)
- [phoneNumber](accountmanagementserviceclient.md#phonenumber)
- [prefectureCode](accountmanagementserviceclient.md#prefecturecode)
- [street1](accountmanagementserviceclient.md#street1)
- [street2](accountmanagementserviceclient.md#street2)
- [url](accountmanagementserviceclient.md#url)
- [urlType](accountmanagementserviceclient.md#urltype)
- [zip](accountmanagementserviceclient.md#zip)

## Properties

### building

• `Optional` **building**: ``null`` \| *string*

<div lang=\"ja\">ビル名です。<br>このフィールドは、ADD時に省略可能となり、SET時に無視されます。<br> ※clientTypeがSELFの場合は、ADD時、SET時ともに無視されます。<br> ※このフィールドは、レスポンスの際に返却されません。</div> 

**`memberof`** AccountManagementServiceClient

___

### city

• `Optional` **city**: ``null`` \| *string*

<div lang=\"ja\">市区町村名です。<br>このフィールドは、ADD時に必須となり、SET時に無視されます。<br> ※clientTypeがSELFの場合は、ADD時、SET時ともに無視されます。<br> ※このフィールドは、レスポンスの際に返却されません。</div> 

**`memberof`** AccountManagementServiceClient

___

### clientPersonName

• `Optional` **clientPersonName**: ``null`` \| *string*

<div lang=\"ja\">広告主の担当者氏名です。<br> このフィールドは、ADD時に省略可能となり、SET時に無視されます。</div> 

**`memberof`** AccountManagementServiceClient

___

### companyName

• `Optional` **companyName**: ``null`` \| *string*

<div lang=\"ja\">広告主名です。<br>このフィールドは、ADD時に必須となり、SET時に無視されます。<br> ※clientTypeがSELFの場合は、ADD時、SET時ともに無視されます。</div> 

**`memberof`** AccountManagementServiceClient

___

### companyNameKana

• `Optional` **companyNameKana**: ``null`` \| *string*

<div lang=\"ja\">広告主名カナです。<br> このフィールドは、ADD時に必須となり、SET時に無視されます。<br> ※clientTypeがSELFの場合は、ADD時、SET時ともに無視されます。</div> 

**`memberof`** AccountManagementServiceClient

___

### enterpriseType

• `Optional` **enterpriseType**: ``null`` \| [*Kabushiki*](./enums/accountmanagementserviceenterprisetype.md#kabushiki) \| [*Yugen*](./enums/accountmanagementserviceenterprisetype.md#yugen) \| [*Gosi*](./enums/accountmanagementserviceenterprisetype.md#gosi) \| [*Zaidan*](./enums/accountmanagementserviceenterprisetype.md#zaidan) \| [*Syadan*](./enums/accountmanagementserviceenterprisetype.md#syadan) \| [*Syukyo*](./enums/accountmanagementserviceenterprisetype.md#syukyo) \| [*Gakko*](./enums/accountmanagementserviceenterprisetype.md#gakko) \| [*Kojin*](./enums/accountmanagementserviceenterprisetype.md#kojin) \| [*Other*](./enums/accountmanagementserviceenterprisetype.md#other) \| [*Gomei*](./enums/accountmanagementserviceenterprisetype.md#gomei) \| [*Hieiri*](./enums/accountmanagementserviceenterprisetype.md#hieiri) \| [*Godo*](./enums/accountmanagementserviceenterprisetype.md#godo) \| [*Kyodo*](./enums/accountmanagementserviceenterprisetype.md#kyodo) \| [*Unknown*](./enums/accountmanagementserviceenterprisetype.md#unknown)

**`memberof`** AccountManagementServiceClient

___

### enterpriseTypePosition

• `Optional` **enterpriseTypePosition**: ``null`` \| [*Front*](./enums/accountmanagementserviceenterprisetypeposition.md#front) \| [*Back*](./enums/accountmanagementserviceenterprisetypeposition.md#back) \| [*Unknown*](./enums/accountmanagementserviceenterprisetypeposition.md#unknown)

**`memberof`** AccountManagementServiceClient

___

### phoneNumber

• `Optional` **phoneNumber**: ``null`` \| *string*

<div lang=\"ja\">電話番号です。<br> ※xxxxx-xxxxx-xxxxx形式です。<br> このフィールドは、ADD時に必須となり、SET時に無視されます。<br> ※clientTypeがSELFの場合は、ADD時、SET時ともに無視されます。<br> ※このフィールドは、レスポンスの際に返却されません。</div> 

**`memberof`** AccountManagementServiceClient

___

### prefectureCode

• `Optional` **prefectureCode**: ``null`` \| [*Hokkaido*](./enums/accountmanagementserviceprefecturecode.md#hokkaido) \| [*Aomori*](./enums/accountmanagementserviceprefecturecode.md#aomori) \| [*Iwate*](./enums/accountmanagementserviceprefecturecode.md#iwate) \| [*Miyagi*](./enums/accountmanagementserviceprefecturecode.md#miyagi) \| [*Akita*](./enums/accountmanagementserviceprefecturecode.md#akita) \| [*Yamagata*](./enums/accountmanagementserviceprefecturecode.md#yamagata) \| [*Fukushima*](./enums/accountmanagementserviceprefecturecode.md#fukushima) \| [*Ibaraki*](./enums/accountmanagementserviceprefecturecode.md#ibaraki) \| [*Tochigi*](./enums/accountmanagementserviceprefecturecode.md#tochigi) \| [*Gunma*](./enums/accountmanagementserviceprefecturecode.md#gunma) \| [*Saitama*](./enums/accountmanagementserviceprefecturecode.md#saitama) \| [*Chiba*](./enums/accountmanagementserviceprefecturecode.md#chiba) \| [*Tokyo*](./enums/accountmanagementserviceprefecturecode.md#tokyo) \| [*Kanagawa*](./enums/accountmanagementserviceprefecturecode.md#kanagawa) \| [*Niigata*](./enums/accountmanagementserviceprefecturecode.md#niigata) \| [*Toyama*](./enums/accountmanagementserviceprefecturecode.md#toyama) \| [*Ishikawa*](./enums/accountmanagementserviceprefecturecode.md#ishikawa) \| [*Fukui*](./enums/accountmanagementserviceprefecturecode.md#fukui) \| [*Yamanashi*](./enums/accountmanagementserviceprefecturecode.md#yamanashi) \| [*Nagano*](./enums/accountmanagementserviceprefecturecode.md#nagano) \| [*Gifu*](./enums/accountmanagementserviceprefecturecode.md#gifu) \| [*Shizuoka*](./enums/accountmanagementserviceprefecturecode.md#shizuoka) \| [*Aichi*](./enums/accountmanagementserviceprefecturecode.md#aichi) \| [*Mie*](./enums/accountmanagementserviceprefecturecode.md#mie) \| [*Siga*](./enums/accountmanagementserviceprefecturecode.md#siga) \| [*Kyoto*](./enums/accountmanagementserviceprefecturecode.md#kyoto) \| [*Osaka*](./enums/accountmanagementserviceprefecturecode.md#osaka) \| [*Hyogo*](./enums/accountmanagementserviceprefecturecode.md#hyogo) \| [*Nara*](./enums/accountmanagementserviceprefecturecode.md#nara) \| [*Wakayama*](./enums/accountmanagementserviceprefecturecode.md#wakayama) \| [*Tottori*](./enums/accountmanagementserviceprefecturecode.md#tottori) \| [*Shimane*](./enums/accountmanagementserviceprefecturecode.md#shimane) \| [*Okayama*](./enums/accountmanagementserviceprefecturecode.md#okayama) \| [*Hiroshima*](./enums/accountmanagementserviceprefecturecode.md#hiroshima) \| [*Yamaguchi*](./enums/accountmanagementserviceprefecturecode.md#yamaguchi) \| [*Tokushima*](./enums/accountmanagementserviceprefecturecode.md#tokushima) \| [*Kagawa*](./enums/accountmanagementserviceprefecturecode.md#kagawa) \| [*Ehime*](./enums/accountmanagementserviceprefecturecode.md#ehime) \| [*Kochi*](./enums/accountmanagementserviceprefecturecode.md#kochi) \| [*Fukuoka*](./enums/accountmanagementserviceprefecturecode.md#fukuoka) \| [*Saga*](./enums/accountmanagementserviceprefecturecode.md#saga) \| [*Nagasaki*](./enums/accountmanagementserviceprefecturecode.md#nagasaki) \| [*Kumamoto*](./enums/accountmanagementserviceprefecturecode.md#kumamoto) \| [*Oita*](./enums/accountmanagementserviceprefecturecode.md#oita) \| [*Miyazaki*](./enums/accountmanagementserviceprefecturecode.md#miyazaki) \| [*Kagoshima*](./enums/accountmanagementserviceprefecturecode.md#kagoshima) \| [*Okinawa*](./enums/accountmanagementserviceprefecturecode.md#okinawa) \| [*None*](./enums/accountmanagementserviceprefecturecode.md#none) \| [*Unknown*](./enums/accountmanagementserviceprefecturecode.md#unknown)

**`memberof`** AccountManagementServiceClient

___

### street1

• `Optional` **street1**: ``null`` \| *string*

<div lang=\"ja\">町・字名です。<br> このフィールドは、ADD時に必須となり、SET時に無視されます。<br> ※clientTypeがSELFの場合は、ADD時、SET時ともに無視されます。<br> ※このフィールドは、レスポンスの際に返却されません。</div> 

**`memberof`** AccountManagementServiceClient

___

### street2

• `Optional` **street2**: ``null`` \| *string*

<div lang=\"ja\">丁目・番地・号です。<br> このフィールドは、ADD時に必須となり、SET時に無視されます。<br> ※clientTypeがSELFの場合は、ADD時、SET時ともに無視されます。<br> ※このフィールドは、レスポンスの際に返却されません。</div> 

**`memberof`** AccountManagementServiceClient

___

### url

• `Optional` **url**: ``null`` \| *string*

<div lang=\"ja\">広告掲載を希望するサイトのURLです。<br> このフィールドは、ADD時に必須となり、SET時に無視されます。</div> 

**`memberof`** AccountManagementServiceClient

___

### urlType

• `Optional` **urlType**: ``null`` \| [*Pc*](./enums/accountmanagementserviceurltype.md#pc) \| [*Docomo*](./enums/accountmanagementserviceurltype.md#docomo) \| [*Kddi*](./enums/accountmanagementserviceurltype.md#kddi) \| [*Softbank*](./enums/accountmanagementserviceurltype.md#softbank) \| [*Other*](./enums/accountmanagementserviceurltype.md#other) \| [*Unknown*](./enums/accountmanagementserviceurltype.md#unknown)

**`memberof`** AccountManagementServiceClient

___

### zip

• `Optional` **zip**: ``null`` \| *string*

<div lang=\"ja\">郵便番号です。<br> ※xxx-xxxx形式です。<br> このフィールドは、ADD時に必須となり、SET時に無視されます。<br> ※clientTypeがSELFの場合は、ADD時、SET時ともに無視されます。<br> ※このフィールドは、レスポンスの際に返却されません。</div> 

**`memberof`** AccountManagementServiceClient
