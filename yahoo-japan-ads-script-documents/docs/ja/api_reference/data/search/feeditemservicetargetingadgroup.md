# FeedItemServiceTargetingAdGroup


<div lang=\"ja\">FeedItemServiceTargetingAdGroupオブジェクトは、データ自動挿入の広告グループとの紐付けを表します。<br> このフィールドは、レスポンスの際に返却されますが、リクエストの際には無視されます。<br> ※アドカスタマイザーの場合、ADDおよびSET時に省略可能となります。</div> 

## Table of contents

### Properties

- [targetingAdGroupId](feeditemservicetargetingadgroup.md#targetingadgroupid)

## Properties

### targetingAdGroupId

• `Optional` **targetingAdGroupId**: ``null`` \| *number*

<div lang=\"ja\">配信に使用する広告グループIDです。<br> ※設定を解除する場合は「0」を指定してください。<br> ※addのリクエストで、「0」指定は未 指定と同じ扱いになります。<br> データ自動挿入の場合、このフィールドはADDおよびSET時に省略可能となります。 </div> 

**`memberof`** FeedItemServiceTargetingAdGroup
