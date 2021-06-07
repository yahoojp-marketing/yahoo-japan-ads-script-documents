# AccountServiceSelector


<div lang=\"ja\">AccountServiceSelectorオブジェクトは、選択するアカウントを表します。</div> 

## Table of contents

### Properties

- [accountIds](accountserviceselector.md#accountids)
- [accountName](accountserviceselector.md#accountname)
- [accountStatuses](accountserviceselector.md#accountstatuses)
- [accountTypes](accountserviceselector.md#accounttypes)
- [authType](accountserviceselector.md#authtype)
- [includeManagerAccount](accountserviceselector.md#includemanageraccount)
- [includeTestAccount](accountserviceselector.md#includetestaccount)
- [numberResults](accountserviceselector.md#numberresults)
- [startIndex](accountserviceselector.md#startindex)

## Properties

### accountIds

• `Optional` **accountIds**: ``null`` \| *number*[]

<div lang=\"ja\">アカウントIDの配列です。</div> 

**`memberof`** AccountServiceSelector

___

### accountName

• `Optional` **accountName**: ``null`` \| *string*

<div lang=\"ja\">アカウント名です。</div> 

**`memberof`** AccountServiceSelector

___

### accountStatuses

• `Optional` **accountStatuses**: ``null`` \| [*AccountServiceStatus*](./enums/accountservicestatus.md)[]

**`memberof`** AccountServiceSelector

___

### accountTypes

• `Optional` **accountTypes**: ``null`` \| [*AccountServiceType*](./enums/accountservicetype.md)[]

**`memberof`** AccountServiceSelector

___

### authType

• `Optional` **authType**: ``null`` \| [*Referable*](./enums/accountserviceauthtype.md#referable) \| [*Updatable*](./enums/accountserviceauthtype.md#updatable) \| [*Unknown*](./enums/accountserviceauthtype.md#unknown)

**`memberof`** AccountServiceSelector

___

### includeManagerAccount

• `Optional` **includeManagerAccount**: ``null`` \| [*OnlyManager*](./enums/accountserviceincludemanageraccount.md#onlymanager) \| [*ExcludeManager*](./enums/accountserviceincludemanageraccount.md#excludemanager) \| [*All*](./enums/accountserviceincludemanageraccount.md#all) \| [*Unknown*](./enums/accountserviceincludemanageraccount.md#unknown)

**`memberof`** AccountServiceSelector

___

### includeTestAccount

• `Optional` **includeTestAccount**: ``null`` \| [*OnlyTest*](./enums/accountserviceincludetestaccount.md#onlytest) \| [*ExcludeTest*](./enums/accountserviceincludetestaccount.md#excludetest) \| [*All*](./enums/accountserviceincludetestaccount.md#all) \| [*Unknown*](./enums/accountserviceincludetestaccount.md#unknown)

**`memberof`** AccountServiceSelector

___

### numberResults

• `Optional` **numberResults**: ``null`` \| *number*

<div lang=\"ja\">ページの最大件数です。このフィールドは、1以上を指定する必要があります。</div> 

**`memberof`** AccountServiceSelector

___

### startIndex

• `Optional` **startIndex**: ``null`` \| *number*

<div lang=\"ja\">ページの先頭のインデックスです。このフィールドは、1以上を指定する必要があります。</div> 

**`memberof`** AccountServiceSelector
