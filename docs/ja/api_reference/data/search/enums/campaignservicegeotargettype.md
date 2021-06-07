# Enumeration: CampaignServiceGeoTargetType


<div lang=\"ja\">CampaignServiceGeoTargetTypeは、地域ターゲティングの地域判定の詳細設定を指定します。<br> ADD時、このフィールドは省略可能となります。その際、デフォルト設定値はDONT_CAREとなります。</div>  <dl class=term>   <dt class=\"term__item\">DONT_CARE</dt>   <dd class=\"term__desc\"><span lang=\"ja\">ターゲット地域設定の場合：<br>対象地域に所在する可能性があるユーザー、対象地域に関連する語句で検索したユーザー、対象地域に関心を示している可能性のあるユーザーに広告を配信します。<br>除外ターゲット地域設定の場合：<br>対象地域に所在する可能性があるユーザー、対象地域に関連する語句で検索したユーザー、対象地域に関心を示している可能性のあるユーザーには広告を配信しません。</span><span lang=\"en\">Positive Geo Target (Advanced location options):<br>Your ads will be displayed to users who may be in the target areas, to users who searched with queries including the targeted locations, to users who may be interested in the target area.<br>Negative Geo Target (Location exclusion options):<br>Your ads will not be displayed to users who may stay in the targeted area, who searched with queries including the targeted locations, to users who may be interested in the area.</span></dd>   <dt class=\"term__item\">AREA_OF_INTENT</dt>   <dd class=\"term__desc\"><span lang=\"ja\">ターゲット地域設定の場合：<br>対象地域に関連する語句で検索したユーザーや、対象地域に関心を示している可能性のあるユーザーのみに広告を配信します。<br>※除外ターゲット地域設定の場合は選択できません。</span><span lang=\"en\">Positive Geo Target (Advanced location options):<br>Your ads will be displayed to users who searched with queries including the targeted locations, to users who may be interested in the target area.<br>* This is not selectable with Negative Geo Target (Location exclusion options).</span></dd>   <dt class=\"term__item\">LOCATION_OF_PRESENCE</dt>   <dd class=\"term__desc\"><span lang=\"ja\">ターゲット地域設定の場合：<br>対象地域に所在する可能性があるユーザーにのみ、広告を配信します。<br>除外ターゲット地域設定の場合：対象地域に所在する可能性があるユーザーには、広告は配信されません。</span><span lang=\"en\">Positive Geo Target (Advanced location options):<br>Your ads will be displayed only to users who may be in the targeted area.<br>Negative Geo Target (Location Exclusion options):<br>Your ads will not be displayed to users who may be in the targeted areas.</span></dd>   <dt class=\"term__item\">UNKNOWN</dt>   <dd class=\"term__desc\"><span lang=\"ja\">未知の値です。</span></dd> </dl>

## Table of contents

### Enumeration members

- [AreaOfIntent](campaignservicegeotargettype.md#areaofintent)
- [DontCare](campaignservicegeotargettype.md#dontcare)
- [LocationOfPresence](campaignservicegeotargettype.md#locationofpresence)
- [Unknown](campaignservicegeotargettype.md#unknown)

## Enumeration members

### AreaOfIntent

• **AreaOfIntent**: = "AREA\_OF\_INTENT"

___

### DontCare

• **DontCare**: = "DONT\_CARE"

___

### LocationOfPresence

• **LocationOfPresence**: = "LOCATION\_OF\_PRESENCE"

___

### Unknown

• **Unknown**: = "UNKNOWN"
