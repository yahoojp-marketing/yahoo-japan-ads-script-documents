# AdGroupCriterionServiceBiddableAdGroupCriterion


<div lang=\"ja\">AdGroupCriterionServiceBiddableAdGroupCriterionオブジェクトは、広告グループの単価設定可能（包含）クライテリアです。</div> 

## Table of contents

### Properties

- [additionalAdvancedMobileUrls](adgroupcriterionservicebiddableadgroupcriterion.md#additionaladvancedmobileurls)
- [additionalAdvancedUrls](adgroupcriterionservicebiddableadgroupcriterion.md#additionaladvancedurls)
- [advancedMobileUrl](adgroupcriterionservicebiddableadgroupcriterion.md#advancedmobileurl)
- [advancedUrl](adgroupcriterionservicebiddableadgroupcriterion.md#advancedurl)
- [approvalStatus](adgroupcriterionservicebiddableadgroupcriterion.md#approvalstatus)
- [bid](adgroupcriterionservicebiddableadgroupcriterion.md#bid)
- [customParameters](adgroupcriterionservicebiddableadgroupcriterion.md#customparameters)
- [destinationUrl](adgroupcriterionservicebiddableadgroupcriterion.md#destinationurl)
- [disapprovalReasonCodes](adgroupcriterionservicebiddableadgroupcriterion.md#disapprovalreasoncodes)
- [reviewAdvancedMobileUrl](adgroupcriterionservicebiddableadgroupcriterion.md#reviewadvancedmobileurl)
- [reviewAdvancedUrl](adgroupcriterionservicebiddableadgroupcriterion.md#reviewadvancedurl)
- [reviewCustomParameters](adgroupcriterionservicebiddableadgroupcriterion.md#reviewcustomparameters)
- [reviewDestinationUrl](adgroupcriterionservicebiddableadgroupcriterion.md#reviewdestinationurl)
- [reviewTrackingUrl](adgroupcriterionservicebiddableadgroupcriterion.md#reviewtrackingurl)
- [trackingUrl](adgroupcriterionservicebiddableadgroupcriterion.md#trackingurl)
- [userStatus](adgroupcriterionservicebiddableadgroupcriterion.md#userstatus)

## Properties

### additionalAdvancedMobileUrls

• `Optional` **additionalAdvancedMobileUrls**: ``null`` \| [*AdGroupCriterionServiceAdditionalAdvancedMobileUrls*](adgroupcriterionserviceadditionaladvancedmobileurls.md)

**`memberof`** AdGroupCriterionServiceBiddableAdGroupCriterion

___

### additionalAdvancedUrls

• `Optional` **additionalAdvancedUrls**: ``null`` \| [*AdGroupCriterionServiceAdditionalAdvancedUrls*](adgroupcriterionserviceadditionaladvancedurls.md)

**`memberof`** AdGroupCriterionServiceBiddableAdGroupCriterion

___

### advancedMobileUrl

• `Optional` **advancedMobileUrl**: ``null`` \| *string*

<div lang=\"ja\">カスタムURL（スマートフォン）です。<br> ADDおよびSET時、このフィールドは省略可能となります。<br> ※空で設定すると、既存のカスタムURL（スマートフォン）は削除されます。</div> 

**`memberof`** AdGroupCriterionServiceBiddableAdGroupCriterion

___

### advancedUrl

• `Optional` **advancedUrl**: ``null`` \| *string*

<div lang=\"ja\">移行後のカスタムURLです。<br> ADDおよびSET時、このフィールドは省略可能となります。※ADD時、移行してtracking Urlを指定している場合は必須となります。<br> ※空で設定すると、既存の移行後のカスタムURLは削除されます。</div> 

**`memberof`** AdGroupCriterionServiceBiddableAdGroupCriterion

___

### approvalStatus

• `Optional` **approvalStatus**: ``null`` \| [*Approved*](./enums/adgroupcriterionserviceapprovalstatus.md#approved) \| [*ApprovedWithReview*](./enums/adgroupcriterionserviceapprovalstatus.md#approvedwithreview) \| [*Review*](./enums/adgroupcriterionserviceapprovalstatus.md#review) \| [*PreDisapproved*](./enums/adgroupcriterionserviceapprovalstatus.md#predisapproved) \| [*PostDisapproved*](./enums/adgroupcriterionserviceapprovalstatus.md#postdisapproved) \| [*Unknown*](./enums/adgroupcriterionserviceapprovalstatus.md#unknown)

**`memberof`** AdGroupCriterionServiceBiddableAdGroupCriterion

___

### bid

• `Optional` **bid**: ``null`` \| [*AdGroupCriterionServiceBid*](adgroupcriterionservicebid.md)

**`memberof`** AdGroupCriterionServiceBiddableAdGroupCriterion

___

### customParameters

• `Optional` **customParameters**: ``null`` \| [*AdGroupCriterionServiceCustomParameters*](adgroupcriterionservicecustomparameters.md)

**`memberof`** AdGroupCriterionServiceBiddableAdGroupCriterion

___

### destinationUrl

• `Optional` **destinationUrl**: ``null`` \| *string*

<div lang=\"ja\">移行前のカスタムURLです。<br> ADDおよびSET時、このフィールドは省略可能となります。<br> ※空で設定すると、既存の移行前のカスタムURLは削除されます。</div> 

**`memberof`** AdGroupCriterionServiceBiddableAdGroupCriterion

___

### disapprovalReasonCodes

• `Optional` **disapprovalReasonCodes**: ``null`` \| *string*[]

<div lang=\"ja\">審査否認コードです。<br> (コード詳細は、DictionaryServiceのgetDisapprovalReasonのレスポンスを参照)</div> 

**`memberof`** AdGroupCriterionServiceBiddableAdGroupCriterion

___

### reviewAdvancedMobileUrl

• `Optional` **reviewAdvancedMobileUrl**: ``null`` \| *string*

<div lang=\"ja\">配信審査中のカスタムURL（スマートフォン）です。</div> 

**`memberof`** AdGroupCriterionServiceBiddableAdGroupCriterion

___

### reviewAdvancedUrl

• `Optional` **reviewAdvancedUrl**: ``null`` \| *string*

<div lang=\"ja\">移行後の配信審査中のカスタムURLです。</div> 

**`memberof`** AdGroupCriterionServiceBiddableAdGroupCriterion

___

### reviewCustomParameters

• `Optional` **reviewCustomParameters**: ``null`` \| [*AdGroupCriterionServiceCustomParameters*](adgroupcriterionservicecustomparameters.md)

**`memberof`** AdGroupCriterionServiceBiddableAdGroupCriterion

___

### reviewDestinationUrl

• `Optional` **reviewDestinationUrl**: ``null`` \| *string*

<div lang=\"ja\">移行前の配信審査中のカスタムURLです。</div> 

**`memberof`** AdGroupCriterionServiceBiddableAdGroupCriterion

___

### reviewTrackingUrl

• `Optional` **reviewTrackingUrl**: ``null`` \| *string*

<div lang=\"ja\">配信審査中のトラッキングURLです。</div> 

**`memberof`** AdGroupCriterionServiceBiddableAdGroupCriterion

___

### trackingUrl

• `Optional` **trackingUrl**: ``null`` \| *string*

<div lang=\"ja\">トラッキングURLです。<br> ADDおよびSET時、このフィールドは省略可能となります。<br> ※空で設定すると、既存のトラッキングURLは削除されます。</div> 

**`memberof`** AdGroupCriterionServiceBiddableAdGroupCriterion

___

### userStatus

• `Optional` **userStatus**: ``null`` \| [*Active*](./enums/adgroupcriterionserviceuserstatus.md#active) \| [*Paused*](./enums/adgroupcriterionserviceuserstatus.md#paused) \| [*Unknown*](./enums/adgroupcriterionserviceuserstatus.md#unknown)

**`memberof`** AdGroupCriterionServiceBiddableAdGroupCriterion
