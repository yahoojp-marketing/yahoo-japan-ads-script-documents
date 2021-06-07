# FeedItemServiceCustomParameter


<div lang=\"ja\">FeedItemServiceCustomParameterは、カスタムパラメータの内容を表します。<br> このフィールドは、ADDおよびSET時に必須となります。<br> SET時、このフィールドは既存の項目を置き換えます。<br> ※削除フラグを立てた場合(isRemove=TRUE)、このフィールドは無視され、こちらの項目関係なく、全項目が削除されます。</div> 

## Table of contents

### Properties

- [key](feeditemservicecustomparameter.md#key)
- [value](feeditemservicecustomparameter.md#value)

## Properties

### key

• `Optional` **key**: ``null`` \| *string*

<div lang=\"ja\">キーです。<br> このフィールドは、ADDおよびSET時に必須となります。</div> 

**`memberof`** FeedItemServiceCustomParameter

___

### value

• `Optional` **value**: ``null`` \| *string*

<div lang=\"ja\">値です。<br> このフィールドは、ADDおよびSET時に省略可能となります。</div> 

**`memberof`** FeedItemServiceCustomParameter
