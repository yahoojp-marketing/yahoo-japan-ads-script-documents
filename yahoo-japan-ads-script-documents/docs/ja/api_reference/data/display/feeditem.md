# FeedItem


<div lang=\"ja\">FeedItemオブジェクトは、商品の情報を格納するコンテナです。</div> 

## Table of contents

### Properties

- [availability](feeditem.md#availability)
- [capacity](feeditem.md#capacity)
- [displaySettings](feeditem.md#displaysettings)
- [feedId](feeditem.md#feedid)
- [formattedPrice](feeditem.md#formattedprice)
- [formattedSalePrice](feeditem.md#formattedsaleprice)
- [inStock](feeditem.md#instock)
- [isRemoveCapacity](feeditem.md#isremovecapacity)
- [isRemoveFormattedPrice](feeditem.md#isremoveformattedprice)
- [isRemoveFormattedSalePrice](feeditem.md#isremoveformattedsaleprice)
- [isRemovePrice](feeditem.md#isremoveprice)
- [isRemoveSalePrice](feeditem.md#isremovesaleprice)
- [itemId](feeditem.md#itemid)
- [price](feeditem.md#price)
- [salePrice](feeditem.md#saleprice)

## Properties

### availability

• `Optional` **availability**: ``null`` \| [*OutOfStock*](./enums/feeditemserviceavailability.md#outofstock) \| [*InStock*](./enums/feeditemserviceavailability.md#instock) \| [*Preorder*](./enums/feeditemserviceavailability.md#preorder) \| [*Unknown*](./enums/feeditemserviceavailability.md#unknown)

**`memberof`** FeedItem

___

### capacity

• `Optional` **capacity**: ``null`` \| *number*

<div lang=\"ja\"> 在庫数です。<br> このフィールドは、リクエストの場合は省略可能です。 </div> 

**`memberof`** FeedItem

___

### displaySettings

• `Optional` **displaySettings**: ``null`` \| *number*

<div lang=\"ja\"> 配信設定です。<br> このフィールドは、リクエストの場合は省略可能です。<br> ※「0:配信しない/1:配信する」を表します。 </div> 

**`memberof`** FeedItem

___

### feedId

• `Optional` **feedId**: ``null`` \| *number*

<div lang=\"ja\"> Feedを識別するIDです。<br> このフィールドは、リクエストの場合は必須です。 </div> 

**`memberof`** FeedItem

___

### formattedPrice

• `Optional` **formattedPrice**: ``null`` \| *string*

<div lang=\"ja\"> 文字列の価格です。<br> このフィールドは、リクエストの場合は省略可能です。 </div> 

**`memberof`** FeedItem

___

### formattedSalePrice

• `Optional` **formattedSalePrice**: ``null`` \| *string*

<div lang=\"ja\"> 文字列のセール価格です。<br> このフィールドは、リクエストの場合は省略可能です。 </div> 

**`memberof`** FeedItem

___

### inStock

• `Optional` **inStock**: ``null`` \| *number*

<div lang=\"ja\"> 在庫情報です。<br> このフィールドは、リクエストの場合は省略可能です。<br> ※「0:在庫なし/1:在庫あり」を表します。 </div> 

**`memberof`** FeedItem

___

### isRemoveCapacity

• `Optional` **isRemoveCapacity**: ``null`` \| [*True*](./enums/feeditemserviceisremoveflg.md#true) \| [*False*](./enums/feeditemserviceisremoveflg.md#false) \| [*Unknown*](./enums/feeditemserviceisremoveflg.md#unknown)

**`memberof`** FeedItem

___

### isRemoveFormattedPrice

• `Optional` **isRemoveFormattedPrice**: ``null`` \| [*True*](./enums/feeditemserviceisremoveflg.md#true) \| [*False*](./enums/feeditemserviceisremoveflg.md#false) \| [*Unknown*](./enums/feeditemserviceisremoveflg.md#unknown)

**`memberof`** FeedItem

___

### isRemoveFormattedSalePrice

• `Optional` **isRemoveFormattedSalePrice**: ``null`` \| [*True*](./enums/feeditemserviceisremoveflg.md#true) \| [*False*](./enums/feeditemserviceisremoveflg.md#false) \| [*Unknown*](./enums/feeditemserviceisremoveflg.md#unknown)

**`memberof`** FeedItem

___

### isRemovePrice

• `Optional` **isRemovePrice**: ``null`` \| [*True*](./enums/feeditemserviceisremoveflg.md#true) \| [*False*](./enums/feeditemserviceisremoveflg.md#false) \| [*Unknown*](./enums/feeditemserviceisremoveflg.md#unknown)

**`memberof`** FeedItem

___

### isRemoveSalePrice

• `Optional` **isRemoveSalePrice**: ``null`` \| [*True*](./enums/feeditemserviceisremoveflg.md#true) \| [*False*](./enums/feeditemserviceisremoveflg.md#false) \| [*Unknown*](./enums/feeditemserviceisremoveflg.md#unknown)

**`memberof`** FeedItem

___

### itemId

• `Optional` **itemId**: ``null`` \| *string*

<div lang=\"ja\"> 商品IDです。<br> このフィールドは、リクエストの場合は必須です。 </div> 

**`memberof`** FeedItem

___

### price

• `Optional` **price**: ``null`` \| *number*

<div lang=\"ja\"> 価格です。<br> このフィールドは、リクエストの場合は省略可能です。 </div> 

**`memberof`** FeedItem

___

### salePrice

• `Optional` **salePrice**: ``null`` \| *number*

<div lang=\"ja\"> セール価格です。<br> このフィールドは、リクエストの場合は省略可能です。 </div> 

**`memberof`** FeedItem
