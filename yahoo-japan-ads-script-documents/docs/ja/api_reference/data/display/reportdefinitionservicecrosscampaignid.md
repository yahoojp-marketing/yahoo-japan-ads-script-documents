# ReportDefinitionServiceCrossCampaignId


<div lang=\"ja\"> ReportDefinitionServiceCrossCampaignIdは、横断リーチレポートの組み合わせの対象となるアカウントおよびキャンペーンIDを示します。<br> このフィールドは、ADD時に省略可能となり、REMOVE時に無視されます。<br> ※ADD時、crossCampaignTypeが<code>CAMPAIGN_ID</code>の場合は必須です。 </div> 

## Table of contents

### Properties

- [account](reportdefinitionservicecrosscampaignid.md#account)
- [campaignId](reportdefinitionservicecrosscampaignid.md#campaignid)

## Properties

### account

• `Optional` **account**: ``null`` \| [*ReportDefinitionServiceAccount*](reportdefinitionserviceaccount.md)

**`memberof`** ReportDefinitionServiceCrossCampaignId

___

### campaignId

• `Optional` **campaignId**: ``null`` \| *number*

<div lang=\"ja\">   横断リーチレポートの組み合わせの対象となるキャンペーンIDです。<br>   このフィールドは、ADD時に省略可能となり、REMOVE時に無視されます。<br>   ※ADD時、crossCampaignReachTypeが<code>CAMPAIGN_ID</code>の場合は必須です。 </div> 

**`memberof`** ReportDefinitionServiceCrossCampaignId
