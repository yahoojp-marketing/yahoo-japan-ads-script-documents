# CampaignServiceAutoCampaignConversionOptimizer


<div lang=\"ja\">CampaignServiceAutoCampaignConversionOptimizerオブジェクトは、コンバージョン最適化設定情報を表します。</div> 

## Table of contents

### Properties

- [conversionOptimizerEligibilityFlg](campaignserviceautocampaignconversionoptimizer.md#conversionoptimizereligibilityflg)
- [targetCpa](campaignserviceautocampaignconversionoptimizer.md#targetcpa)

## Properties

### conversionOptimizerEligibilityFlg

• `Optional` **conversionOptimizerEligibilityFlg**: ``null`` \| [*Enable*](./enums/campaignserviceconversionoptimizereligibilityflg.md#enable) \| [*Disable*](./enums/campaignserviceconversionoptimizereligibilityflg.md#disable) \| [*Unknown*](./enums/campaignserviceconversionoptimizereligibilityflg.md#unknown)

**`memberof`** CampaignServiceAutoCampaignConversionOptimizer

___

### targetCpa

• `Optional` **targetCpa**: ``null`` \| *number*

<div lang=\"ja\"> コンバージョン単価の目標値です。<br> このフィールドは、SET時に省略可能となり、ADDおよびREMOVE時に無視されます。<br> ※設定範囲：1 - 9,999,999,999<br> ※コンバージョン最適化機能が動作している場合には、手動で設定されている入札設定は無効になります。<br> </div> 

**`memberof`** CampaignServiceAutoCampaignConversionOptimizer
