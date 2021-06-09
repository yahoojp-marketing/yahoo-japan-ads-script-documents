# AdGroupBidMultiplier


<div lang=\"ja\">AdGroupBidMultiplierオブジェクトは、入札価格調整率を表します。</div> 

## Table of contents

### Properties

- [accountId](adgroupbidmultiplier.md#accountid)
- [adGroupId](adgroupbidmultiplier.md#adgroupid)
- [bidMultiplier](adgroupbidmultiplier.md#bidmultiplier)
- [campaignId](adgroupbidmultiplier.md#campaignid)
- [platformType](adgroupbidmultiplier.md#platformtype)

## Properties

### accountId

• `Optional` **accountId**: ``null`` \| *number*

<div lang=\"ja\">アカウントIDです。<br> このフィールドは、レスポンスの際に返却されますが、リクエストの際には無視されます。</div> 

**`memberof`** AdGroupBidMultiplier

___

### adGroupId

• `Optional` **adGroupId**: ``null`` \| *number*

<div lang=\"ja\">広告グループIDです。<br> SETおよびREMOVE時、このフィールドは必須となります。</div> 

**`memberof`** AdGroupBidMultiplier

___

### bidMultiplier

• `Optional` **bidMultiplier**: ``null`` \| *number*

<div lang=\"ja\">入札価格調整率です。0～10.00まで指定できます。0を指定した場合、広告は配信されません。<br> また、入札価格調整率の値は小数点第二位まで指定可能です。<br> SET時、このフィールドは必須となります。</div> 

**`memberof`** AdGroupBidMultiplier

___

### campaignId

• `Optional` **campaignId**: ``null`` \| *number*

<div lang=\"ja\">キャンペーンIDです。<br> SETおよびREMOVE時、このフィールドは必須となります。</div> 

**`memberof`** AdGroupBidMultiplier

___

### platformType

• `Optional` **platformType**: ``null`` \| [*SmartPhone*](./enums/adgroupbidmultiplierserviceplatformtype.md#smartphone) \| [*Tablet*](./enums/adgroupbidmultiplierserviceplatformtype.md#tablet) \| [*Desktop*](./enums/adgroupbidmultiplierserviceplatformtype.md#desktop) \| [*Unknown*](./enums/adgroupbidmultiplierserviceplatformtype.md#unknown)

**`memberof`** AdGroupBidMultiplier
