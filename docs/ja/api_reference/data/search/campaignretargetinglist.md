# CampaignRetargetingList


<div lang=\"ja\">CampaignRetargetingListオブジェクトは、キャンペーン階層におけるターゲットリストの設定情報を保持するオブジェクトです。</div> 

## Table of contents

### Properties

- [accountId](campaignretargetinglist.md#accountid)
- [bidMultiplier](campaignretargetinglist.md#bidmultiplier)
- [campaignId](campaignretargetinglist.md#campaignid)
- [campaignName](campaignretargetinglist.md#campaignname)
- [criterionTargetList](campaignretargetinglist.md#criteriontargetlist)
- [excludedType](campaignretargetinglist.md#excludedtype)

## Properties

### accountId

• `Optional` **accountId**: ``null`` \| *number*

<div lang=\"ja\">アカウントIDです。</div> 

**`memberof`** CampaignRetargetingList

___

### bidMultiplier

• `Optional` **bidMultiplier**: ``null`` \| *number*

<div lang=\"ja\">   入札価格調整率です。0.10～10.00まで指定できます。<br>   0を指定した場合、広告は配信されません。<br>   また、入札価格調整率の値は小数点第二位まで指定可能です。<br>   このフィールドは省略可能となります。その際、デフォルト設定値は1.0となります。 </div> 

**`memberof`** CampaignRetargetingList

___

### campaignId

• `Optional` **campaignId**: ``null`` \| *number*

<div lang=\"ja\">キャンペーンIDです。<br>このフィールドは、いずれの場合でも必須です。</div> 

**`memberof`** CampaignRetargetingList

___

### campaignName

• `Optional` **campaignName**: ``null`` \| *string*

<div lang=\"ja\">キャンペーン名称です。</div> 

**`memberof`** CampaignRetargetingList

___

### criterionTargetList

• `Optional` **criterionTargetList**: ``null`` \| [*CampaignRetargetingListServiceCriterionTargetList*](campaignretargetinglistservicecriteriontargetlist.md)

**`memberof`** CampaignRetargetingList

___

### excludedType

• `Optional` **excludedType**: ``null`` \| [*Included*](./enums/campaignretargetinglistserviceexcludedtype.md#included) \| [*Excluded*](./enums/campaignretargetinglistserviceexcludedtype.md#excluded) \| [*Unknown*](./enums/campaignretargetinglistserviceexcludedtype.md#unknown)

**`memberof`** CampaignRetargetingList
