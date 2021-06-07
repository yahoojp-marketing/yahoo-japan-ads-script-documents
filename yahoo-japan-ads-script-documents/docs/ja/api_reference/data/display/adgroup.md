# AdGroup


<div lang=\"ja\">AdGroupオブジェクトは、広告グループ情報を保持します。</div> 

## Table of contents

### Properties

- [accountId](adgroup.md#accountid)
- [adGroupBiddingStrategy](adgroup.md#adgroupbiddingstrategy)
- [adGroupId](adgroup.md#adgroupid)
- [adGroupName](adgroup.md#adgroupname)
- [bid](adgroup.md#bid)
- [campaignId](adgroup.md#campaignid)
- [campaignName](adgroup.md#campaignname)
- [conversionOptimizer](adgroup.md#conversionoptimizer)
- [createdDate](adgroup.md#createddate)
- [device](adgroup.md#device)
- [deviceApp](adgroup.md#deviceapp)
- [deviceOs](adgroup.md#deviceos)
- [deviceOsVersion](adgroup.md#deviceosversion)
- [dynamicImageExtensions](adgroup.md#dynamicimageextensions)
- [feedSetId](adgroup.md#feedsetid)
- [labels](adgroup.md#labels)
- [smartDeviceCarriers](adgroup.md#smartdevicecarriers)
- [userStatus](adgroup.md#userstatus)

## Properties

### accountId

• `Optional` **accountId**: ``null`` \| *number*

<div lang=\"ja\"> アカウントIDです。<br> このフィールドは、リクエストの場合は必須です。 </div> 

**`memberof`** AdGroup

___

### adGroupBiddingStrategy

• `Optional` **adGroupBiddingStrategy**: ``null`` \| [*AdGroupServiceBiddingStrategy*](adgroupservicebiddingstrategy.md)

**`memberof`** AdGroup

___

### adGroupId

• `Optional` **adGroupId**: ``null`` \| *number*

<div lang=\"ja\"> 広告グループIDです。<br> このフィールドは、ADD時は無視され、SETおよびREMOVE時は必須となります。 </div> 

**`memberof`** AdGroup

___

### adGroupName

• `Optional` **adGroupName**: ``null`` \| *string*

<div lang=\"ja\"> 広告グループ名です。<br> このフィールドは、ADD時は必須となり、SET時は省略可能となります。 </div> 

**`memberof`** AdGroup

___

### bid

• `Optional` **bid**: ``null`` \| [*AdGroupServiceBid*](adgroupservicebid.md)

**`memberof`** AdGroup

___

### campaignId

• `Optional` **campaignId**: ``null`` \| *number*

<div lang=\"ja\"> キャンペーンIDです。<br> このフィールドは、リクエストの場合は必須です。 </div> 

**`memberof`** AdGroup

___

### campaignName

• `Optional` **campaignName**: ``null`` \| *string*

<div lang=\"ja\"> キャンペーン名です。<br> このフィールドは、レスポンスの際に返却されますが、リクエストの際には無視されます。 </div> 

**`memberof`** AdGroup

___

### conversionOptimizer

• `Optional` **conversionOptimizer**: ``null`` \| [*AdGroupServiceConversionOptimizer*](adgroupserviceconversionoptimizer.md)

**`memberof`** AdGroup

___

### createdDate

• `Optional` **createdDate**: ``null`` \| *string*

<div lang=\"ja\">広告グループが作成された日時です。<br>※フォーマット：yyyyMMdd</div> 

**`memberof`** AdGroup

___

### device

• `Optional` **device**: ``null`` \| [*AdGroupServiceDeviceType*](./enums/adgroupservicedevicetype.md)[]

**`memberof`** AdGroup

___

### deviceApp

• `Optional` **deviceApp**: ``null`` \| [*AdGroupServiceDeviceAppType*](./enums/adgroupservicedeviceapptype.md)[]

**`memberof`** AdGroup

___

### deviceOs

• `Optional` **deviceOs**: ``null`` \| [*AdGroupServiceDeviceOsType*](./enums/adgroupservicedeviceostype.md)[]

**`memberof`** AdGroup

___

### deviceOsVersion

• `Optional` **deviceOsVersion**: ``null`` \| *string*

<div lang=\"ja\"> OSバージョンです。<br> ADDおよびSET時、このフィールドは省略可能となります。<br> ※設定を解除する場合は、NONEを設定してください。 </div> 

**`memberof`** AdGroup

___

### dynamicImageExtensions

• `Optional` **dynamicImageExtensions**: ``null`` \| [*Active*](./enums/adgroupservicedynamicimageextensions.md#active) \| [*Paused*](./enums/adgroupservicedynamicimageextensions.md#paused) \| [*Unknown*](./enums/adgroupservicedynamicimageextensions.md#unknown)

**`memberof`** AdGroup

___

### feedSetId

• `Optional` **feedSetId**: ``null`` \| *number*

<div lang=\"ja\"> 商品セットIDです。<br> ADDおよびSET時、このフィールドは省略可能となります。<br> *ADD時に未指定の場合、デフォルトセットを自動で関連付けます。 </div> 

**`memberof`** AdGroup

___

### labels

• `Optional` **labels**: ``null`` \| [*AdGroupServiceLabel*](adgroupservicelabel.md)[]

**`memberof`** AdGroup

___

### smartDeviceCarriers

• `Optional` **smartDeviceCarriers**: ``null`` \| [*AdGroupServiceSmartDeviceCarrier*](./enums/adgroupservicesmartdevicecarrier.md)[]

**`memberof`** AdGroup

___

### userStatus

• `Optional` **userStatus**: ``null`` \| [*Active*](./enums/adgroupserviceuserstatus.md#active) \| [*Paused*](./enums/adgroupserviceuserstatus.md#paused) \| [*Unknown*](./enums/adgroupserviceuserstatus.md#unknown)

**`memberof`** AdGroup
