# DictionaryServiceAudienceCategory


<div lang=\"ja\">DictionaryServiceAudienceCategoryオブジェクトは、オーディエンスカテゴリー情報を格納するコンテナです。</div> 

## Table of contents

### Properties

- [audienceCategoryType](dictionaryserviceaudiencecategory.md#audiencecategorytype)
- [child](dictionaryserviceaudiencecategory.md#child)
- [code](dictionaryserviceaudiencecategory.md#code)
- [fullName](dictionaryserviceaudiencecategory.md#fullname)
- [isGuaranteedPermitted](dictionaryserviceaudiencecategory.md#isguaranteedpermitted)
- [name](dictionaryserviceaudiencecategory.md#name)
- [reach](dictionaryserviceaudiencecategory.md#reach)

## Properties

### audienceCategoryType

• `Optional` **audienceCategoryType**: ``null`` \| *string*

<div lang=\"ja\">提供されるカテゴリの種別を表します。</div>  <dl class=term>   <dt class=\"term__item\">AFFINITY</dt>   <dd class=\"term__desc\"><span lang=\"ja\">興味関心です。</span></dd>   <dt class=\"term__item\">IN_MARKET</dt>   <dd class=\"term__desc\"><span lang=\"ja\">購買意向です。</span></dd>   <dt class=\"term__item\">ATTRIBUTE_LIFE_EVENTS</dt>   <dd class=\"term__desc\"><span lang=\"ja\">属性ライフイベントです。</span></dd>   <dt class=\"term__item\">UNKNOWN</dt>   <dd class=\"term__desc\"><span lang=\"ja\">未知の値です。</span></dd> </dl>

**`memberof`** DictionaryServiceAudienceCategory

___

### child

• `Optional` **child**: ``null`` \| [*DictionaryServiceAudienceCategory*](dictionaryserviceaudiencecategory.md)[]

<div lang=\"ja\">子要素としてDictionaryServiceAudienceCategoryオブジェクトを使用します。</div> 

**`memberof`** DictionaryServiceAudienceCategory

___

### code

• `Optional` **code**: ``null`` \| *string*

<div lang=\"ja\">カテゴリコードです。</div> 

**`memberof`** DictionaryServiceAudienceCategory

___

### fullName

• `Optional` **fullName**: ``null`` \| *string*

<div lang=\"ja\">カテゴリ名称です。（カテゴリ名称、サブカテゴリ名称を含めた正式名称です。）</div> 

**`memberof`** DictionaryServiceAudienceCategory

___

### isGuaranteedPermitted

• `Optional` **isGuaranteedPermitted**: ``null`` \| *string*

<div lang=\"ja\">予約型販売対象を表します</div> 

**`memberof`** DictionaryServiceAudienceCategory

___

### name

• `Optional` **name**: ``null`` \| *string*

<div lang=\"ja\">サブカテゴリ名称です。</div> 

**`memberof`** DictionaryServiceAudienceCategory

___

### reach

• `Optional` **reach**: ``null`` \| *number*

<div lang=\"ja\">リーチ数です。</div> 

**`memberof`** DictionaryServiceAudienceCategory
