# AuditLogServiceValue


<div lang=\"ja\">AuditLogServiceValueオブジェクトは、get/addメソッドの実行結果（1エンティティ）を保持するオブジェクトです。</div> 

## Table of contents

### Properties

- [auditLogJob](auditlogservicevalue.md#auditlogjob)
- [errors](auditlogservicevalue.md#errors)
- [operationSucceeded](auditlogservicevalue.md#operationsucceeded)

## Properties

### auditLogJob

• `Optional` **auditLogJob**: ``null`` \| [*AuditLogServiceJob*](auditlogservicejob.md)

**`memberof`** AuditLogServiceValue

___

### errors

• `Optional` **errors**: ``null`` \| [*ModelError*](modelerror.md)[]

<div lang=\"ja\">エラー内容です。</div> 

**`memberof`** AuditLogServiceValue

___

### operationSucceeded

• `Optional` **operationSucceeded**: ``null`` \| *boolean*

<div lang=\"ja\">処理結果です。trueの場合は、処理は成功しました。falseの場合は処理が失敗しています。</div> 

**`memberof`** AuditLogServiceValue
