# Enumeration: BiddingStrategyServiceType


<div lang=\"ja\">BiddingStrategyServiceTypeは、自動入札タイプを表します。<br> このフィールドは、biddingScheme配下ではADD時は必須となり、SET時は省略可能となります。</div>  <dl class=term>   <dt class=\"term__item\">TARGET_ROAS</dt>   <dd class=\"term__desc\"><span lang=\"ja\"\">広告費用対効果の目標値です。<br>※キャンペーンの更新時のみ適用可能です。広告グループには現在設定できません。</span><span lang=\"en\">Target ROAS.<br>* Available on updating campaign process. Currently not available for ad group.</span></dd>   <dt class=\"term__item\">TARGET_SPEND</dt>   <dd class=\"term__desc\"><span lang=\"ja\"\">クリック数を最大化します。<br>※キャンペーンに適用可能です。広告グループには現在設定できません。</span><span lang=\"en\">Maximize Clicks.<br>* Applicable for campaign. Currently not available for ad group.</span></dd>   <dt class=\"term__item\">TARGET_CPA</dt>   <dd class=\"term__desc\"><span lang=\"ja\">コンバージョン単価の目標値です。<br>※キャンペーンの更新時のみ適用可能です。広告グループには現在設定できません。</span><span lang=\"en\">Target conversion spend (CPA).<br>* Available on updating campaign process. Currently not available for ad group.</span></dd>   <dt class=\"term__item\">TARGET_IMPRESSION_SHARE</dt>   <dd class=\"term__desc\"><span lang=\"ja\">インプレッションシェアの目標値です。<br>※キャンペーンの更新時のみ適用可能です。広告グループには現在設定できません。</span><span lang=\"en\">Target value of impression share. <br> * Available on updating campaign process. Currently not available for ad group. </span></dd>   <dt class=\"term__item\">UNKNOWN</dt>   <dd class=\"term__desc\"><span lang=\"ja\"\">未知の値です。</span></dd> </dl>

## Table of contents

### Enumeration members

- [TargetCpa](biddingstrategyservicetype.md#targetcpa)
- [TargetImpressionShare](biddingstrategyservicetype.md#targetimpressionshare)
- [TargetRoas](biddingstrategyservicetype.md#targetroas)
- [TargetSpend](biddingstrategyservicetype.md#targetspend)
- [Unknown](biddingstrategyservicetype.md#unknown)

## Enumeration members

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
