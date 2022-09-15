# AppLink


<div lang=\"ja\">AppLinkオブジェクトは、アプリリンク情報を表します。</div> 

## Table of contents

### Properties

- [accountId](applink.md#accountid)
- [appId](applink.md#appid)
- [appLinkId](applink.md#applinkid)
- [appLinkPlatform](applink.md#applinkplatform)
- [appVendorId](applink.md#appvendorid)
- [appVendorNameEn](applink.md#appvendornameen)
- [appVendorNameJa](applink.md#appvendornameja)
- [linkId](applink.md#linkid)
- [linkStatus](applink.md#linkstatus)
- [syncStatus](applink.md#syncstatus)

## Properties

### accountId

• `Optional` **accountId**: ``null`` \| *number*

<div lang=\"ja\">アカウントIDです。</div> 

**`memberof`** AppLink

___

### appId

• `Optional` **appId**: ``null`` \| *string*

<div lang=\"ja\">アプリIDです。<br> ADD時、このフィールドは必須となります。</div> 

**`memberof`** AppLink

___

### appLinkId

• `Optional` **appLinkId**: ``null`` \| *number*

<div lang=\"ja\">アプリリンクIDです。<br> SETまたはREGENERATE時、このフィールドは必須となります。</div> 

**`memberof`** AppLink

___

### appLinkPlatform

• `Optional` **appLinkPlatform**: ``null`` \| [*Android*](./enums/applinkserviceapplinkplatform.md#android) \| [*Unknown*](./enums/applinkserviceapplinkplatform.md#unknown)

**`memberof`** AppLink

___

### appVendorId

• `Optional` **appVendorId**: ``null`` \| *string*

<div lang=\"ja\">アプリ計測ベンダーIDです。<br> ADD時、このフィールドは必須となります。<br> ※DictionaryService/getAppLinkVendorで取得できるappVendorIdのみ使用できます。</div> 

**`memberof`** AppLink

___

### appVendorNameEn

• `Optional` **appVendorNameEn**: ``null`` \| *string*

<div lang=\"ja\">アプリ計測ベンダー名（英語）です。</div> 

**`memberof`** AppLink

___

### appVendorNameJa

• `Optional` **appVendorNameJa**: ``null`` \| *string*

<div lang=\"ja\">アプリ計測ベンダー名（日本語）です。</div> 

**`memberof`** AppLink

___

### linkId

• `Optional` **linkId**: ``null`` \| *string*

<div lang=\"ja\">リンクIDです。</div> 

**`memberof`** AppLink

___

### linkStatus

• `Optional` **linkStatus**: ``null`` \| [*Enabled*](./enums/applinkservicelinkstatus.md#enabled) \| [*Disabled*](./enums/applinkservicelinkstatus.md#disabled) \| [*Unknown*](./enums/applinkservicelinkstatus.md#unknown)

**`memberof`** AppLink

___

### syncStatus

• `Optional` **syncStatus**: ``null`` \| [*InProgress*](./enums/applinkservicesyncstatus.md#inprogress) \| [*Completed*](./enums/applinkservicesyncstatus.md#completed) \| [*Unknown*](./enums/applinkservicesyncstatus.md#unknown)

**`memberof`** AppLink
