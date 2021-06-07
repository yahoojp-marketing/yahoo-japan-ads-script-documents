# FeedItemServiceTargetingCampaign


<div lang=\"ja\">FeedItemServiceTargetingCampaignオブジェクトは、データ自動挿入のキャンペーンとの紐付けを表します。<br> このフィールドは、レスポンスの際に返却されますが、リクエストの際には無視されます。<br> ※アドカスタマイザーの場合は、ADDおよびSET時に省略可能となります。</div> 

## Table of contents

### Properties

- [targetingCampaignId](feeditemservicetargetingcampaign.md#targetingcampaignid)

## Properties

### targetingCampaignId

• `Optional` **targetingCampaignId**: ``null`` \| *number*

<div lang=\"ja\">配信に使用するキャンペーンIDです。<br> ※設定を解除する場合は「0」を指定してください。<br> ※addのリクエストで、「0」指定は未指定と同じ扱いになります。<br> データ自動挿入の場合、このフィールドはADDおよびSET時に必須となります。</div> 

**`memberof`** FeedItemServiceTargetingCampaign
