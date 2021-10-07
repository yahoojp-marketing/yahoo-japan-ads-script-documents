# CampaignServiceMaximizeConversionValueBiddingScheme


<div lang=\"ja\">CampaignServiceMaximizeConversionValueBiddingSchemeオブジェクトは、広告費用対効果の目標値の自動入札設定情報を表します。<br> ADD時、BiddingStrategyTypeがMAXIMIZE_CONVERSION_VALUEの場合、必須となり、それ以外では省略可能となります。</div> 

## Table of contents

### Properties

- [targetRoas](campaignservicemaximizeconversionvaluebiddingscheme.md#targetroas)

## Properties

### targetRoas

• `Optional` **targetRoas**: ``null`` \| *number*

<div lang=\"ja\">広告費用対効果の目標値です。<br> 0.01 ～ 1000.00（1% ～ 100000%）の範囲内のみ 許容します。<br> ADD時およびSET時、このフィールドは必須となります。<br> ※ROAS:Return On Advertising Spend</div> 

**`memberof`** CampaignServiceMaximizeConversionValueBiddingScheme
