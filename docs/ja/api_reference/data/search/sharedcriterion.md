# SharedCriterion


<div lang=\"ja\">SharedCriterionオブジェクトは、対象外キーワード情報を保持します。</div> 

## Table of contents

### Properties

- [accountId](sharedcriterion.md#accountid)
- [criterionId](sharedcriterion.md#criterionid)
- [keywordMatchType](sharedcriterion.md#keywordmatchtype)
- [sharedListId](sharedcriterion.md#sharedlistid)
- [text](sharedcriterion.md#text)
- [use](sharedcriterion.md#use)

## Properties

### accountId

• `Optional` **accountId**: ``null`` \| *number*

<div lang=\"ja\">アカウントIDです。</div> 

**`memberof`** SharedCriterion

___

### criterionId

• `Optional` **criterionId**: ``null`` \| *number*

<div lang=\"ja\">クライテリオンIDです。<br> REMOVE時、このフィールドは必須となります。</div> 

**`memberof`** SharedCriterion

___

### keywordMatchType

• `Optional` **keywordMatchType**: ``null`` \| [*Exact*](./enums/sharedcriterionservicekeywordmatchtype.md#exact) \| [*Phrase*](./enums/sharedcriterionservicekeywordmatchtype.md#phrase) \| [*Broad*](./enums/sharedcriterionservicekeywordmatchtype.md#broad) \| [*Unknown*](./enums/sharedcriterionservicekeywordmatchtype.md#unknown)

**`memberof`** SharedCriterion

___

### sharedListId

• `Optional` **sharedListId**: ``null`` \| *number*

<div lang=\"ja\">アカウント共有リストIDです。<br> ADDおよびREMOVE時、このフィールドは必須となります。</div> 

**`memberof`** SharedCriterion

___

### text

• `Optional` **text**: ``null`` \| *string*

<div lang=\"ja\">キーワードです。<br> ADD時、このフィールドは必須となります。</div> 

**`memberof`** SharedCriterion

___

### use

• `Optional` **use**: ``null`` \| [*Negative*](./enums/sharedcriterionserviceuse.md#negative) \| [*Unknown*](./enums/sharedcriterionserviceuse.md#unknown)

**`memberof`** SharedCriterion
