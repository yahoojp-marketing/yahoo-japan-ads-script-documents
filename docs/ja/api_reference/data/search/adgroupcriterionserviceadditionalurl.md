# AdGroupCriterionServiceAdditionalUrl


<div lang=\"ja\">AdGroupCriterionServiceAdditionalUrlオブジェクトは、追加する最終リンク先URLを保持します。<br> このフィールドは、ADD時は必須となり、SET時は省略可能となります。</div> 

## Table of contents

### Properties

- [disapprovalReasonCodes](adgroupcriterionserviceadditionalurl.md#disapprovalreasoncodes)
- [reviewUrl](adgroupcriterionserviceadditionalurl.md#reviewurl)
- [url](adgroupcriterionserviceadditionalurl.md#url)

## Properties

### disapprovalReasonCodes

• `Optional` **disapprovalReasonCodes**: ``null`` \| *string*[]

<div lang=\"ja\">審査否認理由のコードです。<br> (コード詳細は、DictionaryServiceのgetDisapprovalReasonのレスポンスを参照)<br> このフィールドは、レスポンスの際に返却されますが、リクエストの際には無視されます。</div> 

**`memberof`** AdGroupCriterionServiceAdditionalUrl

___

### reviewUrl

• `Optional` **reviewUrl**: ``null`` \| *string*

<div lang=\"ja\">審査中の最終リンク先URLです。<br> このフィールドは、レスポンスの際に返却されますが、リクエストの際には無視されます。</div> 

**`memberof`** AdGroupCriterionServiceAdditionalUrl

___

### url

• `Optional` **url**: ``null`` \| *string*

<div lang=\"ja\">最終リンク先URLです。<br> ADDおよびSET時、このフィールドは必須となります。</div> 

**`memberof`** AdGroupCriterionServiceAdditionalUrl
