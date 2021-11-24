# Enumeration: AdGroupServiceDeviceOsType


<div lang=\"ja\"> AdGroupServiceDeviceOsTypeは、配信先デバイスのOSの種類を表します。<br> ADDおよびSET時、このフィールドは省略可能となります。<br> deviceTypeがDESKTOPまたはWAP_MOBILEの場合は、deviceOsTypeを指定することはできません。<br> deviceAppTypeがNONEの場合は、deviceOsTypeを指定することはできません。<br> deviceTypeがNONEの場合は、deviceAppTypeまたはdeviceOsTypeのいずれかを指定する必要があります。 </div>  <dl class=term>   <dt class=\"term__item\">IOS</dt>   <dd class=\"term__desc\"><span lang=\"ja\">iOS向けに配信されます。</span></dd>   <dt class=\"term__item\">ANDROID</dt>   <dd class=\"term__desc\"><span lang=\"ja\">Android向けに配信されます。</span></dd>   <dt class=\"term__item\">NONE</dt>   <dd class=\"term__desc\"><span lang=\"ja\">すべてのOSに配信されます。<br>※AdGroupServiceのみ設定可能</span><span lang=\"en\">Deliver to all OS.<br>*Setting NONE is only available for AdGroupService.</span></dd>   <dt class=\"term__item\">UNKNOWN</dt>   <dd class=\"term__desc\"><span lang=\"ja\">未知の値です。</span></dd> </dl>

## Table of contents

### Enumeration members

- [Android](adgroupservicedeviceostype.md#android)
- [Ios](adgroupservicedeviceostype.md#ios)
- [None](adgroupservicedeviceostype.md#none)
- [Unknown](adgroupservicedeviceostype.md#unknown)

## Enumeration members

### Android

• **Android**: = "ANDROID"

___

### Ios

• **Ios**: = "IOS"

___

### None

• **None**: = "NONE"

___

### Unknown

• **Unknown**: = "UNKNOWN"
