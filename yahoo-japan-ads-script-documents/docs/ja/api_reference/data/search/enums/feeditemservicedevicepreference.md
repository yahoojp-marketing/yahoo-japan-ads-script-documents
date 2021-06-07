# Enumeration: FeedItemServiceDevicePreference


<div lang=\"ja\">FeedItemServiceDevicePreferenceは、広告を優先的に配信するデバイスを選択します。<br> このフィールドは、ADDおよびSET時に省略可能となり、REMOVE時に無視されます。<br> 電話番号オプションの場合、ADD時に省略可能となり、SET時に無視されます。<br> ※ADD時のデフォルト設定値はSMART_PHONEとなります。 </div>  <dl class=term>   <dt class=\"term__item\">SMART_PHONE</dt>   <dd class=\"term__desc\"><span lang=\"ja\">スマートフォンを優先的に配信します。<br>作成（add）時のみご利用いただけます。<br>※優先デバイスの変更（set）・削除（remove）は実施できません。</span><span lang=\"en\">Deliver ads to Smartphone in higher priority<br>Available for add operation only<br>It cannot be used in set or remove operation</span></dd>   <dt class=\"term__item\">NONE</dt>   <dd class=\"term__desc\"><span lang=\"ja\">指定なし</span></dd>   <dt class=\"term__item\">UNKNOWN</dt>   <dd class=\"term__desc\"><span lang=\"ja\">未知の値です。</span></dd> </dl>

## Table of contents

### Enumeration members

- [None](feeditemservicedevicepreference.md#none)
- [SmartPhone](feeditemservicedevicepreference.md#smartphone)
- [Unknown](feeditemservicedevicepreference.md#unknown)

## Enumeration members

### None

• **None**: = "NONE"

___

### SmartPhone

• **SmartPhone**: = "SMART\_PHONE"

___

### Unknown

• **Unknown**: = "UNKNOWN"
