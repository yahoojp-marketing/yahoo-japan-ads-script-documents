# Enumeration: CampaignServiceBiddingStrategyType


<div lang=\"ja\">CampaignServiceBiddingStrategyTypeは、自動入札タイプを表します。<br> ADD時、標準入札設定の場合、このフィールドは必須となり、ポートフォリオ入札設定の場合、省略可能となります。</div>  <dl class=term>   <dt class=\"term__item\">MANUAL_CPC</dt>   <dd class=\"term__desc\"><span lang=\"ja\">手動で入札を行います。<br>※キャンペーンに適用可能です。広告グループには現在設定できません。</span><span lang=\"en\">Manual CPC settings<br>* Available in campaign level. Currently not available for ad group.</span></dd>   <dt class=\"term__item\">TARGET_ROAS</dt>   <dd class=\"term__desc\"><span lang=\"ja\">広告費用対効果の目標値です。<br>※ADDおよびSET時、この値は指定できません。</span><span lang=\"en\">Target ROAS.<br>* This value cannot be specified in ADD and SET operation.</span></dd>   <dt class=\"term__item\">TARGET_SPEND</dt>   <dd class=\"term__desc\"><span lang=\"ja\">クリック数を最大化します。<br>※キャンペーンに適用可能です。広告グループには現在設定できません。</span><span lang=\"en\">Maximize Clicks.<br>* Applicable for campaign. Currently not available for ad group.</span></dd>   <dt class=\"term__item\">TARGET_CPA</dt>   <dd class=\"term__desc\"><span lang=\"ja\">コンバージョン単価の目標値です。<br>※ADDおよびSET時、この値は指定できません。</span><span lang=\"en\">Target conversion spend (CPA).<br>* This value cannot be specified in ADD and SET operation.</span></dd>   <dt class=\"term__item\">MAXIMIZE_CONVERSIONS</dt>   <dd class=\"term__desc\"><span lang=\"ja\">コンバージョン数を最大化します。<br>※キャンペーンに適用可能です。広告グループには現在設定できません。</span><span lang=\"en\">Maximize Conversions.<br>* Applicable for campaign. Currently not available for ad group.</span></dd>   <dt class=\"term__item\">MAXIMIZE_CONVERSION_VALUE</dt>   <dd class=\"term__desc\"><span lang=\"ja\">コンバージョン価値を最大化します。<br>※キャンペーンに適用可能です。広告グループには現在設定できません。</span><span lang=\"en\">Maximize Conversions Value.<br>* Applicable for campaign. Currently not available for ad group.</span></dd>   <dt class=\"term__item\">TARGET_IMPRESSION_SHARE</dt>   <dd class=\"term__desc\"><span lang=\"ja\">インプレッションシェアの目標値です。<br>※キャンペーンに適用可能です。広告グループには現在設定できません。</span><span lang=\"en\">Target value of impression share.<br>* Applicable for campaign. Currently not available for ad group.</span></dd>   <dt class=\"term__item\">UNKNOWN</dt>   <dd class=\"term__desc\"><span lang=\"ja\">未知の値です。</span></dd> </dl>

## Table of contents

### Enumeration members

- [ManualCpc](campaignservicebiddingstrategytype.md#manualcpc)
- [MaximizeConversionValue](campaignservicebiddingstrategytype.md#maximizeconversionvalue)
- [MaximizeConversions](campaignservicebiddingstrategytype.md#maximizeconversions)
- [TargetCpa](campaignservicebiddingstrategytype.md#targetcpa)
- [TargetImpressionShare](campaignservicebiddingstrategytype.md#targetimpressionshare)
- [TargetRoas](campaignservicebiddingstrategytype.md#targetroas)
- [TargetSpend](campaignservicebiddingstrategytype.md#targetspend)
- [Unknown](campaignservicebiddingstrategytype.md#unknown)

## Enumeration members

### ManualCpc

• **ManualCpc**: = "MANUAL\_CPC"

___

### MaximizeConversionValue

• **MaximizeConversionValue**: = "MAXIMIZE\_CONVERSION\_VALUE"

___

### MaximizeConversions

• **MaximizeConversions**: = "MAXIMIZE\_CONVERSIONS"

___

### TargetCpa

• **TargetCpa**: = "TARGET\_CPA"

___

### TargetImpressionShare

• **TargetImpressionShare**: = "TARGET\_IMPRESSION\_SHARE"

___

### TargetRoas

• **TargetRoas**: = "TARGET\_ROAS"

___

### TargetSpend

• **TargetSpend**: = "TARGET\_SPEND"

___

### Unknown

• **Unknown**: = "UNKNOWN"
