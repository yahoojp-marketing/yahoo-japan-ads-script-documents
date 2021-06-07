# AdGroupTargetServiceDeviceTarget


<div lang=\"ja\"> AdGroupTargetServiceDeviceTargetオブジェクトは、デバイスターゲティングの設定情報を保持します。<br> SET時のみ指定可能です。ADD、REMOVEおよびREPLACE時、このフィールドは無視されます。<br> SET時に必要なtargetIdは、AdGroupオブジェクトにデバイスが設定されている場合にレスポンスされます。<br> ※SET時、入札価格調整率のみ設定可能です。 </div> 

## Table of contents

### Properties

- [deviceType](adgrouptargetservicedevicetarget.md#devicetype)

## Properties

### deviceType

• `Optional` **deviceType**: ``null`` \| [*Desktop*](./enums/adgrouptargetservicedevicetype.md#desktop) \| [*WapMobile*](./enums/adgrouptargetservicedevicetype.md#wapmobile) \| [*Smartphone*](./enums/adgrouptargetservicedevicetype.md#smartphone) \| [*Tablet*](./enums/adgrouptargetservicedevicetype.md#tablet) \| [*Unknown*](./enums/adgrouptargetservicedevicetype.md#unknown)

**`memberof`** AdGroupTargetServiceDeviceTarget
