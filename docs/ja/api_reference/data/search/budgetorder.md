# BudgetOrder


<div lang=\"ja\">BudgetOrderオブジェクトは、アカウント予算情報を示します。<br> </div> 

## Table of contents

### Properties

- [accountId](budgetorder.md#accountid)
- [accountType](budgetorder.md#accounttype)
- [amount](budgetorder.md#amount)
- [limitChargeType](budgetorder.md#limitchargetype)

## Properties

### accountId

• `Optional` **accountId**: ``null`` \| *number*

<div lang=\"ja\"> アカウントIDです。<br> SET時、このフィールドは必須となります。 </div> 

**`memberof`** BudgetOrder

___

### accountType

• `Optional` **accountType**: ``null`` \| [*Prepay*](./enums/budgetorderserviceaccounttype.md#prepay) \| [*Invoice*](./enums/budgetorderserviceaccounttype.md#invoice) \| [*Unknown*](./enums/budgetorderserviceaccounttype.md#unknown)

**`memberof`** BudgetOrder

___

### amount

• `Optional` **amount**: ``null`` \| *number*

<div lang=\"ja\"> アカウントの広告予算金額です。<br> SET時、このフィールドは省略可能となります。 月額予算は、accountTypeが<code>INVOICE</code>の場合のみ変更可能です。 また、予算額は1000円単位で指定する必要があります。 </div> 

**`memberof`** BudgetOrder

___

### limitChargeType

• `Optional` **limitChargeType**: ``null`` \| [*Sum*](./enums/budgetorderservicelimitchargetype.md#sum) \| [*Monthly*](./enums/budgetorderservicelimitchargetype.md#monthly) \| [*Unknown*](./enums/budgetorderservicelimitchargetype.md#unknown)

**`memberof`** BudgetOrder
