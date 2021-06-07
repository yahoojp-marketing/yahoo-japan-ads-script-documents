# GuaranteedAdGroup


<div lang=\"ja\">GuaranteedAdGroupオブジェクトは、予約型の広告グループ情報を保持します。</div> 

## Table of contents

### Properties

- [accountId](guaranteedadgroup.md#accountid)
- [adGroupId](guaranteedadgroup.md#adgroupid)
- [adGroupName](guaranteedadgroup.md#adgroupname)
- [adGroupTargets](guaranteedadgroup.md#adgrouptargets)
- [campaignId](guaranteedadgroup.md#campaignid)
- [campaignName](guaranteedadgroup.md#campaignname)
- [device](guaranteedadgroup.md#device)
- [deviceApp](guaranteedadgroup.md#deviceapp)
- [deviceOs](guaranteedadgroup.md#deviceos)
- [isCreativeProfile](guaranteedadgroup.md#iscreativeprofile)
- [labels](guaranteedadgroup.md#labels)
- [userStatus](guaranteedadgroup.md#userstatus)

## Properties

### accountId

• `Optional` **accountId**: ``null`` \| *number*

<div lang=\"ja\"> アカウントIDです。<br> このフィールドは、レスポンスの際に返却されますが、リクエストの際には無視されます。 </div> 

**`memberof`** GuaranteedAdGroup

___

### adGroupId

• `Optional` **adGroupId**: ``null`` \| *number*

<div lang=\"ja\"> 広告グループIDです。<br> このフィールドは、レスポンスの際に返却されますが、リクエストの際には無視されます。 </div> 

**`memberof`** GuaranteedAdGroup

___

### adGroupName

• `Optional` **adGroupName**: ``null`` \| *string*

<div lang=\"ja\"> 広告グループ名です。<br> このフィールドは、ADD時は必須となり、SET時は省略可能となります。 </div> 

**`memberof`** GuaranteedAdGroup

___

### adGroupTargets

• `Optional` **adGroupTargets**: ``null`` \| [*AdGroupTarget*](adgrouptarget.md)[]

**`memberof`** GuaranteedAdGroup

___

### campaignId

• `Optional` **campaignId**: ``null`` \| *number*

<div lang=\"ja\"> キャンペーンIDです。<br> このフィールドは、リクエストの場合は必須です。 </div> 

**`memberof`** GuaranteedAdGroup

___

### campaignName

• `Optional` **campaignName**: ``null`` \| *string*

<div lang=\"ja\"> キャンペーン名です。<br> このフィールドは、レスポンスの際に返却されますが、リクエストの際には無視されます。<br> *ADD時、このフィールドは返却されません。 </div> 

**`memberof`** GuaranteedAdGroup

___

### device

• `Optional` **device**: ``null`` \| [*GuaranteedAdGroupServiceDeviceType*](./enums/guaranteedadgroupservicedevicetype.md)[]

**`memberof`** GuaranteedAdGroup

___

### deviceApp

• `Optional` **deviceApp**: ``null`` \| [*GuaranteedAdGroupServiceDeviceAppType*](./enums/guaranteedadgroupservicedeviceapptype.md)[]

**`memberof`** GuaranteedAdGroup

___

### deviceOs

• `Optional` **deviceOs**: ``null`` \| [*GuaranteedAdGroupServiceDeviceOsType*](./enums/guaranteedadgroupservicedeviceostype.md)[]

**`memberof`** GuaranteedAdGroup

___

### isCreativeProfile

• `Optional` **isCreativeProfile**: ``null`` \| *boolean*

<div lang=\"ja\"> trueの場合、クリエイティブプロファイルで追加された広告グループであることを示します。<br> このフィールドは、レスポンスの際に返却されますが、リクエストの際には無視されます。 </div> 

**`memberof`** GuaranteedAdGroup

___

### labels

• `Optional` **labels**: ``null`` \| [*GuaranteedAdGroupServiceLabel*](guaranteedadgroupservicelabel.md)[]

**`memberof`** GuaranteedAdGroup

___

### userStatus

• `Optional` **userStatus**: ``null`` \| [*Active*](./enums/guaranteedadgroupserviceuserstatus.md#active) \| [*Paused*](./enums/guaranteedadgroupserviceuserstatus.md#paused) \| [*Unknown*](./enums/guaranteedadgroupserviceuserstatus.md#unknown)

**`memberof`** GuaranteedAdGroup
