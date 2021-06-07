# AdGroupAdServiceDescriptionTextAsset


<div lang=\"ja\">AdGroupAdServiceDescriptionTextAssetは、レスポンシブ広告で指定する説明文のテキストアセットを表します。<br> descriptions[]には、2~4件の指定が可能です。<br> ADD時、このフィールドは必須となります。</div> 

## Table of contents

### Properties

- [approvalStatus](adgroupadservicedescriptiontextasset.md#approvalstatus)
- [disapprovalReasonCodes](adgroupadservicedescriptiontextasset.md#disapprovalreasoncodes)
- [pinnedField](adgroupadservicedescriptiontextasset.md#pinnedfield)
- [text](adgroupadservicedescriptiontextasset.md#text)

## Properties

### approvalStatus

• `Optional` **approvalStatus**: ``null`` \| [*Approved*](./enums/adgroupadservicetextassetapprovalstatus.md#approved) \| [*Review*](./enums/adgroupadservicetextassetapprovalstatus.md#review) \| [*PreDisapproved*](./enums/adgroupadservicetextassetapprovalstatus.md#predisapproved) \| [*Unknown*](./enums/adgroupadservicetextassetapprovalstatus.md#unknown)

**`memberof`** AdGroupAdServiceDescriptionTextAsset

___

### disapprovalReasonCodes

• `Optional` **disapprovalReasonCodes**: ``null`` \| *string*[]

<div lang=\"ja\">審査否認の理由コードです。<br> (コード詳細は、DictionaryServiceのgetDisapprovalReasonのレスポンスを参照)<br> このフィールドは、レスポンスの際に返却されますが、リクエストの際には無視されます。</div> 

**`memberof`** AdGroupAdServiceDescriptionTextAsset

___

### pinnedField

• `Optional` **pinnedField**: ``null`` \| [*Unspecified*](./enums/adgroupadservicedescriptionpinnedfield.md#unspecified) \| [*Description1*](./enums/adgroupadservicedescriptionpinnedfield.md#description1) \| [*Description2*](./enums/adgroupadservicedescriptionpinnedfield.md#description2) \| [*Unknown*](./enums/adgroupadservicedescriptionpinnedfield.md#unknown)

**`memberof`** AdGroupAdServiceDescriptionTextAsset

___

### text

• `Optional` **text**: ``null`` \| *string*

<div lang=\"ja\">テキストです。<br>このフィールドは、ADD時は必須となり、SET時は無視されます。</div> 

**`memberof`** AdGroupAdServiceDescriptionTextAsset
