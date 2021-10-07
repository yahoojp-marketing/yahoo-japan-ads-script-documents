# AdGroup


<div lang=\"ja\">AdGroup オブジェクトは、広告グループを表します。</div> 

## Table of contents

### Properties

- [accountId](adgroup.md#accountid)
- [adGroupAdRotationMode](adgroup.md#adgroupadrotationmode)
- [adGroupId](adgroup.md#adgroupid)
- [adGroupName](adgroup.md#adgroupname)
- [adGroupTrackId](adgroup.md#adgrouptrackid)
- [bid](adgroup.md#bid)
- [campaignId](adgroup.md#campaignid)
- [campaignName](adgroup.md#campaignname)
- [campaignTrackId](adgroup.md#campaigntrackid)
- [createdDate](adgroup.md#createddate)
- [customParameters](adgroup.md#customparameters)
- [labels](adgroup.md#labels)
- [settings](adgroup.md#settings)
- [targetCpaOverride](adgroup.md#targetcpaoverride)
- [targetRoasOverride](adgroup.md#targetroasoverride)
- [trackingUrl](adgroup.md#trackingurl)
- [urlReviewData](adgroup.md#urlreviewdata)
- [userStatus](adgroup.md#userstatus)

## Properties

### accountId

• `Optional` **accountId**: ``null`` \| *number*

<div lang=\"ja\">アカウントIDです。<br> このフィールドは、レスポンスの際に返却されますが、リクエストの際には無視されます。</div> 

**`memberof`** AdGroup

___

### adGroupAdRotationMode

• `Optional` **adGroupAdRotationMode**: ``null`` \| [*AdGroupServiceAdGroupAdRotationMode*](adgroupserviceadgroupadrotationmode.md)

**`memberof`** AdGroup

___

### adGroupId

• `Optional` **adGroupId**: ``null`` \| *number*

<div lang=\"ja\">広告グループIDです。<br> このフィールドは、ADD時は無視され、SETおよびREMOVE時は必須となります。</div> 

**`memberof`** AdGroup

___

### adGroupName

• `Optional` **adGroupName**: ``null`` \| *string*

<div lang=\"ja\">広告グループ名です。<br> このフィールドは、ADD時は必須となり、SET時は省略可能となります。</div> 

**`memberof`** AdGroup

___

### adGroupTrackId

• `Optional` **adGroupTrackId**: ``null`` \| *number*

<div lang=\"ja\">トラッキング用広告グループIDです。<br> このフィールドは、レスポンスの際に返却されますが、リクエストの際には無視されます。</div> 

**`memberof`** AdGroup

___

### bid

• `Optional` **bid**: ``null`` \| [*AdGroupServiceBid*](adgroupservicebid.md)

**`memberof`** AdGroup

___

### campaignId

• `Optional` **campaignId**: ``null`` \| *number*

<div lang=\"ja\">キャンペーンIDです。<br> このフィールドは、いずれの場合でも必須となります。</div> 

**`memberof`** AdGroup

___

### campaignName

• `Optional` **campaignName**: ``null`` \| *string*

<div lang=\"ja\">キャンペーン名です。<br> このフィールドは、レスポンスの際に返却されますが、リクエストの際には無視されます。</div> 

**`memberof`** AdGroup

___

### campaignTrackId

• `Optional` **campaignTrackId**: ``null`` \| *number*

<div lang=\"ja\">トラッキング用キャンペーンIDです。<br> このフィールドは、レスポンスの際に返却されますが、リクエストの際には無視されます。</div> 

**`memberof`** AdGroup

___

### createdDate

• `Optional` **createdDate**: ``null`` \| *string*

<div lang=\"ja\">広告グループが作成された日です。<br>※フォーマット：yyyyMMdd</div> 

**`memberof`** AdGroup

___

### customParameters

• `Optional` **customParameters**: ``null`` \| [*AdGroupServiceCustomParameters*](adgroupservicecustomparameters.md)

**`memberof`** AdGroup

___

### labels

• `Optional` **labels**: ``null`` \| [*AdGroupServiceLabel*](adgroupservicelabel.md)[]

**`memberof`** AdGroup

___

### settings

• `Optional` **settings**: ``null`` \| [*AdGroupServiceSettings*](adgroupservicesettings.md)

**`memberof`** AdGroup

___

### targetCpaOverride

• `Optional` **targetCpaOverride**: ``null`` \| *number*

<div lang=\"ja\">コンバージョン単価の目標値です。<br> キャンペーンで設定したコンバージョン単価の目標値を使用する場合は、0を指定してください。<br> このフィールドは、ADDおよびSET時に省略可能となり、REMOVE時に無視されます。<br> ※キャンペーンのbiddingStrategyTypeが<code>TARGET_CPA</code>または<code>MAXIMIZE_CONVERSIONS</code>の場合に変更可能です。</div> 

**`memberof`** AdGroup

___

### targetRoasOverride

• `Optional` **targetRoasOverride**: ``null`` \| *number*

<div lang=\"ja\">広告費用対効果の目標値です。<br> キャンペーンで設定した広告費用対効果の目標値を使用する場合は、0を指定してください。<br> このフィールドは、ADDおよびSET時に省略可能となり、REMOVE時に無視されます。<br> ※キャンペーンのbiddingStrategyTypeが<code>TARGET_ROAS</code>または<code>MAXIMIZE_CONVERSION_VALUE</code>の場合に変更可能です。</div> 

**`memberof`** AdGroup

___

### trackingUrl

• `Optional` **trackingUrl**: ``null`` \| *string*

<div lang=\"ja\">トラッキングURLです。<br> このフィールドは、省略可能となります。<br> ※キャンペーンがアプリキャンペーンでAndroidの場合、設定はできません。<br> ※SET時、こちらが審査中の場合、編集はできません。また、変更がない場合、審査対象とはなりません。</div> 

**`memberof`** AdGroup

___

### urlReviewData

• `Optional` **urlReviewData**: ``null`` \| [*AdGroupServiceUrlReviewData*](adgroupserviceurlreviewdata.md)

**`memberof`** AdGroup

___

### userStatus

• `Optional` **userStatus**: ``null`` \| [*Active*](./enums/adgroupserviceuserstatus.md#active) \| [*Paused*](./enums/adgroupserviceuserstatus.md#paused) \| [*Unknown*](./enums/adgroupserviceuserstatus.md#unknown)

**`memberof`** AdGroup
