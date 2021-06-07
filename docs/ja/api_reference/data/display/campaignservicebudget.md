# CampaignServiceBudget


<div lang=\"ja\"> CampaignServiceBudgetオブジェクトは、キャンペーン予算に関する情報を表します。<br> このフィールドは、ADD時は必須、SET時は省略可能となり、REMOVE時は無視されます。 </div> 

## Table of contents

### Properties

- [amount](campaignservicebudget.md#amount)
- [budgetDeliveryMethod](campaignservicebudget.md#budgetdeliverymethod)

## Properties

### amount

• `Optional` **amount**: ``null`` \| *number*

<div lang=\"ja\"> キャンペーンの一日あたりの予算（一日単位の利用金額）です。<br> このフィールドは、ADDおよびSET時に省略可能となり、REMOVE時は無視されます。<br> budgetDeliveryMethodがSTANDARDの場合はADDおよびSET時に必須です。<br> ※目的ありの場合、ADD時に必須となります。 </div> 

**`memberof`** CampaignServiceBudget

___

### budgetDeliveryMethod

• `Optional` **budgetDeliveryMethod**: ``null`` \| [*Standard*](./enums/campaignservicebudgetdeliverymethod.md#standard) \| [*Accelerated*](./enums/campaignservicebudgetdeliverymethod.md#accelerated) \| [*Unknown*](./enums/campaignservicebudgetdeliverymethod.md#unknown)

**`memberof`** CampaignServiceBudget
