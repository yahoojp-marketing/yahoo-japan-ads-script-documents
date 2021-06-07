# CampaignCriterionServiceKeyword


<div lang=\"ja\">CampaignCriterionServiceKeywordオブジェクトは、キーワードに関する情報を表します。<br> ADD時、このフィールドは省略可能です。※criterionTypeがKEYWORDの場合、必須です。</div> 

## Table of contents

### Properties

- [keywordMatchType](campaigncriterionservicekeyword.md#keywordmatchtype)
- [text](campaigncriterionservicekeyword.md#text)

## Properties

### keywordMatchType

• `Optional` **keywordMatchType**: ``null`` \| [*Exact*](./enums/campaigncriterionservicekeywordmatchtype.md#exact) \| [*Phrase*](./enums/campaigncriterionservicekeywordmatchtype.md#phrase) \| [*Broad*](./enums/campaigncriterionservicekeywordmatchtype.md#broad) \| [*Unknown*](./enums/campaigncriterionservicekeywordmatchtype.md#unknown)

**`memberof`** CampaignCriterionServiceKeyword

___

### text

• `Optional` **text**: ``null`` \| *string*

<div lang=\"ja\">キーワードの内容です。<br> ADD時、このフィールドは必須です。<br> ※最大80文字、10ワードです。</div> 

**`memberof`** CampaignCriterionServiceKeyword
