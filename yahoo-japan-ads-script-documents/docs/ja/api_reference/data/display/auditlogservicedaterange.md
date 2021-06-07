# AuditLogServiceDateRange


<div lang=\"ja\"> AuditLogServiceDateRangeは、addメソッド実行時にダウンロード対象とする更新期間を保持するオブジェクトです。<br> このフィールドは、リクエストの場合は省略可能となります。 </div> 

## Table of contents

### Properties

- [endDate](auditlogservicedaterange.md#enddate)
- [startDate](auditlogservicedaterange.md#startdate)

## Properties

### endDate

• `Optional` **endDate**: ``null`` \| *string*

<div lang=\"ja\"> 終了日付です。<br> このフィールドは、リクエストの場合は省略可能となります。<br> ・入力形式：Ymd形式<br> ・デフォルト値：現在の日付<br> ・指定可能範囲：現在の日付<br> ※終了日付は開始日付以降の日付を指定してください。<br> ※開始日付から終了日付の期間は最大1カ月です。 </div> 

**`memberof`** AuditLogServiceDateRange

___

### startDate

• `Optional` **startDate**: ``null`` \| *string*

<div lang=\"ja\"> 開始日付です。<br> このフィールドは、リクエストの場合は省略可能となります。<br> ・入力形式：Ymd形式<br> ・デフォルト値：現在の日付<br> ・指定可能範囲：前月の月初<br> 例：4/30時点で、開始日付に指定できるもっとも古い日付は3/1 </div> 

**`memberof`** AuditLogServiceDateRange
