# GuaranteedInventoryServiceInventory


<div lang=\"ja\">GuaranteedInventoryオブジェクトは、予約型キャンペーンの配信シミュレーション情報を保持します。</div> 

## Table of contents

### Properties

- [accountId](guaranteedinventoryserviceinventory.md#accountid)
- [actionAfterVideoAdTap](guaranteedinventoryserviceinventory.md#actionaftervideoadtap)
- [adCategoryIds](guaranteedinventoryserviceinventory.md#adcategoryids)
- [adRequirements](guaranteedinventoryserviceinventory.md#adrequirements)
- [campaignBiddingStrategyType](guaranteedinventoryserviceinventory.md#campaignbiddingstrategytype)
- [campaignGoal](guaranteedinventoryserviceinventory.md#campaigngoal)
- [endDate](guaranteedinventoryserviceinventory.md#enddate)
- [inventoryDetailStatus](guaranteedinventoryserviceinventory.md#inventorydetailstatus)
- [inventoryResult](guaranteedinventoryserviceinventory.md#inventoryresult)
- [inventoryUnit](guaranteedinventoryserviceinventory.md#inventoryunit)
- [lifetimeBudget](guaranteedinventoryserviceinventory.md#lifetimebudget)
- [lowerBudgetLimit](guaranteedinventoryserviceinventory.md#lowerbudgetlimit)
- [maxReservableSlots](guaranteedinventoryserviceinventory.md#maxreservableslots)
- [maxReservableVImps](guaranteedinventoryserviceinventory.md#maxreservablevimps)
- [maxSellableReach](guaranteedinventoryserviceinventory.md#maxsellablereach)
- [maxSellableVImps](guaranteedinventoryserviceinventory.md#maxsellablevimps)
- [maximumPurchaseVImps](guaranteedinventoryserviceinventory.md#maximumpurchasevimps)
- [minimumPurchaseVImps](guaranteedinventoryserviceinventory.md#minimumpurchasevimps)
- [packageHistoryId](guaranteedinventoryserviceinventory.md#packagehistoryid)
- [packageId](guaranteedinventoryserviceinventory.md#packageid)
- [packageName](guaranteedinventoryserviceinventory.md#packagename)
- [placementMonopolyFlg](guaranteedinventoryserviceinventory.md#placementmonopolyflg)
- [predictionResults](guaranteedinventoryserviceinventory.md#predictionresults)
- [priceType](guaranteedinventoryserviceinventory.md#pricetype)
- [promotionUrl](guaranteedinventoryserviceinventory.md#promotionurl)
- [reach](guaranteedinventoryserviceinventory.md#reach)
- [requestedConditionPredictionResult](guaranteedinventoryserviceinventory.md#requestedconditionpredictionresult)
- [reservationStatus](guaranteedinventoryserviceinventory.md#reservationstatus)
- [slots](guaranteedinventoryserviceinventory.md#slots)
- [sovRate](guaranteedinventoryserviceinventory.md#sovrate)
- [startDate](guaranteedinventoryserviceinventory.md#startdate)
- [targets](guaranteedinventoryserviceinventory.md#targets)
- [unreservableReason](guaranteedinventoryserviceinventory.md#unreservablereason)
- [upperBudgetLimit](guaranteedinventoryserviceinventory.md#upperbudgetlimit)
- [vImps](guaranteedinventoryserviceinventory.md#vimps)
- [viewableFrequencyCap](guaranteedinventoryserviceinventory.md#viewablefrequencycap)

## Properties

### accountId

• `Optional` **accountId**: ``null`` \| *number*

<div lang=\"ja\"> アカウントIDです。<br> ADD時、このフィールドは省略可能となります。 </div> 

**`memberof`** GuaranteedInventoryServiceInventory

___

### actionAfterVideoAdTap

• `Optional` **actionAfterVideoAdTap**: ``null`` \| [*None*](./enums/guaranteedinventoryserviceactionaftervideoadtap.md#none) \| [*ForView*](./enums/guaranteedinventoryserviceactionaftervideoadtap.md#forview) \| [*ForClick*](./enums/guaranteedinventoryserviceactionaftervideoadtap.md#forclick) \| [*Unknown*](./enums/guaranteedinventoryserviceactionaftervideoadtap.md#unknown)

**`memberof`** GuaranteedInventoryServiceInventory

___

### adCategoryIds

• `Optional` **adCategoryIds**: ``null`` \| *number*[]

<div lang=\"ja\"> 広告カテゴリーIDです。<br> 広告カテゴリーは、配信する広告内容に該当するものを正確に指定して下さい。内容に応じて広告掲載量が変わるため、正確なシミュレーション結果の算出に必要です。<br> 詳細は<a href=\"https://ads-help.yahoo.co.jp/yahooads/guideline/articledetail?lan=ja&aid=50308\" target=\"_blank\">ヘルプ</a>を参照してください。<br> なお、ここで指定した広告カテゴリーと異なる広告が入稿された場合は、入稿した広告内容の修正が必要な旨をメールでご連絡します。<br> ADD時、このフィールドは省略可能となります。 </div> 

**`memberof`** GuaranteedInventoryServiceInventory

___

### adRequirements

• `Optional` **adRequirements**: ``null`` \| [*GuaranteedInventoryServiceAdRequirement*](guaranteedinventoryserviceadrequirement.md)[]

**`memberof`** GuaranteedInventoryServiceInventory

___

### campaignBiddingStrategyType

• `Optional` **campaignBiddingStrategyType**: ``null`` \| [*MaxVcpm*](./enums/guaranteedinventoryservicecampaignbiddingstrategytype.md#maxvcpm) \| [*Sov*](./enums/guaranteedinventoryservicecampaignbiddingstrategytype.md#sov) \| [*Unknown*](./enums/guaranteedinventoryservicecampaignbiddingstrategytype.md#unknown)

**`memberof`** GuaranteedInventoryServiceInventory

___

### campaignGoal

• `Optional` **campaignGoal**: ``null`` \| *string*

<div lang=\"ja\"> キャンペーン目的です。<br> このフィールドは、レスポンスの際に返却されますが、リクエストの際には無視されます。 </div> 

**`memberof`** GuaranteedInventoryServiceInventory

___

### endDate

• `Optional` **endDate**: ``null`` \| *string*

<div lang=\"ja\"> キャンペーンの終了日です。<br> ADD時、このフィールドは必須となります。<br> </div>  Format: yyyyMMdd

**`memberof`** GuaranteedInventoryServiceInventory

___

### inventoryDetailStatus

• `Optional` **inventoryDetailStatus**: ``null`` \| [*Wait*](./enums/guaranteedinventoryserviceinventorydetailstatus.md#wait) \| [*Succeeded*](./enums/guaranteedinventoryserviceinventorydetailstatus.md#succeeded) \| [*Failed*](./enums/guaranteedinventoryserviceinventorydetailstatus.md#failed) \| [*Unknown*](./enums/guaranteedinventoryserviceinventorydetailstatus.md#unknown)

**`memberof`** GuaranteedInventoryServiceInventory

___

### inventoryResult

• `Optional` **inventoryResult**: ``null`` \| [*GuaranteedInventoryServiceInventoryResult*](guaranteedinventoryserviceinventoryresult.md)[]

**`memberof`** GuaranteedInventoryServiceInventory

___

### inventoryUnit

• `Optional` **inventoryUnit**: ``null`` \| [*Daily*](./enums/guaranteedinventoryserviceinventoryunit.md#daily) \| [*Weekly*](./enums/guaranteedinventoryserviceinventoryunit.md#weekly) \| [*Monthly*](./enums/guaranteedinventoryserviceinventoryunit.md#monthly) \| [*Lifetime*](./enums/guaranteedinventoryserviceinventoryunit.md#lifetime) \| [*Unknown*](./enums/guaranteedinventoryserviceinventoryunit.md#unknown)

**`memberof`** GuaranteedInventoryServiceInventory

___

### lifetimeBudget

• `Optional` **lifetimeBudget**: ``null`` \| *number*

<div lang=\"ja\"> キャンペーンの通期予算額です。<br> ※この「通期予算」は、キャンペーンの全期間を通じて消費される予算を意味します。<br> このフィールドは、レスポンスの際に返却されますが、リクエストの際には無視されます。 </div> 

**`memberof`** GuaranteedInventoryServiceInventory

___

### lowerBudgetLimit

• `Optional` **lowerBudgetLimit**: ``null`` \| *number*

<div lang=\"ja\"> 予約可能な下限通期予算です。<br> このフィールドは、レスポンスの際に返却されますが、リクエストの際には無視されます。 </div> 

**`memberof`** GuaranteedInventoryServiceInventory

___

### maxReservableSlots

• `Optional` **maxReservableSlots**: ``null`` \| *number*

<div lang=\"ja\"> 最大予約可能枠数です。<br> このフィールドは、レスポンスの際に返却されますが、リクエストの際には無視されます。 </div> 

**`memberof`** GuaranteedInventoryServiceInventory

___

### maxReservableVImps

• `Optional` **maxReservableVImps**: ``null`` \| *number*

<div lang=\"ja\"> 指定された条件で予約可能な最大配信量です。<br> このフィールドは、レスポンスの際に返却されますが、リクエストの際には無視されます。 </div> 

**`memberof`** GuaranteedInventoryServiceInventory

___

### maxSellableReach

• `Optional` **maxSellableReach**: ``null`` \| *number*

<div lang=\"ja\"> 販売可能な最大リーチ数です。<br> このフィールドは、レスポンスの際に返却されますが、リクエストの際には無視されます。 </div> 

**`memberof`** GuaranteedInventoryServiceInventory

___

### maxSellableVImps

• `Optional` **maxSellableVImps**: ``null`` \| *number*

<div lang=\"ja\"> 販売可能な最大ビューアブルインプレッション数です。<br> このフィールドは、レスポンスの際に返却されますが、リクエストの際には無視されます。 </div> 

**`memberof`** GuaranteedInventoryServiceInventory

___

### maximumPurchaseVImps

• `Optional` **maximumPurchaseVImps**: ``null`` \| *number*

<div lang=\"ja\">最大購入ビューアブルインプレッション数を表します。</div> 

**`memberof`** GuaranteedInventoryServiceInventory

___

### minimumPurchaseVImps

• `Optional` **minimumPurchaseVImps**: ``null`` \| *number*

<div lang=\"ja\">最低購入ビューアブルインプレッション数を表します。</div> 

**`memberof`** GuaranteedInventoryServiceInventory

___

### packageHistoryId

• `Optional` **packageHistoryId**: ``null`` \| *number*

<div lang=\"ja\"> 商品履歴IDです。<br> ADD時、このフィールドは必須となります。 </div> 

**`memberof`** GuaranteedInventoryServiceInventory

___

### packageId

• `Optional` **packageId**: ``null`` \| *number*

<div lang=\"ja\"> 商品IDです。<br> ADD時、このフィールドは必須となります。 </div> 

**`memberof`** GuaranteedInventoryServiceInventory

___

### packageName

• `Optional` **packageName**: ``null`` \| *string*

<div lang=\"ja\"> 商品名です。<br> このフィールドは、レスポンスの際に返却されますが、リクエストの際には無視されます。 </div> 

**`memberof`** GuaranteedInventoryServiceInventory

___

### placementMonopolyFlg

• `Optional` **placementMonopolyFlg**: ``null`` \| [*False*](./enums/guaranteedinventoryserviceplacementmonopolyflg.md#false) \| [*True*](./enums/guaranteedinventoryserviceplacementmonopolyflg.md#true) \| [*Unknown*](./enums/guaranteedinventoryserviceplacementmonopolyflg.md#unknown)

**`memberof`** GuaranteedInventoryServiceInventory

___

### predictionResults

• `Optional` **predictionResults**: ``null`` \| [*GuaranteedInventoryServicePredictionResult*](guaranteedinventoryservicepredictionresult.md)[]

**`memberof`** GuaranteedInventoryServiceInventory

___

### priceType

• `Optional` **priceType**: ``null`` \| [*VimpsCustom*](./enums/guaranteedinventoryservicepricetype.md#vimpscustom) \| [*VimpsSov*](./enums/guaranteedinventoryservicepricetype.md#vimpssov) \| [*VimpsReach*](./enums/guaranteedinventoryservicepricetype.md#vimpsreach) \| [*Slots*](./enums/guaranteedinventoryservicepricetype.md#slots) \| [*Unknown*](./enums/guaranteedinventoryservicepricetype.md#unknown)

**`memberof`** GuaranteedInventoryServiceInventory

___

### promotionUrl

• `Optional` **promotionUrl**: ``null`` \| *string*

<div lang=\"ja\">表示URLです。<br> ADD時、このフィールドは省略可能となります。</div> 

**`memberof`** GuaranteedInventoryServiceInventory

___

### reach

• `Optional` **reach**: ``null`` \| *number*

<div lang=\"ja\"> リーチ数です。<br> このフィールドは、レスポンスの際に返却されますが、リクエストの際には無視されます。 </div> 

**`memberof`** GuaranteedInventoryServiceInventory

___

### requestedConditionPredictionResult

• `Optional` **requestedConditionPredictionResult**: ``null`` \| [*GuaranteedInventoryServicePredictionResult*](guaranteedinventoryservicepredictionresult.md)

**`memberof`** GuaranteedInventoryServiceInventory

___

### reservationStatus

• `Optional` **reservationStatus**: ``null`` \| [*Reservable*](./enums/guaranteedinventoryservicereservationstatus.md#reservable) \| [*Unreservable*](./enums/guaranteedinventoryservicereservationstatus.md#unreservable) \| [*Reserved*](./enums/guaranteedinventoryservicereservationstatus.md#reserved) \| [*Unknown*](./enums/guaranteedinventoryservicereservationstatus.md#unknown)

**`memberof`** GuaranteedInventoryServiceInventory

___

### slots

• `Optional` **slots**: ``null`` \| *number*

<div lang=\"ja\"> 購入枠数です。<br> このフィールドは、レスポンスの際に返却されますが、リクエストの際には無視されます。 </div> 

**`memberof`** GuaranteedInventoryServiceInventory

___

### sovRate

• `Optional` **sovRate**: ``null`` \| *number*

<div lang=\"ja\"> SOV（1%〜100%）です。<br> このフィールドは、レスポンスの際に返却されますが、リクエストの際には無視されます。 </div> 

**`memberof`** GuaranteedInventoryServiceInventory

___

### startDate

• `Optional` **startDate**: ``null`` \| *string*

<div lang=\"ja\"> キャンペーンの開始日です。<br> ADD時、このフィールドは必須となります。 </div>  Format: yyyyMMdd

**`memberof`** GuaranteedInventoryServiceInventory

___

### targets

• `Optional` **targets**: ``null`` \| [*GuaranteedInventoryServiceAdGroupTarget*](guaranteedinventoryserviceadgrouptarget.md)[]

**`memberof`** GuaranteedInventoryServiceInventory

___

### unreservableReason

• `Optional` **unreservableReason**: ``null`` \| [*NotEnoughDeliveryTarget*](./enums/guaranteedinventoryserviceunreservablereason.md#notenoughdeliverytarget) \| [*OutOfStock*](./enums/guaranteedinventoryserviceunreservablereason.md#outofstock) \| [*OverSovDailyLimit*](./enums/guaranteedinventoryserviceunreservablereason.md#oversovdailylimit) \| [*OverSovWeeklyLimit*](./enums/guaranteedinventoryserviceunreservablereason.md#oversovweeklylimit) \| [*Unknown*](./enums/guaranteedinventoryserviceunreservablereason.md#unknown)

**`memberof`** GuaranteedInventoryServiceInventory

___

### upperBudgetLimit

• `Optional` **upperBudgetLimit**: ``null`` \| *number*

<div lang=\"ja\"> 予約可能な上限通期予算です。<br> このフィールドは、レスポンスの際に返却されますが、リクエストの際には無視されます。 </div> 

**`memberof`** GuaranteedInventoryServiceInventory

___

### vImps

• `Optional` **vImps**: ``null`` \| *number*

<div lang=\"ja\"> ビューアブルインプレッションです。<br> このフィールドは、レスポンスの際に返却されますが、リクエストの際には無視されます。 </div> 

**`memberof`** GuaranteedInventoryServiceInventory

___

### viewableFrequencyCap

• `Optional` **viewableFrequencyCap**: ``null`` \| [*GuaranteedInventoryServiceViewableFrequencyCap*](guaranteedinventoryserviceviewablefrequencycap.md)

**`memberof`** GuaranteedInventoryServiceInventory
