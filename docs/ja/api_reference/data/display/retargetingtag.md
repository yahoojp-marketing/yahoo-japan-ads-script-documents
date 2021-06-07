# RetargetingTag


<div lang=\"ja\">RetargetingTagオブジェクトは、サイトリターゲティングのタグ情報を表します。</div> 

## Table of contents

### Properties

- [accountId](retargetingtag.md#accountid)
- [advancedTag](retargetingtag.md#advancedtag)
- [approvalStatus](retargetingtag.md#approvalstatus)
- [retargetingTagId](retargetingtag.md#retargetingtagid)
- [tag](retargetingtag.md#tag)

## Properties

### accountId

• `Optional` **accountId**: ``null`` \| *number*

<div lang=\"ja\">アカウントIDです。</div> 

**`memberof`** RetargetingTag

___

### advancedTag

• `Optional` **advancedTag**: ``null`` \| *string*

<div lang=\"ja\"> リニューアル版のサイトリターゲティングタグは、従来のタグよりもブラウザーなどの環境の影響を受けづらい新しいフォーマットです。<br> 詳細は、「<a href=\"https://ads-help.yahoo.co.jp/yahooads/ydn/articledetail?lan=ja&aid=1397\">サイトリターゲティングタグの取得とサイトへの設置</a>」を参照してください。<br> このフィールドは、レスポンスの際に返却されますが、リクエストの際には無視されます。 </div> 

**`memberof`** RetargetingTag

___

### approvalStatus

• `Optional` **approvalStatus**: ``null`` \| [*Available*](./enums/retargetingtagserviceapprovalstatus.md#available) \| [*Disapproved*](./enums/retargetingtagserviceapprovalstatus.md#disapproved) \| [*DisapprovedWithReview*](./enums/retargetingtagserviceapprovalstatus.md#disapprovedwithreview) \| [*Unknown*](./enums/retargetingtagserviceapprovalstatus.md#unknown)

**`memberof`** RetargetingTag

___

### retargetingTagId

• `Optional` **retargetingTagId**: ``null`` \| *string*

<div lang=\"ja\">サイトリターゲティングのタグIDです。</div> 

**`memberof`** RetargetingTag

___

### tag

• `Optional` **tag**: ``null`` \| *string*

<div lang=\"ja\">サイトリターゲティングタグです。</div> 

**`memberof`** RetargetingTag
