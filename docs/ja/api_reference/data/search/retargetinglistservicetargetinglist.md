# RetargetingListServiceTargetingList


<div lang=\"ja\">RetargetingListServiceTargetingListは、リターゲティング情報（ターゲットリスト）を保持するオブジェクトです。</div> 

## Table of contents

### Properties

- [accountId](retargetinglistservicetargetinglist.md#accountid)
- [closingReason](retargetinglistservicetargetinglist.md#closingreason)
- [defaultTargetList](retargetinglistservicetargetinglist.md#defaulttargetlist)
- [logicalTargetList](retargetinglistservicetargetinglist.md#logicaltargetlist)
- [reach](retargetinglistservicetargetinglist.md#reach)
- [reachStorageSpan](retargetinglistservicetargetinglist.md#reachstoragespan)
- [reachStorageStatus](retargetinglistservicetargetinglist.md#reachstoragestatus)
- [retargetingAccountStatus](retargetinglistservicetargetinglist.md#retargetingaccountstatus)
- [ruleBaseTargetList](retargetinglistservicetargetinglist.md#rulebasetargetlist)
- [targetListDescription](retargetinglistservicetargetinglist.md#targetlistdescription)
- [targetListId](retargetinglistservicetargetinglist.md#targetlistid)
- [targetListName](retargetinglistservicetargetinglist.md#targetlistname)
- [targetListOwner](retargetinglistservicetargetinglist.md#targetlistowner)
- [targetListTrackId](retargetinglistservicetargetinglist.md#targetlisttrackid)
- [targetListType](retargetinglistservicetargetinglist.md#targetlisttype)

## Properties

### accountId

• `Optional` **accountId**: ``null`` \| *number*

<div lang=\"ja\">アカウントIDです。<br> このフィールドは、いずれの場合でも必須となります。</div> 

**`memberof`** RetargetingListServiceTargetingList

___

### closingReason

• `Optional` **closingReason**: ``null`` \| [*UnusedList*](./enums/retargetinglistserviceclosingreason.md#unusedlist) \| [*Unknown*](./enums/retargetinglistserviceclosingreason.md#unknown)

**`memberof`** RetargetingListServiceTargetingList

___

### defaultTargetList

• `Optional` **defaultTargetList**: ``null`` \| [*RetargetingListServiceDefaultTargetList*](retargetinglistservicedefaulttargetlist.md)

**`memberof`** RetargetingListServiceTargetingList

___

### logicalTargetList

• `Optional` **logicalTargetList**: ``null`` \| [*RetargetingListServiceLogicalTargetList*](retargetinglistservicelogicaltargetlist.md)

**`memberof`** RetargetingListServiceTargetingList

___

### reach

• `Optional` **reach**: ``null`` \| *number*

<div lang=\"ja\">リストに蓄積されているユーザー数です。</div> 

**`memberof`** RetargetingListServiceTargetingList

___

### reachStorageSpan

• `Optional` **reachStorageSpan**: ``null`` \| *number*

<div lang=\"ja\">Cookieを保持する日数です。<br> SET時、このフィールドは省略可能となります。<br>LogicalTargetListの場合、SET時にこのフィールドは無視されます。<br> ※Default：180<br> ※1-540日まで設定可能です。</div> 

**`memberof`** RetargetingListServiceTargetingList

___

### reachStorageStatus

• `Optional` **reachStorageStatus**: ``null`` \| [*Open*](./enums/retargetinglistservicereachstoragestatus.md#open) \| [*Closed*](./enums/retargetinglistservicereachstoragestatus.md#closed) \| [*Unknown*](./enums/retargetinglistservicereachstoragestatus.md#unknown)

**`memberof`** RetargetingListServiceTargetingList

___

### retargetingAccountStatus

• `Optional` **retargetingAccountStatus**: ``null`` \| [*RetargetingListServiceRetargetingAccountStatus*](retargetinglistserviceretargetingaccountstatus.md)

**`memberof`** RetargetingListServiceTargetingList

___

### ruleBaseTargetList

• `Optional` **ruleBaseTargetList**: ``null`` \| [*RetargetingListServiceRuleBaseTargetList*](retargetinglistservicerulebasetargetlist.md)

**`memberof`** RetargetingListServiceTargetingList

___

### targetListDescription

• `Optional` **targetListDescription**: ``null`` \| *string*

<div lang=\"ja\">ターゲットリストの説明です。<br> このフィールドは、いずれの場合でも省略可能となります。</div> 

**`memberof`** RetargetingListServiceTargetingList

___

### targetListId

• `Optional` **targetListId**: ``null`` \| *number*

<div lang=\"ja\">ターゲットリストIDです。<br> SET時、このフィールドは必須となります。</div> 

**`memberof`** RetargetingListServiceTargetingList

___

### targetListName

• `Optional` **targetListName**: ``null`` \| *string*

<div lang=\"ja\">ターゲットリスト名です。<br> ADD時にこのフィールドは必須となり、SET時にこのフィールドは省略可能となります。</div> 

**`memberof`** RetargetingListServiceTargetingList

___

### targetListOwner

• `Optional` **targetListOwner**: ``null`` \| [*Owner*](./enums/retargetinglistservicetargetlistowner.md#owner) \| [*Shared*](./enums/retargetinglistservicetargetlistowner.md#shared) \| [*Unknown*](./enums/retargetinglistservicetargetlistowner.md#unknown)

**`memberof`** RetargetingListServiceTargetingList

___

### targetListTrackId

• `Optional` **targetListTrackId**: ``null`` \| *number*

<div lang=\"ja\">ターゲットリストのトラッキング用IDです。</div> 

**`memberof`** RetargetingListServiceTargetingList

___

### targetListType

• `Optional` **targetListType**: ``null`` \| [*Default*](./enums/retargetinglistservicetargetlisttype.md#default) \| [*Rule*](./enums/retargetinglistservicetargetlisttype.md#rule) \| [*Logical*](./enums/retargetinglistservicetargetlisttype.md#logical) \| [*Unknown*](./enums/retargetinglistservicetargetlisttype.md#unknown)

**`memberof`** RetargetingListServiceTargetingList
