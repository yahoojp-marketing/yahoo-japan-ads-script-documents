# AdGroupTargetServiceCarrierTarget


<div lang=\"ja\"> AdGroupTargetServiceCarrierTargetオブジェクトは、モバイルキャリアターゲティングの設定情報を保持します。<br> SET時のみ指定可能です。ADD、REMOVEおよびREPLACE時、このフィールドは無視されます。<br> SET時に必要なtargetIdは、AdGroupオブジェクトにキャリアが設定されている場合にレスポンスされます。<br> ※SET時、入札価格調整率のみ設定可能です。 </div> 

## Table of contents

### Properties

- [carrierType](adgrouptargetservicecarriertarget.md#carriertype)

## Properties

### carrierType

• `Optional` **carrierType**: ``null`` \| [*Docomo*](./enums/adgrouptargetservicecarriertype.md#docomo) \| [*Kddi*](./enums/adgrouptargetservicecarriertype.md#kddi) \| [*Softbank*](./enums/adgrouptargetservicecarriertype.md#softbank) \| [*Ymobile*](./enums/adgrouptargetservicecarriertype.md#ymobile) \| [*Others*](./enums/adgrouptargetservicecarriertype.md#others) \| [*Unknown*](./enums/adgrouptargetservicecarriertype.md#unknown)

**`memberof`** AdGroupTargetServiceCarrierTarget
