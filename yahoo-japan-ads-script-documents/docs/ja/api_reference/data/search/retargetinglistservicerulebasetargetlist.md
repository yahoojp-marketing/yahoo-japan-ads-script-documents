# RetargetingListServiceRuleBaseTargetList


<div lang=\"ja\">RetargetingListServiceRuleBaseTargetListは、ベースターゲットリストの情報を保持するオブジェクトです。<br> このフィールドは、省略可能となります。<br> ※targetListTypeがRULEの場合、このフィールドは必須となります。</div> 

## Table of contents

### Properties

- [endDate](retargetinglistservicerulebasetargetlist.md#enddate)
- [isAllVisitorRule](retargetinglistservicerulebasetargetlist.md#isallvisitorrule)
- [isDateSpecificRule](retargetinglistservicerulebasetargetlist.md#isdatespecificrule)
- [rules](retargetinglistservicerulebasetargetlist.md#rules)
- [startDate](retargetinglistservicerulebasetargetlist.md#startdate)

## Properties

### endDate

• `Optional` **endDate**: ``null`` \| *string*

<div lang=\"ja\">ルール適用終了日です。<br> このフィールドは、ADDおよびSET時に省略可能となります。<br> isDateSpecificがTRUEである場合、ADDおよびSET時に必須となります。<br> ※YYYYMMDD形式です。<br> ※リクエスト日は2037/12/30まで 指定可能です。</div> 

**`memberof`** RetargetingListServiceRuleBaseTargetList

___

### isAllVisitorRule

• `Optional` **isAllVisitorRule**: ``null`` \| [*True*](./enums/retargetinglistserviceisallvisitorrule.md#true) \| [*False*](./enums/retargetinglistserviceisallvisitorrule.md#false) \| [*Unknown*](./enums/retargetinglistserviceisallvisitorrule.md#unknown)

**`memberof`** RetargetingListServiceRuleBaseTargetList

___

### isDateSpecificRule

• `Optional` **isDateSpecificRule**: ``null`` \| [*True*](./enums/retargetinglistserviceisdatespecificrule.md#true) \| [*False*](./enums/retargetinglistserviceisdatespecificrule.md#false) \| [*Unknown*](./enums/retargetinglistserviceisdatespecificrule.md#unknown)

**`memberof`** RetargetingListServiceRuleBaseTargetList

___

### rules

• `Optional` **rules**: ``null`` \| [*RetargetingListServiceRuleGroup*](retargetinglistservicerulegroup.md)[]

**`memberof`** RetargetingListServiceRuleBaseTargetList

___

### startDate

• `Optional` **startDate**: ``null`` \| *string*

<div lang=\"ja\">ルール適用開始日です。<br> ADDおよびSET時、このフィールドは省略可能となります。<br> isDateSpecificがTRUEである場合、ADDおよびSET時に必須となります。 <br> ※YYYYMMDD形式です。<br>※リクエスト日は2037/12/30まで 指定可能です。</div> 

**`memberof`** RetargetingListServiceRuleBaseTargetList
