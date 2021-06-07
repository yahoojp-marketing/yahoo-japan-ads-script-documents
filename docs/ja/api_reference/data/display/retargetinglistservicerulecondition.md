# RetargetingListServiceRuleCondition


<div lang=\"ja\"> RetargetingListServiceRuleConditionオブジェクトは、ターゲットリストに設定可能な条件を表します。<br> このフィールドは、ADDおよびSET時に必須となります。 </div> 

## Table of contents

### Properties

- [compareOperator](retargetinglistservicerulecondition.md#compareoperator)
- [ruleType](retargetinglistservicerulecondition.md#ruletype)
- [value](retargetinglistservicerulecondition.md#value)

## Properties

### compareOperator

• `Optional` **compareOperator**: ``null`` \| [*Equal*](./enums/retargetinglistservicecompareoperator.md#equal) \| [*Included*](./enums/retargetinglistservicecompareoperator.md#included) \| [*StartWith*](./enums/retargetinglistservicecompareoperator.md#startwith) \| [*EndWith*](./enums/retargetinglistservicecompareoperator.md#endwith) \| [*NotEqual*](./enums/retargetinglistservicecompareoperator.md#notequal) \| [*NotIncluded*](./enums/retargetinglistservicecompareoperator.md#notincluded) \| [*NotStartWith*](./enums/retargetinglistservicecompareoperator.md#notstartwith) \| [*NotEndWith*](./enums/retargetinglistservicecompareoperator.md#notendwith) \| [*Unknown*](./enums/retargetinglistservicecompareoperator.md#unknown)

**`memberof`** RetargetingListServiceRuleCondition

___

### ruleType

• `Optional` **ruleType**: ``null`` \| [*Url*](./enums/retargetinglistserviceruletype.md#url) \| [*Label*](./enums/retargetinglistserviceruletype.md#label) \| [*RefererUrl*](./enums/retargetinglistserviceruletype.md#refererurl) \| [*PageType*](./enums/retargetinglistserviceruletype.md#pagetype) \| [*ItemId*](./enums/retargetinglistserviceruletype.md#itemid) \| [*ItemCategoryId*](./enums/retargetinglistserviceruletype.md#itemcategoryid) \| [*EventType*](./enums/retargetinglistserviceruletype.md#eventtype) \| [*Unknown*](./enums/retargetinglistserviceruletype.md#unknown)

**`memberof`** RetargetingListServiceRuleCondition

___

### value

• `Optional` **value**: ``null`` \| *string*

<div lang=\"ja\"> ルールで評価する値です。<br> このフィールドは、ADDおよびSET時に必須となり、REMOVE時に無視されます。<br> ※ruleTypeがEVENT_TYPEの場合、以下のイベント種別に記載の値のみ指定可能となります。 </div>          </td>       </tr>     </tbody>   </table> </details>

**`memberof`** RetargetingListServiceRuleCondition
