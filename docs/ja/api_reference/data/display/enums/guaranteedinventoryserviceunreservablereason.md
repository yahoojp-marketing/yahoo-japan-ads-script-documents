# Enumeration: GuaranteedInventoryServiceUnreservableReason


<div lang=\"ja\"> GuaranteedInventoryServiceUnreservableReasonは、予約ができない理由を表します。<br> このフィールドは、レスポンスの際に返却されますが、リクエストの際には無視されます。 </div>  <dl class=term>   <dt class=\"term__item\">NOT_ENOUGH_DELIVERY_TARGET</dt>   <dd class=\"term__desc\"><span lang=\"ja\">配信対象が少なすぎます。</span></dd>   <dt class=\"term__item\">OUT_OF_STOCK</dt>   <dd class=\"term__desc\"><span lang=\"ja\">配信在庫がありません。</span></dd>   <dt class=\"term__item\">OUT_OF_STOCK</dt>   <dd class=\"term__desc\"><span lang=\"ja\">1日のSOV予約上限に達しています。</span><span lang=\"en\">Number of SOV exceeded the daily limit./span></dd>   <dt class=\"term__item\">OUT_OF_STOCK</dt>   <dd class=\"term__desc\"><span lang=\"ja\">1週間のSOV予約上限に達しています。</span></dd>   <dt class=\"term__item\">UNKNOWN</dt>   <dd class=\"term__desc\"><span lang=\"ja\">未知の値です。</span></dd> </dl>

## Table of contents

### Enumeration members

- [NotEnoughDeliveryTarget](guaranteedinventoryserviceunreservablereason.md#notenoughdeliverytarget)
- [OutOfStock](guaranteedinventoryserviceunreservablereason.md#outofstock)
- [OverSovDailyLimit](guaranteedinventoryserviceunreservablereason.md#oversovdailylimit)
- [OverSovWeeklyLimit](guaranteedinventoryserviceunreservablereason.md#oversovweeklylimit)
- [Unknown](guaranteedinventoryserviceunreservablereason.md#unknown)

## Enumeration members

### NotEnoughDeliveryTarget

• **NotEnoughDeliveryTarget**: = "NOT\_ENOUGH\_DELIVERY\_TARGET"

___

### OutOfStock

• **OutOfStock**: = "OUT\_OF\_STOCK"

___

### OverSovDailyLimit

• **OverSovDailyLimit**: = "OVER\_SOV\_DAILY\_LIMIT"

___

### OverSovWeeklyLimit

• **OverSovWeeklyLimit**: = "OVER\_SOV\_WEEKLY\_LIMIT"

___

### Unknown

• **Unknown**: = "UNKNOWN"
