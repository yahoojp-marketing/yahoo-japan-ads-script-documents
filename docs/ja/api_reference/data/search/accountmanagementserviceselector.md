# AccountManagementServiceSelector


<div lang=\"ja\">AccountManagementServiceSelectorオブジェクトは、選択するアカウントを表します。</div> 

## Table of contents

### Properties

- [accountIds](accountmanagementserviceselector.md#accountids)
- [accountStatuses](accountmanagementserviceselector.md#accountstatuses)
- [accountTypes](accountmanagementserviceselector.md#accounttypes)
- [authType](accountmanagementserviceselector.md#authtype)
- [includeTestAccount](accountmanagementserviceselector.md#includetestaccount)
- [numberResults](accountmanagementserviceselector.md#numberresults)
- [startIndex](accountmanagementserviceselector.md#startindex)

## Properties

### accountIds

• `Optional` **accountIds**: ``null`` \| *number*[]

<div lang=\"ja\">検索条件：アカウントID</div> 

**`memberof`** AccountManagementServiceSelector

___

### accountStatuses

• `Optional` **accountStatuses**: ``null`` \| [*AccountManagementServiceStatus*](./enums/accountmanagementservicestatus.md)[]

<div lang=\"ja\">検索条件：アカウントステータス</div> 

**`memberof`** AccountManagementServiceSelector

___

### accountTypes

• `Optional` **accountTypes**: ``null`` \| [*AccountManagementServicePaymentType*](./enums/accountmanagementservicepaymenttype.md)[]

<div lang=\"ja\">検索条件：アカウントの料金支払い種別</div> 

**`memberof`** AccountManagementServiceSelector

___

### authType

• `Optional` **authType**: ``null`` \| [*Referable*](./enums/accountmanagementserviceauthtype.md#referable) \| [*Updatable*](./enums/accountmanagementserviceauthtype.md#updatable) \| [*Unknown*](./enums/accountmanagementserviceauthtype.md#unknown)

**`memberof`** AccountManagementServiceSelector

___

### includeTestAccount

• `Optional` **includeTestAccount**: ``null`` \| [*OnlyTest*](./enums/accountmanagementserviceincludetestaccount.md#onlytest) \| [*ExcludeTest*](./enums/accountmanagementserviceincludetestaccount.md#excludetest) \| [*All*](./enums/accountmanagementserviceincludetestaccount.md#all) \| [*Unknown*](./enums/accountmanagementserviceincludetestaccount.md#unknown)

**`memberof`** AccountManagementServiceSelector

___

### numberResults

• `Optional` **numberResults**: ``null`` \| *number*

<div lang=\"ja\">ページの最大件数です。このフィールドは、1以上を指定する必要があります。</div> 

**`memberof`** AccountManagementServiceSelector

___

### startIndex

• `Optional` **startIndex**: ``null`` \| *number*

<div lang=\"ja\">ページの先頭のインデックスです。このフィールドは、1以上を指定する必要があります。</div> 

**`memberof`** AccountManagementServiceSelector
