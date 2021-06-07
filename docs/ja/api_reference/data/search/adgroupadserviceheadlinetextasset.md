# AdGroupAdServiceHeadlineTextAsset


<div lang=\"ja\">AdGroupAdServiceHeadlineTextAssetは、レスポンシブ広告で指定するタイトルのテキストアセットを表します。<br> headlines[]には、3~15件の指定が可能です。<br> ADD時、このフィールドは必須となります。</div> 

## Table of contents

### Properties

- [approvalStatus](adgroupadserviceheadlinetextasset.md#approvalstatus)
- [disapprovalReasonCodes](adgroupadserviceheadlinetextasset.md#disapprovalreasoncodes)
- [pinnedField](adgroupadserviceheadlinetextasset.md#pinnedfield)
- [text](adgroupadserviceheadlinetextasset.md#text)

## Properties

### approvalStatus

• `Optional` **approvalStatus**: ``null`` \| [*Approved*](./enums/adgroupadservicetextassetapprovalstatus.md#approved) \| [*Review*](./enums/adgroupadservicetextassetapprovalstatus.md#review) \| [*PreDisapproved*](./enums/adgroupadservicetextassetapprovalstatus.md#predisapproved) \| [*Unknown*](./enums/adgroupadservicetextassetapprovalstatus.md#unknown)

**`memberof`** AdGroupAdServiceHeadlineTextAsset

___

### disapprovalReasonCodes

• `Optional` **disapprovalReasonCodes**: ``null`` \| *string*[]

<div lang=\"ja\">審査否認の理由コードです。<br> (コード詳細は、DictionaryServiceのgetDisapprovalReasonのレスポンスを参照)<br> このフィールドは、レスポンスの際に返却されますが、リクエストの際には無視されます。</div> 

**`memberof`** AdGroupAdServiceHeadlineTextAsset

___

### pinnedField

• `Optional` **pinnedField**: ``null`` \| [*Unspecified*](./enums/adgroupadserviceheadlinepinnedfield.md#unspecified) \| [*Headline1*](./enums/adgroupadserviceheadlinepinnedfield.md#headline1) \| [*Headline2*](./enums/adgroupadserviceheadlinepinnedfield.md#headline2) \| [*Headline3*](./enums/adgroupadserviceheadlinepinnedfield.md#headline3) \| [*Unknown*](./enums/adgroupadserviceheadlinepinnedfield.md#unknown)

**`memberof`** AdGroupAdServiceHeadlineTextAsset

___

### text

• `Optional` **text**: ``null`` \| *string*

<div lang=\"ja\">テキストです。<br>このフィールドは、ADD時は必須となり、SET時は無視されます。</div> 

**`memberof`** AdGroupAdServiceHeadlineTextAsset
