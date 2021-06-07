# CampaignServiceUrlReviewData


<div lang=\"ja\">CampaignServiceUrlReviewDataオブジェクトは、URLの審査状況を表します。<br> このフィールドは、レスポンスの際に返却されますが、リクエストの際には無視されます。</div> 

## Table of contents

### Properties

- [disapprovalReasonCodes](campaignserviceurlreviewdata.md#disapprovalreasoncodes)
- [disapprovalReviewUrl](campaignserviceurlreviewdata.md#disapprovalreviewurl)
- [inReviewUrl](campaignserviceurlreviewdata.md#inreviewurl)
- [urlApprovalStatus](campaignserviceurlreviewdata.md#urlapprovalstatus)

## Properties

### disapprovalReasonCodes

• `Optional` **disapprovalReasonCodes**: ``null`` \| *string*[]

<div lang=\"ja\">審査否認理由コードです。</div> 

**`memberof`** CampaignServiceUrlReviewData

___

### disapprovalReviewUrl

• `Optional` **disapprovalReviewUrl**: ``null`` \| [*CampaignServiceReviewUrl*](campaignservicereviewurl.md)

**`memberof`** CampaignServiceUrlReviewData

___

### inReviewUrl

• `Optional` **inReviewUrl**: ``null`` \| [*CampaignServiceReviewUrl*](campaignservicereviewurl.md)

**`memberof`** CampaignServiceUrlReviewData

___

### urlApprovalStatus

• `Optional` **urlApprovalStatus**: ``null`` \| [*None*](./enums/campaignserviceurlapprovalstatus.md#none) \| [*Approved*](./enums/campaignserviceurlapprovalstatus.md#approved) \| [*ApprovedWithReview*](./enums/campaignserviceurlapprovalstatus.md#approvedwithreview) \| [*Review*](./enums/campaignserviceurlapprovalstatus.md#review) \| [*Disapproved*](./enums/campaignserviceurlapprovalstatus.md#disapproved) \| [*Unknown*](./enums/campaignserviceurlapprovalstatus.md#unknown)

**`memberof`** CampaignServiceUrlReviewData
