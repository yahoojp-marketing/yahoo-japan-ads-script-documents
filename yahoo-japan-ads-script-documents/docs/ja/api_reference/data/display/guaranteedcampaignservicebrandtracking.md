# GuaranteedCampaignServiceBrandTracking


<div lang=\"ja\"> GuaranteedCampaignServiceBrandTrackingは、ブランド効果測定レポートの設定情報を保持します。<br> このフィールドは、レスポンスの際に返却されますが、リクエストの際には無視されます。 </div> 

## Table of contents

### Properties

- [audienceCategoryIds1](guaranteedcampaignservicebrandtracking.md#audiencecategoryids1)
- [audienceCategoryIds2](guaranteedcampaignservicebrandtracking.md#audiencecategoryids2)
- [businessCategoryIds](guaranteedcampaignservicebrandtracking.md#businesscategoryids)

## Properties

### audienceCategoryIds1

• `Optional` **audienceCategoryIds1**: ``null`` \| *string*[]

<div lang=\"ja\"> オーディエンスカテゴリIDグループ1です。<br> レポート作成時、ここで指定されたカテゴリーに対して強い興味関心を持つ層を対象に集計します。<br> このフィールドは、レスポンスの際に返却されますが、リクエストの際には無視されます。 </div> 

**`memberof`** GuaranteedCampaignServiceBrandTracking

___

### audienceCategoryIds2

• `Optional` **audienceCategoryIds2**: ``null`` \| *string*[]

<div lang=\"ja\"> オーディエンスカテゴリIDグループ2です。<br> レポート作成時、ここで指定されたカテゴリーに対して少し興味関心を持つ層を対象に集計します。<br> このフィールドは、レスポンスの際に返却されますが、リクエストの際には無視されます。 </div> 

**`memberof`** GuaranteedCampaignServiceBrandTracking

___

### businessCategoryIds

• `Optional` **businessCategoryIds**: ``null`` \| *string*[]

<div lang=\"ja\"> ビジネスカテゴリIDグループです。<br> アンケート対象になる広告・商材の業種の種別を表します。<br> ※返却される値は、DictionaryServiceのgetBusinessCategoryで取得されるDictionaryServiceBusinessCategoryのbusinessCategoryIdフィールドをご確認ください。<br> このフィールドは、レスポンスの際に返却されますが、リクエストの際には無視されます。 </div> 

**`memberof`** GuaranteedCampaignServiceBrandTracking
