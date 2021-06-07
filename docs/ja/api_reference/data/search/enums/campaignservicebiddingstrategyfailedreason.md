# Enumeration: CampaignServiceBiddingStrategyFailedReason


<div lang=\"ja\">CampaignServiceBiddingStrategyFailedReasonは、自動入札設定の結果（失敗原因）です。<br> このフィールドは、レスポンスの際に返却されますが、リクエストの際には無視されます。</div>  <dl class=term>   <dt class=\"term__item\">FAILURE</dt>   <dd class=\"term__desc\"><span lang=\"ja\">原因不明です。</span></dd>   <dt class=\"term__item\">CONVERSION_TRACKING_NOT_ENABLED</dt>   <dd class=\"term__desc\"><span lang=\"ja\">コンバージョン測定タグが発行されていません。</span></dd>   <dt class=\"term__item\">NOT_ENOUGH_CONVERSIONS</dt>   <dd class=\"term__desc\"><span lang=\"ja\">コンバージョンの情報が十分でありません。</span></dd>   <dt class=\"term__item\">CANNOT_CREATE_CAMPAIGN_WITH_CONVERSION_OPTIMIZER</dt>   <dd class=\"term__desc\"><span lang=\"ja\">コンバージョンオプティマイザーの情報は作成不可です。</span></dd>   <dt class=\"term__item\">BIDDING_STRATEGY_CANNOT_BE_OVERRIDDEN</dt>   <dd class=\"term__desc\"><span lang=\"ja\">自動入札設定の上書きができません。</span></dd>   <dt class=\"term__item\">NOT_CPC_CAMPAIGN</dt>   <dd class=\"term__desc\"><span lang=\"ja\">手動入札ではありません。</span></dd>   <dt class=\"term__item\">UNKNOWN</dt>   <dd class=\"term__desc\"><span lang=\"ja\">未知の値です。</span></dd> </dl>

## Table of contents

### Enumeration members

- [BiddingStrategyCannotBeOverridden](campaignservicebiddingstrategyfailedreason.md#biddingstrategycannotbeoverridden)
- [CannotCreateCampaignWithConversionOptimizer](campaignservicebiddingstrategyfailedreason.md#cannotcreatecampaignwithconversionoptimizer)
- [ConversionTrackingNotEnabled](campaignservicebiddingstrategyfailedreason.md#conversiontrackingnotenabled)
- [Failure](campaignservicebiddingstrategyfailedreason.md#failure)
- [NotCpcCampaign](campaignservicebiddingstrategyfailedreason.md#notcpccampaign)
- [NotEnoughConversions](campaignservicebiddingstrategyfailedreason.md#notenoughconversions)
- [Unknown](campaignservicebiddingstrategyfailedreason.md#unknown)

## Enumeration members

### BiddingStrategyCannotBeOverridden

• **BiddingStrategyCannotBeOverridden**: = "BIDDING\_STRATEGY\_CANNOT\_BE\_OVERRIDDEN"

___

### CannotCreateCampaignWithConversionOptimizer

• **CannotCreateCampaignWithConversionOptimizer**: = "CANNOT\_CREATE\_CAMPAIGN\_WITH\_CONVERSION\_OPTIMIZER"

___

### ConversionTrackingNotEnabled

• **ConversionTrackingNotEnabled**: = "CONVERSION\_TRACKING\_NOT\_ENABLED"

___

### Failure

• **Failure**: = "FAILURE"

___

### NotCpcCampaign

• **NotCpcCampaign**: = "NOT\_CPC\_CAMPAIGN"

___

### NotEnoughConversions

• **NotEnoughConversions**: = "NOT\_ENOUGH\_CONVERSIONS"

___

### Unknown

• **Unknown**: = "UNKNOWN"
