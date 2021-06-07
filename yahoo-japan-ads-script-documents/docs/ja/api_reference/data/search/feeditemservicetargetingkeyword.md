# FeedItemServiceTargetingKeyword


<div lang=\"ja\">FeedItemServiceTargetingKeywordオブジェクトは、データ自動挿入のターゲットキーワードを表します。<br> このフィールドは、レスポンスの際に返却されますが、リクエストの際には無視されます。<br> ※アドカスタマイザーの場合は、ADDおよびSET時に省略可能となります。</div> 

## Table of contents

### Properties

- [keywordMatchType](feeditemservicetargetingkeyword.md#keywordmatchtype)
- [targetingKeywordId](feeditemservicetargetingkeyword.md#targetingkeywordid)
- [text](feeditemservicetargetingkeyword.md#text)

## Properties

### keywordMatchType

• `Optional` **keywordMatchType**: ``null`` \| [*Exact*](./enums/feeditemservicekeywordmatchtype.md#exact) \| [*Phrase*](./enums/feeditemservicekeywordmatchtype.md#phrase) \| [*Broad*](./enums/feeditemservicekeywordmatchtype.md#broad) \| [*Unknown*](./enums/feeditemservicekeywordmatchtype.md#unknown)

**`memberof`** FeedItemServiceTargetingKeyword

___

### targetingKeywordId

• `Optional` **targetingKeywordId**: ``null`` \| *number*

<div lang=\"ja\">指定したキーワード（text）を識別する IDになります。<br> ※設定を解除する場合は「0」を指定 してください。<br> このフィールドは、SET時に省略可能となります。</div> 

**`memberof`** FeedItemServiceTargetingKeyword

___

### text

• `Optional` **text**: ``null`` \| *string*

<div lang=\"ja\">指定するキーワードです。<br>※入力制限：80文字、10ワード までです。<br> このフィールドはADDおよびSET時に必須となります。</div> 

**`memberof`** FeedItemServiceTargetingKeyword
