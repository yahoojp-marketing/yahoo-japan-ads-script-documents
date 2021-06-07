# FeedItemServiceSimpleFeedItemAttribute


<div lang=\"ja\">このフィールドは、ADDおよびSET時に省略可能となり、REMOVE時に無視されます。<br> ※placeholderFieldがSTRUCTURED_SNIPPET_VALUES, ADDITIONAL_ADVANCED_URLS, ADDITIONAL_ADVANCED_MOBILE_URLSの場合、ADDおよびSET時に必須となります。</div> 

## Table of contents

### Properties

- [feedAttributeValue](feeditemservicesimplefeeditemattribute.md#feedattributevalue)
- [reviewFeedAttributeValue](feeditemservicesimplefeeditemattribute.md#reviewfeedattributevalue)

## Properties

### feedAttributeValue

• `Optional` **feedAttributeValue**: ``null`` \| *string*

<div lang=\"ja\">フィードアイテム情報の値です。<br><br> ※データ自動挿入の利用時は、属性は以下のように入力してください：<br> ・AD_CUSTOMIZER_INTEGER<br> ex) 99999999<br>・AD_CUSTOMIZER_PRICE<br> ex) 19800 or 19,800<br> ・AD_CUSTOMIZER_DATE<br> ex) 20151231 235959<br> ・AD_CUSTOMIZER_STRING<br> ex) hoge ・STRUCTURED_SNIPPET_HEADER<br> ex) ブランド</div> 

**`memberof`** FeedItemServiceSimpleFeedItemAttribute

___

### reviewFeedAttributeValue

• `Optional` **reviewFeedAttributeValue**: ``null`` \| *string*

<div lang=\"ja\">審査中のフィードアイテム情報です。<br> ※審査中の間のみ、レスポンス時に表示されます。</div> 

**`memberof`** FeedItemServiceSimpleFeedItemAttribute
