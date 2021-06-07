# ReportDefinitionServiceCrossCampaignBuying


<div lang=\"ja\"> ReportDefinitionServiceCrossCampaignBuyingは、横断リーチレポートの組み合わせの対象となるアカウントおよびキャンペーン購入タイプを示します。<br> このフィールドは、ADD時に省略可能となり、REMOVE時に無視されます。<br> ※ADD時、crossCampaignTypeが<code>CAMPAIGN_BUYING_TYPE</code>の場合は必須です。 </div> 

## Table of contents

### Properties

- [account](reportdefinitionservicecrosscampaignbuying.md#account)
- [campaignBuyingType](reportdefinitionservicecrosscampaignbuying.md#campaignbuyingtype)

## Properties

### account

• `Optional` **account**: ``null`` \| [*ReportDefinitionServiceAccount*](reportdefinitionserviceaccount.md)

**`memberof`** ReportDefinitionServiceCrossCampaignBuying

___

### campaignBuyingType

• `Optional` **campaignBuyingType**: ``null`` \| [*Auction*](./enums/reportdefinitionservicecrosscampaignbuyingtype.md#auction) \| [*Guaranteed*](./enums/reportdefinitionservicecrosscampaignbuyingtype.md#guaranteed) \| [*Unknown*](./enums/reportdefinitionservicecrosscampaignbuyingtype.md#unknown)

**`memberof`** ReportDefinitionServiceCrossCampaignBuying
