# Enumeration: ReportDefinitionServiceFrequencyRange


<div lang=\"ja\"> ReportDefinitionServiceFrequencyRangeは、フリークエンシーの計測期間を表します。<br> このフィールドは、ADD時に省略可能となり、REMOVE時に無視されます。 </div>  <dl class=term>   <dt class=\"term__item\">DAILY</dt>   <dd class=\"term__desc\"><span lang=\"ja\">1日単位です。</span></dd>   <dt class=\"term__item\">WEEKLY</dt>   <dd class=\"term__desc\"><span lang=\"ja\">1週間単位です。</span></dd>   <dt class=\"term__item\">MONTHLY</dt>   <dd class=\"term__desc\"><span lang=\"ja\">1ヶ月単位です。</span></dd>   <dt class=\"term__item\">GUARANTEED_CAMPAIGN_PERIOD</dt>   <dd class=\"term__desc\">   <span lang=\"ja\">     通期です。<br>     リーチレポートでのみ指定可能です。<br>     通期を指定する場合は、reportDateRangeTypeでもGUARANTEED_CAMPAIGN_PERIODを指定する必要があります。<br>     ※この「通期」は、予約型キャンペーンの開始から終了までの全期間を意味します。   </span>   <span lang=\"en\">     Lifetime.<br>     Can be specified only in the reach report.<br>     If specified this, \"GUARANTEED_CAMPAIGN_PERIOD\" must be specified for reportDateRangeType as well.<br>     * \"lifetime\" means the entire period from the start to the end of the guaranteed campaign.   </span> </dd>   <dt class=\"term__item\">UNKNOWN</dt>   <dd class=\"term__desc\"><span lang=\"ja\">未知の値です。</span></dd> </dl>

## Table of contents

### Enumeration members

- [Daily](reportdefinitionservicefrequencyrange.md#daily)
- [GuaranteedCampaignPeriod](reportdefinitionservicefrequencyrange.md#guaranteedcampaignperiod)
- [Monthly](reportdefinitionservicefrequencyrange.md#monthly)
- [Unknown](reportdefinitionservicefrequencyrange.md#unknown)
- [Weekly](reportdefinitionservicefrequencyrange.md#weekly)

## Enumeration members

### Daily

• **Daily**: = "DAILY"

___

### GuaranteedCampaignPeriod

• **GuaranteedCampaignPeriod**: = "GUARANTEED\_CAMPAIGN\_PERIOD"

___

### Monthly

• **Monthly**: = "MONTHLY"

___

### Unknown

• **Unknown**: = "UNKNOWN"

___

### Weekly

• **Weekly**: = "WEEKLY"
