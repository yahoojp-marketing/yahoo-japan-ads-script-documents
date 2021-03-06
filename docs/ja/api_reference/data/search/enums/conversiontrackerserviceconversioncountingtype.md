# Enumeration: ConversionTrackerServiceConversionCountingType


<div lang=\"ja\">ConversionTrackerServiceConversionCountingTypeは、コンバージョンの計測方法を表します。<br> このフィールドは、ADDおよびSET時に省略可能となります。<br> ※ADD時のデフォルト設定値はONE_PER_CLICKとなります。<br> ※conversionTrackerTypeがAPP_LINK_CONVERSIONの場合、ADDおよびSET時にappEventTypeがfirst_openの場合はONE_PER_CLICKのみ指定可能となります。<br> appEventTypeはConversionTrackerService/getAppEventTypeで取得されるappEvent.appEventTypeで確認できます。</div>  <dl class=term>   <dt class=\"term__item\">ONE_PER_CLICK</dt>   <dd class=\"term__desc\"><span lang=\"ja\">ユニークコンバージョンです。</span></dd>   <dt class=\"term__item\">MANY_PER_CLICK</dt>   <dd class=\"term__desc\"><span lang=\"ja\">総コンバージョンです。</span></dd>   <dt class=\"term__item\">UNKNOWN</dt>   <dd class=\"term__desc\"><span lang=\"ja\">未知の値です。</span></dd> </dl>

## Table of contents

### Enumeration members

- [ManyPerClick](conversiontrackerserviceconversioncountingtype.md#manyperclick)
- [OnePerClick](conversiontrackerserviceconversioncountingtype.md#oneperclick)
- [Unknown](conversiontrackerserviceconversioncountingtype.md#unknown)

## Enumeration members

### ManyPerClick

• **ManyPerClick**: = "MANY\_PER\_CLICK"

___

### OnePerClick

• **OnePerClick**: = "ONE\_PER\_CLICK"

___

### Unknown

• **Unknown**: = "UNKNOWN"
