# Enumeration: ReportDefinitionServiceReportIncludeDeleted


<div lang=\"ja\">ReportDefinitionServiceReportIncludeDeletedオブジェクトは、削除済みの項目をレポートに出力するかを選択します。<br> レポートタイプがCAMPAIGN, ADGROUP, AD, KEYWORDS, FEED_ITEM, AD_CUSTOMIZERS, WEBPAGE_CRITERIONの場合のみ、ADD時にこのフィールドは省略可能となります。<br> それ以外のレポートタイプの場合、ADD時、このフィールドは無視されます。<br> reportIncludeDeletedがFALSEの場合、以下エンティティはレポートに出力されません。</div>  <table border=\"1\"> <tr><th>reportType</th><th>entity</th></tr> <tr><td>CAMPAIGN</td><td>CAMPAIGN</td></tr> <tr><td>ADGROUP</td><td>CAMPAIGN, ADGROUP</td></tr> <tr><td>AD</td><td>CAMPAIGN, ADGROUP, AD</td></tr> <tr><td>KEYWORD</td><td>CAMPAIGN, ADGROUP, KEYWORD</td></tr> <tr><td>FEED_ITEM</td><td>FEED_ITEM</td></tr> <tr><td>AD_CUSTOMIZERS</td><td>FEED_ITEM</td></tr> <tr><td>WEBPAGE_CRITERION</td><td>CAMPAIGN, ADGROUP, CRITERION</td></tr> </table> <dl class=term>   <dt class=\"term__item\">TRUE</dt>   <dd class=\"term__desc\"><span lang=\"ja\">出力します。<br>※デフォルトに設定されます。</span><span lang=\"en\">Output.<br>*Default setting.</span></dd>   <dt class=\"term__item\">FALSE</dt>   <dd class=\"term__desc\"><span lang=\"ja\">出力しません。</span></dd>   <dt class=\"term__item\">UNKNOWN</dt>   <dd class=\"term__desc\"><span lang=\"ja\">未知の値です。</span></dd> </dl>

## Table of contents

### Enumeration members

- [False](reportdefinitionservicereportincludedeleted.md#false)
- [True](reportdefinitionservicereportincludedeleted.md#true)
- [Unknown](reportdefinitionservicereportincludedeleted.md#unknown)

## Enumeration members

### False

• **False**: = "FALSE"

___

### True

• **True**: = "TRUE"

___

### Unknown

• **Unknown**: = "UNKNOWN"
