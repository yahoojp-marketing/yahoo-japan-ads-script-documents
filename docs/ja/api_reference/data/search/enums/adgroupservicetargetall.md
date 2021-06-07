# Enumeration: AdGroupServiceTargetAll


<div lang=\"ja\">AdGroupServiceTargetAllは、サイトリターゲティングにおける配信対象ユーザーの設定内容を表します。<br> ADDおよびSET時、このフィールドは必須となります。<br> ※TargetingSettingが未設定の場合、ADD時のデフォルト設定値はACTIVEとなります。</div>  <dl class=term>   <dt class=\"term__item\">ACTIVE</dt>   <dd class=\"term__desc\"><span lang=\"ja\">すべてのユーザーを配信対象とします。<br>ターゲットリストのユーザーは入札価格調整率の適用のみ行います。</span><span lang=\"en\">All users are target of ad delivery.<br>Only applying bid adjustment rate is done for users on the Target List.</span></dd>   <dt class=\"term__item\">DEACTIVE</dt>   <dd class=\"term__desc\"><span lang=\"ja\">ターゲットリストのユーザーのみを配信対象とします。<br>また、ターゲットリストのユーザーに対して入札価格調整率を適用します。</span><span lang=\"en\">Users on the Target List are target of ad delivery.<br>And bid adjustment rate is applied to users on the Target List.</span></dd>   <dt class=\"term__item\">UNKNOWN</dt>   <dd class=\"term__desc\"><span lang=\"ja\">未知の値です。</span></dd> </dl>

## Table of contents

### Enumeration members

- [Active](adgroupservicetargetall.md#active)
- [Deactive](adgroupservicetargetall.md#deactive)
- [Unknown](adgroupservicetargetall.md#unknown)

## Enumeration members

### Active

• **Active**: = "ACTIVE"

___

### Deactive

• **Deactive**: = "DEACTIVE"

___

### Unknown

• **Unknown**: = "UNKNOWN"
