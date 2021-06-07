# ReportDefinitionServiceCrossCampaignGoal


<div lang=\"ja\"> ReportDefinitionServiceCrossCampaignGoalは、横断リーチレポートの組み合わせの対象となるアカウントおよびキャンペーン目的を示します。<br> このフィールドは、ADD時に省略可能となり、REMOVE時に無視されます。<br> ※ADD時、crossCampaignTypeが<code>CAMPAIGN_GOAL</code>の場合は必須です。 </div> 

## Table of contents

### Properties

- [account](reportdefinitionservicecrosscampaigngoal.md#account)
- [campaignGoal](reportdefinitionservicecrosscampaigngoal.md#campaigngoal)

## Properties

### account

• `Optional` **account**: ``null`` \| [*ReportDefinitionServiceAccount*](reportdefinitionserviceaccount.md)

**`memberof`** ReportDefinitionServiceCrossCampaignGoal

___

### campaignGoal

• `Optional` **campaignGoal**: ``null`` \| *string*

<div lang=\"ja\">   横断リーチレポートの組み合わせの対象となるキャンペーン目的です。<br>   このフィールドは、ADD時に省略可能となり、REMOVE時に無視されます。<br>   ※ADD時、crossCampaignReachTypeが<code>CAMPAIGN_GOAL</code>の場合は必須です。<br>   ※BRAND_AWARENESSを指定すると「運用型：ブランド認知」と「予約型：ブランド認知」の両方が対象になります。<br>   ※BRAND_AWARENESS_GUARANTEEDは指定できません。 </div> 

**`memberof`** ReportDefinitionServiceCrossCampaignGoal
