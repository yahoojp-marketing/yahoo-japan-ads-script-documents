# RetargetingListServiceTargetList


<div lang=\"ja\"> RetargetingListServiceTargetListオブジェクトは、リターゲティングのターゲット種類とターゲットリストの情報を表します。<br> このフィールドは、ADDおよびSET時に必須となり、REMOVE時に無視されます。 </div> 

## Table of contents

### Properties

- [combinationTargetList](retargetinglistservicetargetlist.md#combinationtargetlist)
- [customAudienceTargetList](retargetinglistservicetargetlist.md#customaudiencetargetlist)
- [ruleTargetList](retargetinglistservicetargetlist.md#ruletargetlist)
- [similarityTargetList](retargetinglistservicetargetlist.md#similaritytargetlist)
- [targetListType](retargetinglistservicetargetlist.md#targetlisttype)

## Properties

### combinationTargetList

• `Optional` **combinationTargetList**: ``null`` \| [*RetargetingListServiceCombinationTargetList*](retargetinglistservicecombinationtargetlist.md)

**`memberof`** RetargetingListServiceTargetList

___

### customAudienceTargetList

• `Optional` **customAudienceTargetList**: ``null`` \| [*RetargetingListServiceCustomAudienceTargetList*](retargetinglistservicecustomaudiencetargetlist.md)

**`memberof`** RetargetingListServiceTargetList

___

### ruleTargetList

• `Optional` **ruleTargetList**: ``null`` \| [*RetargetingListServiceRuleTargetList*](retargetinglistserviceruletargetlist.md)

**`memberof`** RetargetingListServiceTargetList

___

### similarityTargetList

• `Optional` **similarityTargetList**: ``null`` \| [*RetargetingListServiceSimilarityTargetList*](retargetinglistservicesimilaritytargetlist.md)

**`memberof`** RetargetingListServiceTargetList

___

### targetListType

• **targetListType**: ``null`` \| [*DefaultList*](./enums/retargetinglistservicetargetlisttype.md#defaultlist) \| [*Rule*](./enums/retargetinglistservicetargetlisttype.md#rule) \| [*Combination*](./enums/retargetinglistservicetargetlisttype.md#combination) \| [*Similarity*](./enums/retargetinglistservicetargetlisttype.md#similarity) \| [*CustomAudience*](./enums/retargetinglistservicetargetlisttype.md#customaudience) \| [*Unknown*](./enums/retargetinglistservicetargetlisttype.md#unknown)

**`memberof`** RetargetingListServiceTargetList
