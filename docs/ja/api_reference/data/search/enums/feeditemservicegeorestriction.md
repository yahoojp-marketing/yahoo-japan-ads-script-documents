# Enumeration: FeedItemServiceGeoRestriction


<div lang=\"ja\">FeedItemServiceGeoRestrictionオブジェクトは、地域設定の配信を制御します。<br> このフィールドは、ADDおよびSET時に省略可能となり、REMOVE時に無視されます。<br> ※ADD時のデフォルト設定値はNONEとなります。 </div>  <dl class=term>   <dt class=\"term__item\">NONE</dt>   <dd class=\"term__desc\"><span lang=\"ja\">検索キーワードとユーザーの所在地の関係にかかわらず、配信されます。</span></dd>   <dt class=\"term__item\">LOCATION_OF_PRESENCE</dt>   <dd class=\"term__desc\"><span lang=\"ja\">検索キーワードがユーザーの所在地と無関係の場合は配信されません。</span></dd>   <dt class=\"term__item\">UNKNOWN</dt>   <dd class=\"term__desc\"><span lang=\"ja\">未知の値です。</span></dd> </dl>

## Table of contents

### Enumeration members

- [LocationOfPresence](feeditemservicegeorestriction.md#locationofpresence)
- [None](feeditemservicegeorestriction.md#none)
- [Unknown](feeditemservicegeorestriction.md#unknown)

## Enumeration members

### LocationOfPresence

• **LocationOfPresence**: = "LOCATION\_OF\_PRESENCE"

___

### None

• **None**: = "NONE"

___

### Unknown

• **Unknown**: = "UNKNOWN"
