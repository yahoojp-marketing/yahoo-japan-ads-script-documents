# CampaignRetargetingListServiceSelector


<div lang=\"ja\">CampaignRetargetingListServiceSelectorオブジェクトは、キャンペーン階層におけるターゲットリストの設定情報を取得するための検索条件（実行パラメータ）を保持します。</div> 

## Table of contents

### Properties

- [accountId](campaignretargetinglistserviceselector.md#accountid)
- [campaignIds](campaignretargetinglistserviceselector.md#campaignids)
- [excludedType](campaignretargetinglistserviceselector.md#excludedtype)
- [numberResults](campaignretargetinglistserviceselector.md#numberresults)
- [startIndex](campaignretargetinglistserviceselector.md#startindex)
- [targetListIds](campaignretargetinglistserviceselector.md#targetlistids)

## Properties

### accountId

• **accountId**: *number*

<div lang=\"ja\">アカウントIDです。</div> 

**`memberof`** CampaignRetargetingListServiceSelector

___

### campaignIds

• `Optional` **campaignIds**: ``null`` \| *number*[]

<div lang=\"ja\">キャンペーンIDです。</div> 

**`memberof`** CampaignRetargetingListServiceSelector

___

### excludedType

• `Optional` **excludedType**: ``null`` \| [*Included*](./enums/campaignretargetinglistserviceexcludedtype.md#included) \| [*Excluded*](./enums/campaignretargetinglistserviceexcludedtype.md#excluded) \| [*Unknown*](./enums/campaignretargetinglistserviceexcludedtype.md#unknown)

**`memberof`** CampaignRetargetingListServiceSelector

___

### numberResults

• `Optional` **numberResults**: ``null`` \| *number*

<div lang=\"ja\">ページの最大件数です。このフィールドは、1以上を指定する必要があります。</div> 

**`memberof`** CampaignRetargetingListServiceSelector

___

### startIndex

• `Optional` **startIndex**: ``null`` \| *number*

<div lang=\"ja\">ページの先頭のインデックスです。このフィールドは、1以上を指定する必要があります。</div> 

**`memberof`** CampaignRetargetingListServiceSelector

___

### targetListIds

• `Optional` **targetListIds**: ``null`` \| *number*[]

<div lang=\"ja\">ターゲットリストIDです。</div> 

**`memberof`** CampaignRetargetingListServiceSelector
