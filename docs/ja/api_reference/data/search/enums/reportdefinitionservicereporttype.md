# Enumeration: ReportDefinitionServiceReportType


<div lang=\"ja\">ReportDefinitionServiceReportTypeは、レポートの種類を表します。<br> ADD時、このフィールドは必須となります。</div>  <dl class=term>   <dt class=\"term__item\">ACCOUNT</dt>   <dd class=\"term__desc\"><span lang=\"ja\">アカウントレポートです。</span><span lang=\"en\">Account Report.<br>Performance data of selected account.</span></dd>   <dt class=\"term__item\">CAMPAIGN</dt>   <dd class=\"term__desc\"><span lang=\"ja\">キャンペーンレポートです。</span><span lang=\"en\">Campaign Report.<br>Performance data for selected campaigns.</span></dd>   <dt class=\"term__item\">ADGROUP</dt>   <dd class=\"term__desc\"><span lang=\"ja\">広告グループレポートです。</span><span lang=\"en\">Ad Group Report.<br>Performance data for selected ad group for one or more of campaigns.</span></dd>   <dt class=\"term__item\">AD</dt>   <dd class=\"term__desc\"><span lang=\"ja\">広告レポートです。</span><span lang=\"en\">Ad Report.<br>Performance data for selected ads.</span></dd>   <dt class=\"term__item\">KEYWORDS</dt>   <dd class=\"term__desc\"><span lang=\"ja\">キーワードレポートです。</span><span lang=\"en\">Keyword Report.<br>Performance data for selected keywords.</span></dd>   <dt class=\"term__item\">SEARCH_QUERY</dt>   <dd class=\"term__desc\"><span lang=\"ja\">検索クエリレポートです。</span><span lang=\"en\">Search Query Report.<br>Performance data for search queries which triggered the ad and received the clicks.</span></dd>   <dt class=\"term__item\">GEO</dt>   <dd class=\"term__desc\"><span lang=\"ja\">地域別レポートです。</span><span lang=\"en\">Geo Report.<br>Performance data by selected location.</span></dd>   <dt class=\"term__item\">FEED_ITEM</dt>   <dd class=\"term__desc\"><span lang=\"ja\">広告表示オプションレポートです。</span><span lang=\"en\">Ad Display Option Report.<br>Performance data for selected Quick Links and/or Call Extension.</span></dd>   <dt class=\"term__item\">GEO_TARGET</dt>   <dd class=\"term__desc\"><span lang=\"ja\">地域ターゲティングレポートです。</span><span lang=\"en\">Geo Targeting Report.<br>Performance data for location targeting.</span></dd>   <dt class=\"term__item\">SCHEDULE_TARGET</dt>   <dd class=\"term__desc\"><span lang=\"ja\">曜日・時間帯ターゲティングレポートです。</span><span lang=\"en\">Schedule Targeting Report.<br>Performance data in Day of Week / Hours.</span></dd>   <dt class=\"term__item\">BID_STRATEGY</dt>   <dd class=\"term__desc\"><span lang=\"ja\">自動入札レポートです。</span><span lang=\"en\">Auto Bidding Report.<br>Performance data for selected Auto Bidding.</span></dd>   <dt class=\"term__item\">CAMPAIGN_TARGET_LIST</dt>   <dd class=\"term__desc\"><span lang=\"ja\">キャンペーンターゲット設定レポートです。</span><span lang=\"en\">Canpaign Target Report.<br>Performance data for selected target list.</span></dd>   <dt class=\"term__item\">ADGROUP_TARGET_LIST</dt>   <dd class=\"term__desc\"><span lang=\"ja\">広告グループ設定レポートです。</span><span lang=\"en\">Ad Group Report.<br>Performance data for selected target list.</span></dd>   <dt class=\"term__item\">LANDING_PAGE_URL</dt>   <dd class=\"term__desc\"><span lang=\"ja\">最終リンク先URLレポートです。</span><span lang=\"en\">Landing Page Report.<br>Performance data for the final URL.</span></dd>   <dt class=\"term__item\">KEYWORDLESS_QUERY</dt>   <dd class=\"term__desc\"><span lang=\"ja\">検索クエリーレポート（動的検索連動型広告）です。</span></dd>   <dt class=\"term__item\">WEBPAGE_CRITERION</dt>   <dd class=\"term__desc\"><span lang=\"ja\">ページフィードターゲティングレポートです。</span></dd>   <dt class=\"term__item\">BID_MODIFIER</dt>   <dd class=\"term__desc\"><span lang=\"ja\">入札価格調整率レポートです。</span></dd>   <dt class=\"term__item\">CAMPAIGN_ASSET</dt>   <dd class=\"term__desc\"><span lang=\"ja\">（新）広告表示オプションレポート（キャンペーン）です。</span></dd>   <dt class=\"term__item\">ADGROUP_ASSET</dt>   <dd class=\"term__desc\"><span lang=\"ja\">（新）広告表示オプションレポート（広告グループ）です。</span></dd>   <dt class=\"term__item\">UNKNOWN</dt>   <dd class=\"term__desc\"><span lang=\"ja\">未知の値です。</span></dd> </dl>

## Table of contents

### Enumeration members

- [Account](reportdefinitionservicereporttype.md#account)
- [Ad](reportdefinitionservicereporttype.md#ad)
- [Adgroup](reportdefinitionservicereporttype.md#adgroup)
- [AdgroupAsset](reportdefinitionservicereporttype.md#adgroupasset)
- [AdgroupTargetList](reportdefinitionservicereporttype.md#adgrouptargetlist)
- [BidModifier](reportdefinitionservicereporttype.md#bidmodifier)
- [BidStrategy](reportdefinitionservicereporttype.md#bidstrategy)
- [Campaign](reportdefinitionservicereporttype.md#campaign)
- [CampaignAsset](reportdefinitionservicereporttype.md#campaignasset)
- [CampaignTargetList](reportdefinitionservicereporttype.md#campaigntargetlist)
- [FeedItem](reportdefinitionservicereporttype.md#feeditem)
- [Geo](reportdefinitionservicereporttype.md#geo)
- [GeoTarget](reportdefinitionservicereporttype.md#geotarget)
- [KeywordlessQuery](reportdefinitionservicereporttype.md#keywordlessquery)
- [Keywords](reportdefinitionservicereporttype.md#keywords)
- [LandingPageUrl](reportdefinitionservicereporttype.md#landingpageurl)
- [ScheduleTarget](reportdefinitionservicereporttype.md#scheduletarget)
- [SearchQuery](reportdefinitionservicereporttype.md#searchquery)
- [Unknown](reportdefinitionservicereporttype.md#unknown)
- [WebpageCriterion](reportdefinitionservicereporttype.md#webpagecriterion)

## Enumeration members

### Account

• **Account**: = "ACCOUNT"

___

### Ad

• **Ad**: = "AD"

___

### Adgroup

• **Adgroup**: = "ADGROUP"

___

### AdgroupAsset

• **AdgroupAsset**: = "ADGROUP\_ASSET"

___

### AdgroupTargetList

• **AdgroupTargetList**: = "ADGROUP\_TARGET\_LIST"

___

### BidModifier

• **BidModifier**: = "BID\_MODIFIER"

___

### BidStrategy

• **BidStrategy**: = "BID\_STRATEGY"

___

### Campaign

• **Campaign**: = "CAMPAIGN"

___

### CampaignAsset

• **CampaignAsset**: = "CAMPAIGN\_ASSET"

___

### CampaignTargetList

• **CampaignTargetList**: = "CAMPAIGN\_TARGET\_LIST"

___

### FeedItem

• **FeedItem**: = "FEED\_ITEM"

___

### Geo

• **Geo**: = "GEO"

___

### GeoTarget

• **GeoTarget**: = "GEO\_TARGET"

___

### KeywordlessQuery

• **KeywordlessQuery**: = "KEYWORDLESS\_QUERY"

___

### Keywords

• **Keywords**: = "KEYWORDS"

___

### LandingPageUrl

• **LandingPageUrl**: = "LANDING\_PAGE\_URL"

___

### ScheduleTarget

• **ScheduleTarget**: = "SCHEDULE\_TARGET"

___

### SearchQuery

• **SearchQuery**: = "SEARCH\_QUERY"

___

### Unknown

• **Unknown**: = "UNKNOWN"

___

### WebpageCriterion

• **WebpageCriterion**: = "WEBPAGE\_CRITERION"
