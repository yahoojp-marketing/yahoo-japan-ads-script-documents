# GuaranteedSimulation


<div lang=\"ja\">GuaranteedSimulationオブジェクトは、予約型キャンペーンの配信シミュレーション情報を保持します。</div> 

## Table of contents

### Properties

- [accountId](guaranteedsimulation.md#accountid)
- [actionAfterVideoAdTap](guaranteedsimulation.md#actionaftervideoadtap)
- [adCategoryIds](guaranteedsimulation.md#adcategoryids)
- [adPlaceType](guaranteedsimulation.md#adplacetype)
- [adRequirements](guaranteedsimulation.md#adrequirements)
- [campaignGoal](guaranteedsimulation.md#campaigngoal)
- [endDate](guaranteedsimulation.md#enddate)
- [guaranteedSimulationId](guaranteedsimulation.md#guaranteedsimulationid)
- [lifetimeBudget](guaranteedsimulation.md#lifetimebudget)
- [lowerBudgetLimit](guaranteedsimulation.md#lowerbudgetlimit)
- [maxReach](guaranteedsimulation.md#maxreach)
- [maxVImps](guaranteedsimulation.md#maxvimps)
- [packageHistoryId](guaranteedsimulation.md#packagehistoryid)
- [packageId](guaranteedsimulation.md#packageid)
- [prediction](guaranteedsimulation.md#prediction)
- [reach](guaranteedsimulation.md#reach)
- [reservationStatus](guaranteedsimulation.md#reservationstatus)
- [slots](guaranteedsimulation.md#slots)
- [sovRate](guaranteedsimulation.md#sovrate)
- [startDate](guaranteedsimulation.md#startdate)
- [targets](guaranteedsimulation.md#targets)
- [unreservableReason](guaranteedsimulation.md#unreservablereason)
- [upperBudgetLimit](guaranteedsimulation.md#upperbudgetlimit)
- [vImps](guaranteedsimulation.md#vimps)
- [viewableFrequencyCap](guaranteedsimulation.md#viewablefrequencycap)

## Properties

### accountId

• `Optional` **accountId**: ``null`` \| *number*

<div lang=\"ja\"> アカウントIDです。<br> このフィールドは、リクエストの場合は必須です。 </div> 

**`memberof`** GuaranteedSimulation

___

### actionAfterVideoAdTap

• `Optional` **actionAfterVideoAdTap**: ``null`` \| [*None*](./enums/guaranteedsimulationserviceactionaftervideoadtap.md#none) \| [*ForView*](./enums/guaranteedsimulationserviceactionaftervideoadtap.md#forview) \| [*ForClick*](./enums/guaranteedsimulationserviceactionaftervideoadtap.md#forclick) \| [*Unknown*](./enums/guaranteedsimulationserviceactionaftervideoadtap.md#unknown)

**`memberof`** GuaranteedSimulation

___

### adCategoryIds

• `Optional` **adCategoryIds**: ``null`` \| *number*[]

<div lang=\"ja\"> 広告カテゴリーIDです。<br> 広告カテゴリーは、配信する広告内容に該当するものを正確に指定して下さい。内容に応じて広告掲載量が変わるため、正確なシミュレーション結果の算出に必要です。<br> 詳細は<a href=\"https://ads-help.yahoo.co.jp/yahooads/guideline/articledetail?lan=ja&aid=50308\" target=\"_blank\">ヘルプ</a>を参照してください。<br> なお、ここで指定した広告カテゴリーと異なる広告が入稿された場合は、入稿した広告内容の修正が必要な旨をメールでご連絡します。<br> ※指定した広告カテゴリーと広告タイプの組み合わせによっては、予約のキャンセルが必要な場合があります。その場合はキャンセル料が発生します。<br> 指定可能な値は、GuaranteedSimulationService/getAdCategoryで取得されるGuaranteedSimulationServiceAdCategoryオブジェクトのadCategoryIdフィールドをご参照ください。<br> ADD時、このフィールドは省略可能となります。 </div> 

**`memberof`** GuaranteedSimulation

___

### adPlaceType

• `Optional` **adPlaceType**: ``null`` \| [*YahooJapanTop*](./enums/guaranteedsimulationserviceadplacetype.md#yahoojapantop) \| [*YahooJapanAll*](./enums/guaranteedsimulationserviceadplacetype.md#yahoojapanall) \| [*YahooJapanExclusionOfTop*](./enums/guaranteedsimulationserviceadplacetype.md#yahoojapanexclusionoftop) \| [*Unknown*](./enums/guaranteedsimulationserviceadplacetype.md#unknown)

**`memberof`** GuaranteedSimulation

___

### adRequirements

• `Optional` **adRequirements**: ``null`` \| [*GuaranteedSimulationServiceAdRequirement*](guaranteedsimulationserviceadrequirement.md)[]

**`memberof`** GuaranteedSimulation

___

### campaignGoal

• `Optional` **campaignGoal**: ``null`` \| *string*

<div lang=\"ja\"> キャンペーン目的です。<br> ADD時、このフィールドは必須となります。<br> ※指定可能な値は、AccountAuthorityServiceのGET操作で得られるAccountAuthorityのauthoritiesフィールドをご確認ください。<br> </div> 

**`memberof`** GuaranteedSimulation

___

### endDate

• `Optional` **endDate**: ``null`` \| *string*

<div lang=\"ja\"> 終了日です。<br> ADD時、このフィールドは必須となります。<br> </div>  Format: yyyyMMdd

**`memberof`** GuaranteedSimulation

___

### guaranteedSimulationId

• `Optional` **guaranteedSimulationId**: ``null`` \| *number*

<div lang=\"ja\"> シミュレーションIDです。<br> このフィールドは、レスポンスの際に返却されますが、リクエストの際には無視されます。 </div> 

**`memberof`** GuaranteedSimulation

___

### lifetimeBudget

• `Optional` **lifetimeBudget**: ``null`` \| *number*

<div lang=\"ja\"> キャンペーンの通期予算額です。<br> ※この「通期予算」は、キャンペーンの全期間を通じて消費される予算を意味します。<br> ADD時、このフィールドは省略可能となります。<br> ※lifetimeBudget, reach, vImps, slotsは同時に設定することができません。 </div> 

**`memberof`** GuaranteedSimulation

___

### lowerBudgetLimit

• `Optional` **lowerBudgetLimit**: ``null`` \| *number*

<div lang=\"ja\"> 予約可能な下限通期予算です。<br> このフィールドは、レスポンスの際に返却されますが、リクエストの際には無視されます。 </div> 

**`memberof`** GuaranteedSimulation

___

### maxReach

• `Optional` **maxReach**: ``null`` \| *number*

<div lang=\"ja\"> 最大リーチ数です。<br> このフィールドは、レスポンスの際に返却されますが、リクエストの際には無視されます。 </div> 

**`memberof`** GuaranteedSimulation

___

### maxVImps

• `Optional` **maxVImps**: ``null`` \| *number*

<div lang=\"ja\"> 最大ビューアブルインプレッション数です。<br> このフィールドは、レスポンスの際に返却されますが、リクエストの際には無視されます。 </div> 

**`memberof`** GuaranteedSimulation

___

### packageHistoryId

• `Optional` **packageHistoryId**: ``null`` \| *number*

<div lang=\"ja\"> 商品履歴IDです。<br> ADD時、このフィールドは省略可能となります。 </div> 

**`memberof`** GuaranteedSimulation

___

### packageId

• `Optional` **packageId**: ``null`` \| *number*

<div lang=\"ja\"> 商品IDです。<br> ADD時、このフィールドは省略可能となります。 </div> 

**`memberof`** GuaranteedSimulation

___

### prediction

• `Optional` **prediction**: ``null`` \| [*GuaranteedSimulationServicePrediction*](guaranteedsimulationserviceprediction.md)

**`memberof`** GuaranteedSimulation

___

### reach

• `Optional` **reach**: ``null`` \| *number*

<div lang=\"ja\"> リーチ数です。<br> ADD時、このフィールドは省略可能となります。<br> ※lifetimeBudget, reach, vImps, slotsは同時に設定することができません。 </div> 

**`memberof`** GuaranteedSimulation

___

### reservationStatus

• `Optional` **reservationStatus**: ``null`` \| [*Reservable*](./enums/guaranteedsimulationservicereservationstatus.md#reservable) \| [*Unreservable*](./enums/guaranteedsimulationservicereservationstatus.md#unreservable) \| [*Reserved*](./enums/guaranteedsimulationservicereservationstatus.md#reserved) \| [*Unknown*](./enums/guaranteedsimulationservicereservationstatus.md#unknown)

**`memberof`** GuaranteedSimulation

___

### slots

• `Optional` **slots**: ``null`` \| *number*

<div lang=\"ja\"> 購入枠数です。<br> ADD時、このフィールドは省略可能となります。<br> ※lifetimeBudget, reach, vImps, slotsは同時に設定することができません。 </div> 

**`memberof`** GuaranteedSimulation

___

### sovRate

• `Optional` **sovRate**: ``null`` \| *number*

<div lang=\"ja\"> SOV（1%〜100%）です。<br> ADD時、このフィールドは省略可能となります。 </div> 

**`memberof`** GuaranteedSimulation

___

### startDate

• `Optional` **startDate**: ``null`` \| *string*

<div lang=\"ja\"> 開始日です。<br> ADD時、このフィールドは必須となります。 </div>  Format: yyyyMMdd

**`memberof`** GuaranteedSimulation

___

### targets

• `Optional` **targets**: ``null`` \| [*GuaranteedSimulationServiceAdGroupTarget*](guaranteedsimulationserviceadgrouptarget.md)[]

**`memberof`** GuaranteedSimulation

___

### unreservableReason

• `Optional` **unreservableReason**: ``null`` \| [*NotEnoughDeliveryTarget*](./enums/guaranteedsimulationserviceunreservablereason.md#notenoughdeliverytarget) \| [*OutOfStock*](./enums/guaranteedsimulationserviceunreservablereason.md#outofstock) \| [*OverSovDailyLimit*](./enums/guaranteedsimulationserviceunreservablereason.md#oversovdailylimit) \| [*OverSovWeeklyLimit*](./enums/guaranteedsimulationserviceunreservablereason.md#oversovweeklylimit) \| [*Unknown*](./enums/guaranteedsimulationserviceunreservablereason.md#unknown)

**`memberof`** GuaranteedSimulation

___

### upperBudgetLimit

• `Optional` **upperBudgetLimit**: ``null`` \| *number*

<div lang=\"ja\"> 予約可能な上限通期予算です。<br> このフィールドは、レスポンスの際に返却されますが、リクエストの際には無視されます。 </div> 

**`memberof`** GuaranteedSimulation

___

### vImps

• `Optional` **vImps**: ``null`` \| *number*

<div lang=\"ja\"> ビューアブルインプレッションです。<br> ADD時、このフィールドは省略可能となります。<br> ※lifetimeBudget, reach, vImps, slotsは同時に設定することができません。 </div> 

**`memberof`** GuaranteedSimulation

___

### viewableFrequencyCap

• `Optional` **viewableFrequencyCap**: ``null`` \| [*GuaranteedSimulationServiceViewableFrequencyCap*](guaranteedsimulationserviceviewablefrequencycap.md)

**`memberof`** GuaranteedSimulation
