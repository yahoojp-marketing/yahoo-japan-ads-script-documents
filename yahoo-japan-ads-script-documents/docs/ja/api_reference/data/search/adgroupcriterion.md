# AdGroupCriterion


<div lang=\"ja\">AdGroupCriterionオブジェクトは、広告グループのクライテリアを表します。</div> 

## Table of contents

### Properties

- [accountId](adgroupcriterion.md#accountid)
- [adGroupId](adgroupcriterion.md#adgroupid)
- [adGroupName](adgroupcriterion.md#adgroupname)
- [adGroupTrackId](adgroupcriterion.md#adgrouptrackid)
- [biddableAdGroupCriterion](adgroupcriterion.md#biddableadgroupcriterion)
- [campaignId](adgroupcriterion.md#campaignid)
- [campaignName](adgroupcriterion.md#campaignname)
- [campaignTrackId](adgroupcriterion.md#campaigntrackid)
- [criterion](adgroupcriterion.md#criterion)
- [invalidedTrademarks](adgroupcriterion.md#invalidedtrademarks)
- [labels](adgroupcriterion.md#labels)
- [trademarkStatus](adgroupcriterion.md#trademarkstatus)
- [use](adgroupcriterion.md#use)

## Properties

### accountId

• `Optional` **accountId**: ``null`` \| *number*

<div lang=\"ja\">アカウントIDです。</div> 

**`memberof`** AdGroupCriterion

___

### adGroupId

• `Optional` **adGroupId**: ``null`` \| *number*

<div lang=\"ja\">広告グループIDです。<br> このフィールドは、いずれの場合でも必須となります。</div> 

**`memberof`** AdGroupCriterion

___

### adGroupName

• `Optional` **adGroupName**: ``null`` \| *string*

<div lang=\"ja\">広告グループ名です。</div> 

**`memberof`** AdGroupCriterion

___

### adGroupTrackId

• `Optional` **adGroupTrackId**: ``null`` \| *number*

<div lang=\"ja\">トラッキング用広告グループIDです。</div> 

**`memberof`** AdGroupCriterion

___

### biddableAdGroupCriterion

• `Optional` **biddableAdGroupCriterion**: ``null`` \| [*AdGroupCriterionServiceBiddableAdGroupCriterion*](adgroupcriterionservicebiddableadgroupcriterion.md)

**`memberof`** AdGroupCriterion

___

### campaignId

• `Optional` **campaignId**: ``null`` \| *number*

<div lang=\"ja\">キャンペーンIDです。<br> このフィールドは、いずれの場合でも必須となります。</div> 

**`memberof`** AdGroupCriterion

___

### campaignName

• `Optional` **campaignName**: ``null`` \| *string*

<div lang=\"ja\">キャンペーン名です。</div> 

**`memberof`** AdGroupCriterion

___

### campaignTrackId

• `Optional` **campaignTrackId**: ``null`` \| *number*

<div lang=\"ja\">トラッキング用キャンペーンIDです。</div> 

**`memberof`** AdGroupCriterion

___

### criterion

• `Optional` **criterion**: ``null`` \| [*AdGroupCriterionServiceCriterion*](adgroupcriterionservicecriterion.md)

**`memberof`** AdGroupCriterion

___

### invalidedTrademarks

• `Optional` **invalidedTrademarks**: ``null`` \| *string*[]

<div lang=\"ja\">制限された商標です。<br> このフィールドは、レスポンスの際に返却されますが、リクエストの際には無視されます。 </div> 

**`memberof`** AdGroupCriterion

___

### labels

• `Optional` **labels**: ``null`` \| [*AdGroupCriterionServiceLabel*](adgroupcriterionservicelabel.md)[]

**`memberof`** AdGroupCriterion

___

### trademarkStatus

• `Optional` **trademarkStatus**: ``null`` \| [*NoRestriction*](./enums/adgroupcriterionservicetrademarkstatus.md#norestriction) \| [*ConflictWithTrademark*](./enums/adgroupcriterionservicetrademarkstatus.md#conflictwithtrademark) \| [*ClaimInProgress*](./enums/adgroupcriterionservicetrademarkstatus.md#claiminprogress) \| [*DisapprovedClaim*](./enums/adgroupcriterionservicetrademarkstatus.md#disapprovedclaim) \| [*DisapprovedReviewer*](./enums/adgroupcriterionservicetrademarkstatus.md#disapprovedreviewer) \| [*Unknown*](./enums/adgroupcriterionservicetrademarkstatus.md#unknown)

**`memberof`** AdGroupCriterion

___

### use

• `Optional` **use**: ``null`` \| [*Biddable*](./enums/adgroupcriterionserviceuse.md#biddable) \| [*Negative*](./enums/adgroupcriterionserviceuse.md#negative) \| [*Unknown*](./enums/adgroupcriterionserviceuse.md#unknown)

**`memberof`** AdGroupCriterion
