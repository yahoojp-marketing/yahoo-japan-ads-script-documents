# GuaranteedReservationServiceValue


<div lang=\"ja\">GuaranteedReservationServiceValueオブジェクトは、操作結果を含むシミュレーション結果に基づいた予約情報を表します。</div> 

## Table of contents

### Properties

- [adGroup](guaranteedreservationservicevalue.md#adgroup)
- [campaign](guaranteedreservationservicevalue.md#campaign)
- [errors](guaranteedreservationservicevalue.md#errors)
- [operationSucceeded](guaranteedreservationservicevalue.md#operationsucceeded)

## Properties

### adGroup

• `Optional` **adGroup**: ``null`` \| [*GuaranteedAdGroup*](guaranteedadgroup.md)[]

**`memberof`** GuaranteedReservationServiceValue

___

### campaign

• `Optional` **campaign**: ``null`` \| [*GuaranteedCampaign*](guaranteedcampaign.md)

**`memberof`** GuaranteedReservationServiceValue

___

### errors

• `Optional` **errors**: ``null`` \| [*ModelError*](modelerror.md)[]

<div lang=\"ja\">エラー内容です。</div> 

**`memberof`** GuaranteedReservationServiceValue

___

### operationSucceeded

• `Optional` **operationSucceeded**: ``null`` \| *boolean*

<div lang=\"ja\">処理結果です。trueの場合は、処理は成功しました。falseの場合は処理が失敗しています。</div> 

**`memberof`** GuaranteedReservationServiceValue
