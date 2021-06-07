# Enumeration: FeedSetServiceConditionType


<div lang=\"ja\"> 商品セットの条件に設定できる項目の種別です。<br> ADD時、このフィールドは必須です。 </div>  <dl class=term>   <dt class=\"term__item\">CATEGORY_ID</dt>   <dd class=\"term__desc\"><span lang=\"ja\">カテゴリーID</span></dd>   <dt class=\"term__item\">STOCK_QUANTITY</dt>   <dd class=\"term__desc\"><span lang=\"ja\">在庫数</span></dd>   <dt class=\"term__item\">PRICE</dt>   <dd class=\"term__desc\"><span lang=\"ja\">価格</span></dd>   <dt class=\"term__item\">SALE_PRICE</dt>   <dd class=\"term__desc\"><span lang=\"ja\">セール価格</span></dd>   <dt class=\"term__item\">RATING</dt>   <dd class=\"term__desc\"><span lang=\"ja\">評価</span></dd>   <dt class=\"term__item\">REVIEWS</dt>   <dd class=\"term__desc\"><span lang=\"ja\">評価件数</span></dd>   <dt class=\"term__item\">BADGE</dt>   <dd class=\"term__desc\"><span lang=\"ja\">バッジ種別<br>FeedSetServiceConditionで設定可能な値:<br><a href=\"https://support-marketing.yahoo.co.jp/promotionalads/ydn/articledetail?lan=ja&amp;aid=36277\" rel=\"nofollow\">データフィードのファイルフォーマット</a>の「商品リストファイルの入力項目」にある「Badge」で利用できる値のみ指定できます。<br></span><span lang=\"en\">Type of badge<br>Available values on FeedSetServiceCondition:<br>The values which is available for &#34;Badge&#34; in the &#34;Data feed (item list)&#34; part of the guideline page &#34;<a href=\"https://support-marketing.yahoo.co.jp/promotionalads/ydn/articledetail?lan=en&amp;aid=22325\" rel=\"nofollow\">Dynamic Ads for Display</a>&#34; can be specified.<br></span></dd>   <dt class=\"term__item\">AGE_GROUP</dt>   <dd class=\"term__desc\"><span lang=\"ja\">年齢層<br>FeedSetServiceConditionで設定可能な値:<br><a href=\"https://support-marketing.yahoo.co.jp/promotionalads/ydn/articledetail?lan=ja&amp;aid=36277\" rel=\"nofollow\">データフィードのファイルフォーマット</a>の「商品リストファイルの入力項目」にある「AgeGroup」で利用できる値のみ指定できます。<br></span><span lang=\"en\">Age group<br>Available values on FeedSetServiceCondition:<br>The values which is available for &#34;AgeGroup&#34; in the &#34;Data feed (item list)&#34; part of the guideline page &#34;<a href=\"https://support-marketing.yahoo.co.jp/promotionalads/ydn/articledetail?lan=en&amp;aid=22325\" rel=\"nofollow\">Dynamic Ads for Display</a>&#34; can be specified.<br></span></dd>   <dt class=\"term__item\">AVAILABILITY_DATE</dt>   <dd class=\"term__desc\"><span lang=\"ja\">入荷予定日</span></dd>   <dt class=\"term__item\">GENDER_GROUP</dt>   <dd class=\"term__desc\"><span lang=\"ja\">性別<br>FeedSetServiceConditionで設定可能な値:<br><a href=\"https://support-marketing.yahoo.co.jp/promotionalads/ydn/articledetail?lan=ja&amp;aid=36277\" rel=\"nofollow\">データフィードのファイルフォーマット</a>の「商品リストファイルの入力項目」にある「GenderGroup」で利用できる値のみ指定できます。<br></span><span lang=\"en\">Gender group<br>Available values on FeedSetServiceCondition:<br>The values which is available for &#34;GenderGroup&#34; in the &#34;Data feed (item list)&#34; part of the guideline page &#34;<a href=\"https://support-marketing.yahoo.co.jp/promotionalads/ydn/articledetail?lan=en&amp;aid=22325\" rel=\"nofollow\">Dynamic Ads for Display</a>&#34; can be specified.<br></span></dd>   <dt class=\"term__item\">GOOGLE_PRODUCT_CATEGORY</dt>   <dd class=\"term__desc\"><span lang=\"ja\">Google商品カテゴリ<br>FeedSetServiceConditionで設定可能な値:<br>Google商品カテゴリで取得できるGoogle商品カテゴリのidのみ指定できます。<br></span><span lang=\"en\">Google product category<br>Available values on FeedSetServiceCondition:<br>Only Google product category ID that can be acquired in Google product category can be specified.<br></span></dd>   <dt class=\"term__item\">LOCATION</dt>   <dd class=\"term__desc\"><span lang=\"ja\">地域<br>DictionaryServiceGeographicLocationType.FEEDを指定して取得できる地域情報のcodeのみ指定できます。<br></span><span lang=\"en\">Location<br>Only the Location information code acquired by declaring DictionaryServiceGeographicLocationType.FEED can be specified.<br></span></dd>   <dt class=\"term__item\">SALES_RANK</dt>   <dd class=\"term__desc\"><span lang=\"ja\">売上順位</span></dd>   <dt class=\"term__item\">UNKNOWN</dt>   <dd class=\"term__desc\"><span lang=\"ja\">未知の値です。</span></dd> </dl>

## Table of contents

### Enumeration members

- [AgeGroup](feedsetserviceconditiontype.md#agegroup)
- [AvailabilityDate](feedsetserviceconditiontype.md#availabilitydate)
- [Badge](feedsetserviceconditiontype.md#badge)
- [CategoryId](feedsetserviceconditiontype.md#categoryid)
- [GenderGroup](feedsetserviceconditiontype.md#gendergroup)
- [GoogleProductCategory](feedsetserviceconditiontype.md#googleproductcategory)
- [Location](feedsetserviceconditiontype.md#location)
- [Price](feedsetserviceconditiontype.md#price)
- [Rating](feedsetserviceconditiontype.md#rating)
- [Reviews](feedsetserviceconditiontype.md#reviews)
- [SalePrice](feedsetserviceconditiontype.md#saleprice)
- [SalesRank](feedsetserviceconditiontype.md#salesrank)
- [StockQuantity](feedsetserviceconditiontype.md#stockquantity)
- [Unknown](feedsetserviceconditiontype.md#unknown)

## Enumeration members

### AgeGroup

• **AgeGroup**: = "AGE\_GROUP"

___

### AvailabilityDate

• **AvailabilityDate**: = "AVAILABILITY\_DATE"

___

### Badge

• **Badge**: = "BADGE"

___

### CategoryId

• **CategoryId**: = "CATEGORY\_ID"

___

### GenderGroup

• **GenderGroup**: = "GENDER\_GROUP"

___

### GoogleProductCategory

• **GoogleProductCategory**: = "GOOGLE\_PRODUCT\_CATEGORY"

___

### Location

• **Location**: = "LOCATION"

___

### Price

• **Price**: = "PRICE"

___

### Rating

• **Rating**: = "RATING"

___

### Reviews

• **Reviews**: = "REVIEWS"

___

### SalePrice

• **SalePrice**: = "SALE\_PRICE"

___

### SalesRank

• **SalesRank**: = "SALES\_RANK"

___

### StockQuantity

• **StockQuantity**: = "STOCK\_QUANTITY"

___

### Unknown

• **Unknown**: = "UNKNOWN"
