# AdGroupWebpage


<div lang=\"ja\">AdGroupWebpageオブジェクトは、広告グループに関連付けた配信/除外設定の情報を保持します。</div> 

## Table of contents

### Properties

- [accountId](adgroupwebpage.md#accountid)
- [adGroupId](adgroupwebpage.md#adgroupid)
- [adGroupTrackId](adgroupwebpage.md#adgrouptrackid)
- [bid](adgroupwebpage.md#bid)
- [campaignId](adgroupwebpage.md#campaignid)
- [campaignTrackId](adgroupwebpage.md#campaigntrackid)
- [excludedType](adgroupwebpage.md#excludedtype)
- [userStatus](adgroupwebpage.md#userstatus)
- [webpage](adgroupwebpage.md#webpage)

## Properties

### accountId

• `Optional` **accountId**: ``null`` \| *number*

<div lang=\"ja\">アカウントIDです。<br>このフィールドは、レスポンスの際に返却されますが、リクエストの際には無視されます。</div> 

**`memberof`** AdGroupWebpage

___

### adGroupId

• `Optional` **adGroupId**: ``null`` \| *number*

<div lang=\"ja\">広告グループIDです。<br>このフィールドは、いずれの場合でも必須です。</div> 

**`memberof`** AdGroupWebpage

___

### adGroupTrackId

• `Optional` **adGroupTrackId**: ``null`` \| *number*

<div lang=\"ja\">広告グループトラッキングIDです。<br>このフィールドは、レスポンスの際に返却されますが、リクエストの際には無視されます。</div> 

**`memberof`** AdGroupWebpage

___

### bid

• `Optional` **bid**: ``null`` \| [*AdGroupWebpageServiceBid*](adgroupwebpageservicebid.md)

**`memberof`** AdGroupWebpage

___

### campaignId

• `Optional` **campaignId**: ``null`` \| *number*

<div lang=\"ja\">キャンペーンIDです。<br>このフィールドは、いずれの場合でも必須です。</div> 

**`memberof`** AdGroupWebpage

___

### campaignTrackId

• `Optional` **campaignTrackId**: ``null`` \| *number*

<div lang=\"ja\">キャンペーントラッキングIDです。<br>このフィールドは、レスポンスの際に返却されますが、リクエストの際には無視されます。</div> 

**`memberof`** AdGroupWebpage

___

### excludedType

• `Optional` **excludedType**: ``null`` \| [*Included*](./enums/adgroupwebpageserviceexcludedtype.md#included) \| [*Excluded*](./enums/adgroupwebpageserviceexcludedtype.md#excluded) \| [*Unknown*](./enums/adgroupwebpageserviceexcludedtype.md#unknown)

**`memberof`** AdGroupWebpage

___

### userStatus

• `Optional` **userStatus**: ``null`` \| [*Active*](./enums/adgroupwebpageserviceuserstatus.md#active) \| [*Paused*](./enums/adgroupwebpageserviceuserstatus.md#paused) \| [*Unknown*](./enums/adgroupwebpageserviceuserstatus.md#unknown)

**`memberof`** AdGroupWebpage

___

### webpage

• `Optional` **webpage**: ``null`` \| [*AdGroupWebpageServiceWebpage*](adgroupwebpageservicewebpage.md)

**`memberof`** AdGroupWebpage
