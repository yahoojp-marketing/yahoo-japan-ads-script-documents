# AuditLogServiceDateRange


<div lang=\"ja\">AuditLogServiceDateRangeオブジェクトは操作履歴を取得する条件、期間を示します。<br> このフィールドは、必須です。</div> 

## Table of contents

### Properties

- [endDate](auditlogservicedaterange.md#enddate)
- [startDate](auditlogservicedaterange.md#startdate)

## Properties

### endDate

• `Optional` **endDate**: ``null`` \| *string*

<div lang=\"ja\">対象期間の終了日です。<br> このフィールドは、必須です。<br> ※1 「YYYYMMDDhhmmss」形式です。秒単位まで指定できます。<br> 時間の指定がない場合は、0:00:00として扱われます。<br>　 【例】2016年5月25日 午後2時5分35秒に設定したい場合：20160525140535<br> ※2 日付は19700101～20371231まで設定可能です。</div> 

**`memberof`** AuditLogServiceDateRange

___

### startDate

• `Optional` **startDate**: ``null`` \| *string*

<div lang=\"ja\">対象期間の開始日です。<br> このフィールドは、必須です。<br> ※1 「YYYYMMDDhhmmss」形式です。秒単位まで指定できます。<br> 時間の指定がない場合は、0:00:00として扱われます。<br>　 【例】2016年5月25日 午後2時5分35秒に設定したい場合：20160525140535<br> ※2 日付は19700101～20371231まで設定可能です。</div> 

**`memberof`** AuditLogServiceDateRange
