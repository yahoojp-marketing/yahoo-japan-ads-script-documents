# AdGroupRetargetingList


<div lang=\"ja\">AdGroupRetargetingListは、広告グループレベルでのターゲットリスト設定を保持するオブジェクトです。</div> 

## Table of contents

### Properties

- [accountId](adgroupretargetinglist.md#accountid)
- [adGroupId](adgroupretargetinglist.md#adgroupid)
- [adGroupName](adgroupretargetinglist.md#adgroupname)
- [bidMultiplier](adgroupretargetinglist.md#bidmultiplier)
- [campaignId](adgroupretargetinglist.md#campaignid)
- [campaignName](adgroupretargetinglist.md#campaignname)
- [criterionTargetList](adgroupretargetinglist.md#criteriontargetlist)
- [excludedType](adgroupretargetinglist.md#excludedtype)

## Properties

### accountId

• `Optional` **accountId**: ``null`` \| *number*

<div lang=\"ja\">アカウントIDです。<br> このフィールドは、レスポンスの際に返却されますが、リクエストの際には無視されます。</div> 

**`memberof`** AdGroupRetargetingList

___

### adGroupId

• `Optional` **adGroupId**: ``null`` \| *number*

<div lang=\"ja\">広告グループIDです。<br> このフィールドは、いずれの場合でも必須です。</div> 

**`memberof`** AdGroupRetargetingList

___

### adGroupName

• `Optional` **adGroupName**: ``null`` \| *string*

<div lang=\"ja\">広告グループ名です。<br> このフィールドは、レスポンスの際に返却されますが、リクエストの際には無視されます。</div> 

**`memberof`** AdGroupRetargetingList

___

### bidMultiplier

• `Optional` **bidMultiplier**: ``null`` \| *number*

<div lang=\"ja\">MaxCPC上昇値です。<br> このフィールドは省略可能となります。その際、デフォルト設定値は1.00となります。</div> 

**`memberof`** AdGroupRetargetingList

___

### campaignId

• `Optional` **campaignId**: ``null`` \| *number*

<div lang=\"ja\">キャンペーンIDです。<br> このフィールドは、いずれの場合でも必須です。</div> 

**`memberof`** AdGroupRetargetingList

___

### campaignName

• `Optional` **campaignName**: ``null`` \| *string*

<div lang=\"ja\">キャンペーン名です。<br> このフィールドは、レスポンスの際に返却されますが、リクエストの際には無視されます。</div> 

**`memberof`** AdGroupRetargetingList

___

### criterionTargetList

• `Optional` **criterionTargetList**: ``null`` \| [*AdGroupRetargetingListServiceCriterionTargetList*](adgroupretargetinglistservicecriteriontargetlist.md)

**`memberof`** AdGroupRetargetingList

___

### excludedType

• `Optional` **excludedType**: ``null`` \| [*Included*](./enums/adgroupretargetinglistserviceexcludedtype.md#included) \| [*Excluded*](./enums/adgroupretargetinglistserviceexcludedtype.md#excluded) \| [*Unknown*](./enums/adgroupretargetinglistserviceexcludedtype.md#unknown)

**`memberof`** AdGroupRetargetingList
