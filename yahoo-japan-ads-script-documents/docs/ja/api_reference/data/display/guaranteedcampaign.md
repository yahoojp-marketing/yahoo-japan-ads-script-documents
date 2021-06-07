# GuaranteedCampaign


<div lang=\"ja\">GuaranteedCampaignオブジェクトは、予約型のキャンペーン情報を表します。</div> 

## Table of contents

### Properties

- [\_package](guaranteedcampaign.md#_package)
- [accountId](guaranteedcampaign.md#accountid)
- [adCategoryStatus](guaranteedcampaign.md#adcategorystatus)
- [brandTracking](guaranteedcampaign.md#brandtracking)
- [campaignBiddingStrategy](guaranteedcampaign.md#campaignbiddingstrategy)
- [campaignCanceledDate](guaranteedcampaign.md#campaigncanceleddate)
- [campaignGoal](guaranteedcampaign.md#campaigngoal)
- [campaignId](guaranteedcampaign.md#campaignid)
- [campaignName](guaranteedcampaign.md#campaignname)
- [endDate](guaranteedcampaign.md#enddate)
- [guaranteedSimulationId](guaranteedcampaign.md#guaranteedsimulationid)
- [labels](guaranteedcampaign.md#labels)
- [lifetimeBudget](guaranteedcampaign.md#lifetimebudget)
- [notificationEmailAddress](guaranteedcampaign.md#notificationemailaddress)
- [servingStatus](guaranteedcampaign.md#servingstatus)
- [startDate](guaranteedcampaign.md#startdate)
- [userStatus](guaranteedcampaign.md#userstatus)
- [viewableFrequencyCap](guaranteedcampaign.md#viewablefrequencycap)

## Properties

### \_package

• `Optional` **\_package**: ``null`` \| [*GuaranteedCampaignServicePackage*](guaranteedcampaignservicepackage.md)

**`memberof`** GuaranteedCampaign

___

### accountId

• `Optional` **accountId**: ``null`` \| *number*

<div lang=\"ja\"> アカウントIDです。<br> このフィールドは、リクエストの場合は必須です。 </div> 

**`memberof`** GuaranteedCampaign

___

### adCategoryStatus

• `Optional` **adCategoryStatus**: ``null`` \| [*Added*](./enums/guaranteedcampaignserviceadcategorystatus.md#added) \| [*None*](./enums/guaranteedcampaignserviceadcategorystatus.md#none) \| [*Unknown*](./enums/guaranteedcampaignserviceadcategorystatus.md#unknown)

**`memberof`** GuaranteedCampaign

___

### brandTracking

• `Optional` **brandTracking**: ``null`` \| [*GuaranteedCampaignServiceBrandTracking*](guaranteedcampaignservicebrandtracking.md)

**`memberof`** GuaranteedCampaign

___

### campaignBiddingStrategy

• `Optional` **campaignBiddingStrategy**: ``null`` \| [*GuaranteedCampaignServiceCampaignBiddingStrategy*](guaranteedcampaignservicecampaignbiddingstrategy.md)

**`memberof`** GuaranteedCampaign

___

### campaignCanceledDate

• `Optional` **campaignCanceledDate**: ``null`` \| *string*

<div lang=\"ja\"> 予約型のキャンペーンをキャンセルした日時です。<br> ※フォーマット：yyyyMMddHHmmss<br> このフィールドは、レスポンスの際に返却されますが、リクエストの際には無視されます。 </div> 

**`memberof`** GuaranteedCampaign

___

### campaignGoal

• `Optional` **campaignGoal**: ``null`` \| *string*

<div lang=\"ja\"> キャンペーン目的です。<br> このフィールドは、レスポンスの際に返却されますが、リクエストの際には無視されます。 </div> 

**`memberof`** GuaranteedCampaign

___

### campaignId

• `Optional` **campaignId**: ``null`` \| *number*

<div lang=\"ja\"> キャンペーンIDです。<br> このフィールドはSET時に必須となります。 </div> 

**`memberof`** GuaranteedCampaign

___

### campaignName

• `Optional` **campaignName**: ``null`` \| *string*

<div lang=\"ja\"> キャンペーン名です。 </div> 

**`memberof`** GuaranteedCampaign

___

### endDate

• `Optional` **endDate**: ``null`` \| *string*

<div lang=\"ja\"> 終了日です。<br> ※フォーマット：yyyyMMdd<br> このフィールドは、レスポンスの際に返却されますが、リクエストの際には無視されます。 </div> 

**`memberof`** GuaranteedCampaign

___

### guaranteedSimulationId

• `Optional` **guaranteedSimulationId**: ``null`` \| *number*

<div lang=\"ja\"> シミュレーションIDです。<br> このフィールドは、レスポンスの際に返却されますが、リクエストの際には無視されます。 </div> 

**`memberof`** GuaranteedCampaign

___

### labels

• `Optional` **labels**: ``null`` \| [*GuaranteedCampaignServiceLabel*](guaranteedcampaignservicelabel.md)[]

**`memberof`** GuaranteedCampaign

___

### lifetimeBudget

• `Optional` **lifetimeBudget**: ``null`` \| [*GuaranteedCampaignServiceLifetimeBudget*](guaranteedcampaignservicelifetimebudget.md)

**`memberof`** GuaranteedCampaign

___

### notificationEmailAddress

• `Optional` **notificationEmailAddress**: ``null`` \| *string*[]

<div lang=\"ja\"> 連絡先メールアドレスです。<br> </div> 

**`memberof`** GuaranteedCampaign

___

### servingStatus

• `Optional` **servingStatus**: ``null`` \| [*Serving*](./enums/guaranteedcampaignserviceservingstatus.md#serving) \| [*Ended*](./enums/guaranteedcampaignserviceservingstatus.md#ended) \| [*Pending*](./enums/guaranteedcampaignserviceservingstatus.md#pending) \| [*Unknown*](./enums/guaranteedcampaignserviceservingstatus.md#unknown)

**`memberof`** GuaranteedCampaign

___

### startDate

• `Optional` **startDate**: ``null`` \| *string*

<div lang=\"ja\"> 開始日です。<br> ※フォーマット：yyyyMMdd<br> このフィールドは、レスポンスの際に返却されますが、リクエストの際には無視されます。 </div> 

**`memberof`** GuaranteedCampaign

___

### userStatus

• `Optional` **userStatus**: ``null`` \| [*Active*](./enums/guaranteedcampaignserviceuserstatus.md#active) \| [*Paused*](./enums/guaranteedcampaignserviceuserstatus.md#paused) \| [*Unknown*](./enums/guaranteedcampaignserviceuserstatus.md#unknown)

**`memberof`** GuaranteedCampaign

___

### viewableFrequencyCap

• `Optional` **viewableFrequencyCap**: ``null`` \| [*GuaranteedCampaignServiceViewableFrequencyCap*](guaranteedcampaignserviceviewablefrequencycap.md)

**`memberof`** GuaranteedCampaign
