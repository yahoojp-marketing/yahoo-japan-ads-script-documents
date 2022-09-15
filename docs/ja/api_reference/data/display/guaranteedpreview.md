# GuaranteedPreview


<div lang=\"ja\">GuaranteedPreviewオブジェクトは、予約型キャンペーンのプレビュー情報を保持します。</div> 

## Table of contents

### Properties

- [accountId](guaranteedpreview.md#accountid)
- [material](guaranteedpreview.md#material)
- [previewUrl](guaranteedpreview.md#previewurl)

## Properties

### accountId

• `Optional` **accountId**: ``null`` \| *number*

<div lang=\"ja\"> アカウントIDです。<br> このフィールドは、リクエストの場合は必須です。 </div> 

**`memberof`** GuaranteedPreview

___

### material

• `Optional` **material**: ``null`` \| [*GuaranteedPreviewServiceMaterial*](guaranteedpreviewservicematerial.md)

**`memberof`** GuaranteedPreview

___

### previewUrl

• `Optional` **previewUrl**: ``null`` \| *string*

<div lang=\"ja\"> プレビューURLです。<br> 有効なプレビューURLを取得する場合、指定されたアカウントID配下にある広告IDおよび各種メディアIDを指定してください。<br> このフィールドは、レスポンスの際に返却されますが、リクエストの際には無視されます。 </div> 

**`memberof`** GuaranteedPreview
