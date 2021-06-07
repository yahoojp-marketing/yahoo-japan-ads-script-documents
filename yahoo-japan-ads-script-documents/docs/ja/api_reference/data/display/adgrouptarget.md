# AdGroupTarget


<div lang=\"ja\"> AdGroupTargetオブジェクトは、広告グループに設定されているターゲティング情報を格納します。<br> このオブジェクトは、GuaranteedAdGroupServiceで広告グループを追加する場合は必須です。<br> *GuaranteedAdGroupServiceでGETする際、このフィールドは返却されません。 </div> 

## Table of contents

### Properties

- [accountId](adgrouptarget.md#accountid)
- [adGroupId](adgrouptarget.md#adgroupid)
- [bidMultiplier](adgrouptarget.md#bidmultiplier)
- [campaignId](adgrouptarget.md#campaignid)
- [target](adgrouptarget.md#target)

## Properties

### accountId

• `Optional` **accountId**: ``null`` \| *number*

<div lang=\"ja\"> アカウントIDです。<br> このフィールドは、レスポンスの際に返却されますが、リクエストの際には無視されます。 </div> 

**`memberof`** AdGroupTarget

___

### adGroupId

• `Optional` **adGroupId**: ``null`` \| *number*

<div lang=\"ja\"> 広告グループIDです。<br> このフィールドは、リクエストの場合は必須です。 </div> 

**`memberof`** AdGroupTarget

___

### bidMultiplier

• `Optional` **bidMultiplier**: ``null`` \| *number*

<div lang=\"ja\"> 入札価格調整率です。<br> このフィールドは、ADD、SETおよびREPLACE時は省略可能となり、REMOVE時は無視されます。<br> ※入札価格調整率が設定できないターゲティングの場合は返却されません。<br> ※広告グループのターゲティングにSITE_RETARGETING、SEARCH_TARGET、PLACEMENT_TARGETのいずれかを指定し、かつその広告グループがYDNキャンペーンに紐づいている場合にbidMultiplierを指定しなかった時は、nullが代入されます。<br> ※その他の場合でbidMultiplierを指定しなかった時は1.0が代入されます。 </div> 

**`memberof`** AdGroupTarget

___

### campaignId

• `Optional` **campaignId**: ``null`` \| *number*

<div lang=\"ja\"> キャンペーンIDです。<br> このフィールドは、リクエストの場合は必須です。 </div> 

**`memberof`** AdGroupTarget

___

### target

• `Optional` **target**: ``null`` \| [*AdGroupTargetServiceTarget*](adgrouptargetservicetarget.md)

**`memberof`** AdGroupTarget
