# AdGroupServiceAutoConversionOptimizer


<div lang=\"ja\"> AdGroupServiceAutoConversionOptimizerオブジェクトは、コンバージョン最適化設定情報を表します。<br> SET時、このフィールドは省略可能となります。<br> ADD時、このフィールドは指定できません。 </div> 

## Table of contents

### Properties

- [eligibilityFlg](adgroupserviceautoconversionoptimizer.md#eligibilityflg)
- [targetCpa](adgroupserviceautoconversionoptimizer.md#targetcpa)

## Properties

### eligibilityFlg

• `Optional` **eligibilityFlg**: ``null`` \| [*Enable*](./enums/adgroupserviceeligibilityflg.md#enable) \| [*Disable*](./enums/adgroupserviceeligibilityflg.md#disable) \| [*Unknown*](./enums/adgroupserviceeligibilityflg.md#unknown)

**`memberof`** AdGroupServiceAutoConversionOptimizer

___

### targetCpa

• `Optional` **targetCpa**: ``null`` \| *number*

<div lang=\"ja\"> コンバージョン単価の目標値です。<br> SET時、このフィールドは省略可能となります。<br> ADD時、このフィールドは指定できません。<br> ※設定範囲は1 - 9,999,999,999です。<br> ※コンバージョン最適化機能が動作している場合には、手動で設定されている入札設定は無効になります。 </div> 

**`memberof`** AdGroupServiceAutoConversionOptimizer
