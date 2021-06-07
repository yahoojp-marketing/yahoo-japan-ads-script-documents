# AdGroupAdServiceResponsiveSearchAd


<div lang=\"ja\">AdGroupAdServiceResponsiveSearchAdオブジェクトは、レスポンシブ広告を表します。<br> ADD時、このフィールドは省略可能となります。※adTypeがRESPONSIVE_SEARCH_ADの場合は必須です。</div> 

## Table of contents

### Properties

- [descriptions](adgroupadserviceresponsivesearchad.md#descriptions)
- [headlines](adgroupadserviceresponsivesearchad.md#headlines)
- [path1](adgroupadserviceresponsivesearchad.md#path1)
- [path2](adgroupadserviceresponsivesearchad.md#path2)

## Properties

### descriptions

• `Optional` **descriptions**: ``null`` \| [*AdGroupAdServiceDescriptionTextAsset*](adgroupadservicedescriptiontextasset.md)[]

**`memberof`** AdGroupAdServiceResponsiveSearchAd

___

### headlines

• `Optional` **headlines**: ``null`` \| [*AdGroupAdServiceHeadlineTextAsset*](adgroupadserviceheadlinetextasset.md)[]

**`memberof`** AdGroupAdServiceResponsiveSearchAd

___

### path1

• `Optional` **path1**: ``null`` \| *string*

<div lang=\"ja\">自動作成される表示URLを補足するパスです。<br> ADD時、このフィールドは省略可能となります。その際、デフォルト設定値はnullとなります。<br>※path2を指定する場合は、path1は必須です。</div> 

**`memberof`** AdGroupAdServiceResponsiveSearchAd

___

### path2

• `Optional` **path2**: ``null`` \| *string*

<div lang=\"ja\">自動作成される表示URLを補足するパスです。<br> ADD時、このフィールドは省略可能となります。その際、デフォルト設定値はnullとなります。<br>※path1を指定していない場合、path2は無視されます。</div> 

**`memberof`** AdGroupAdServiceResponsiveSearchAd
