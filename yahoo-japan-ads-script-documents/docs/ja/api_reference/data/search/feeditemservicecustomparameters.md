# FeedItemServiceCustomParameters


<div lang=\"ja\">FeedItemServiceCustomParametersオブジェクトは、カスタムパラメータの設定を表します。<br> CustomParametersおよびReviewCustomParameters配下では、このフィールドはレスポンスの際に返却されますが、リクエストの際には無視されます。<br> ※CustomParameters配下でのみ、クイックリンクオプションの場合、ADDおよびSET時に省略可能となります。</div> 

## Table of contents

### Properties

- [isRemove](feeditemservicecustomparameters.md#isremove)
- [parameters](feeditemservicecustomparameters.md#parameters)

## Properties

### isRemove

• `Optional` **isRemove**: ``null`` \| [*True*](./enums/feeditemserviceisremove.md#true) \| [*False*](./enums/feeditemserviceisremove.md#false) \| [*Unknown*](./enums/feeditemserviceisremove.md#unknown)

**`memberof`** FeedItemServiceCustomParameters

___

### parameters

• `Optional` **parameters**: ``null`` \| [*FeedItemServiceCustomParameter*](feeditemservicecustomparameter.md)[]

**`memberof`** FeedItemServiceCustomParameters
