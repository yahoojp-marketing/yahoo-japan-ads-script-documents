# Enumeration: AdGroupServiceDeviceAppType


<div lang=\"ja\"> AdGroupServiceDeviceAppTypeは、配信先のアプリケーション種別を表します。<br> ADDおよびSET時、このフィールドは省略可能となります。<br> deviceTypeがDESKTOPまたはWAP_MOBILEの場合は、deviceAppTypeを指定することはできません。<br> deviceTypeがNONEの場合は、deviceAppTypeまたはdeviceOsTypeのいずれかを指定する必要があります。 </div>  <dl class=term>   <dt class=\"term__item\">APP</dt>   <dd class=\"term__desc\"><span lang=\"ja\">アプリ向けに配信されます。</span></dd>   <dt class=\"term__item\">WEB</dt>   <dd class=\"term__desc\"><span lang=\"ja\">ウェブサイト向けに配信されます。</span></dd>   <dt class=\"term__item\">NONE</dt>   <dd class=\"term__desc\"><span lang=\"ja\">すべてに配信されます。<br>※AdGroupServiceのみ設定可能</span><span lang=\"en\">Deliver to all devices.<br>*Setting NONE is only available for AdGroupService.</span></dd>   <dt class=\"term__item\">UNKNOWN</dt>   <dd class=\"term__desc\"><span lang=\"ja\">未知の値です。</span></dd> </dl>

## Table of contents

### Enumeration members

- [App](adgroupservicedeviceapptype.md#app)
- [None](adgroupservicedeviceapptype.md#none)
- [Unknown](adgroupservicedeviceapptype.md#unknown)
- [Web](adgroupservicedeviceapptype.md#web)

## Enumeration members

### App

• **App**: = "APP"

___

### None

• **None**: = "NONE"

___

### Unknown

• **Unknown**: = "UNKNOWN"

___

### Web

• **Web**: = "WEB"
