# Enumeration: FeedItemServiceIsRemove


<div lang=\"ja\">FeedItemServiceIsRemoveは、カスタムパラメータの削除フラグです。<br> customParametersおよびreviewCustomParameters配下の場合、このフィールドはSET時に省略可能となります。<br> locationオブジェクト配下の場合、このフィールドは、ADDおよびREMOVE時に無視され、SET時に省略可能となります。<br> ※地域設定を解除する場合は、locationオブジェクトのisRemoveにTRUEを指定します。<br> 地域設定解除後は、geoTargetingRestrictionにNONEが設定されます。</div>  <dl class=term>   <dt class=\"term__item\">TRUE</dt>   <dd class=\"term__desc\"><span lang=\"ja\">カスタムパラメータの削除フラグがオンです。</span></dd>   <dt class=\"term__item\">FALSE</dt>   <dd class=\"term__desc\"><span lang=\"ja\">カスタムパラメータの削除フラグがオフです。</span></dd>   <dt class=\"term__item\">UNKNOWN</dt>   <dd class=\"term__desc\"><span lang=\"ja\">未知の値です。</span></dd> </dl>

## Table of contents

### Enumeration members

- [False](feeditemserviceisremove.md#false)
- [True](feeditemserviceisremove.md#true)
- [Unknown](feeditemserviceisremove.md#unknown)

## Enumeration members

### False

• **False**: = "FALSE"

___

### True

• **True**: = "TRUE"

___

### Unknown

• **Unknown**: = "UNKNOWN"
