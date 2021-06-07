# BrandLift


<div lang=\"ja\">BrandLiftオブジェクトは、ブランドリフトの情報を表します。</div> 

## Table of contents

### Properties

- [accountId](brandlift.md#accountid)
- [approvalStatus](brandlift.md#approvalstatus)
- [brandLiftId](brandlift.md#brandliftid)
- [campaignId](brandlift.md#campaignid)
- [campaignName](brandlift.md#campaignname)
- [campaignStartDate](brandlift.md#campaignstartdate)
- [disapprovalReason](brandlift.md#disapprovalreason)
- [disapprovalReasonCodes](brandlift.md#disapprovalreasoncodes)
- [notificationBusinessIds](brandlift.md#notificationbusinessids)
- [questions](brandlift.md#questions)
- [reviewCompleteDate](brandlift.md#reviewcompletedate)
- [submitDate](brandlift.md#submitdate)

## Properties

### accountId

• `Optional` **accountId**: ``null`` \| *number*

<div lang=\"ja\">アカウントIDです。</div> 

**`memberof`** BrandLift

___

### approvalStatus

• `Optional` **approvalStatus**: ``null`` \| [*Approved*](./enums/brandliftserviceapprovalstatus.md#approved) \| [*ApprovedWithReview*](./enums/brandliftserviceapprovalstatus.md#approvedwithreview) \| [*Review*](./enums/brandliftserviceapprovalstatus.md#review) \| [*PreDisapproved*](./enums/brandliftserviceapprovalstatus.md#predisapproved) \| [*PostDisapproved*](./enums/brandliftserviceapprovalstatus.md#postdisapproved) \| [*Unknown*](./enums/brandliftserviceapprovalstatus.md#unknown)

**`memberof`** BrandLift

___

### brandLiftId

• `Optional` **brandLiftId**: ``null`` \| *number*

<div lang=\"ja\">ブランドリフト調査IDです。</div> 

**`memberof`** BrandLift

___

### campaignId

• `Optional` **campaignId**: ``null`` \| *number*

<div lang=\"ja\">キャンペーンIDです。</div> 

**`memberof`** BrandLift

___

### campaignName

• `Optional` **campaignName**: ``null`` \| *string*

<div lang=\"ja\">キャンペーン名です。</div> 

**`memberof`** BrandLift

___

### campaignStartDate

• `Optional` **campaignStartDate**: ``null`` \| *string*

<div lang=\"ja\">キャンペーン配信開始日時です。</div>  <br>Format: yyyyMMdd

**`memberof`** BrandLift

___

### disapprovalReason

• `Optional` **disapprovalReason**: ``null`` \| *string*

<div lang=\"ja\">審査否認理由です。</div> 

**`memberof`** BrandLift

___

### disapprovalReasonCodes

• `Optional` **disapprovalReasonCodes**: ``null`` \| *string*[]

<div lang=\"ja\">審査否認理由コードです。</div> 

**`memberof`** BrandLift

___

### notificationBusinessIds

• `Optional` **notificationBusinessIds**: ``null`` \| *string*[]

<div lang=\"ja\">連絡先Yahoo! JAPANビジネスIDです。</div> 

**`memberof`** BrandLift

___

### questions

• `Optional` **questions**: ``null`` \| [*BrandLiftServiceQuestion*](brandliftservicequestion.md)[]

**`memberof`** BrandLift

___

### reviewCompleteDate

• `Optional` **reviewCompleteDate**: ``null`` \| *string*

<div lang=\"ja\">審査完了日時です。</div>  <br>Format: yyyyMMddHHmmss

**`memberof`** BrandLift

___

### submitDate

• `Optional` **submitDate**: ``null`` \| *string*

<div lang=\"ja\">入稿日時です。</div>  <br>Format: yyyyMMddHHmmss

**`memberof`** BrandLift
