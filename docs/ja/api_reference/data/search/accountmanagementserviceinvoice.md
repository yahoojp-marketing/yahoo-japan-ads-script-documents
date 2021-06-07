# AccountManagementServiceInvoice


<div lang=\"ja\">AccountManagementServiceInvoiceオブジェクトは、後金支払情報を表します。<br> このフィールドは、ADD時は必須となり、SET時は省略可能となります。</div> 

## Table of contents

### Properties

- [budgetAmount](accountmanagementserviceinvoice.md#budgetamount)
- [endDate](accountmanagementserviceinvoice.md#enddate)
- [startDate](accountmanagementserviceinvoice.md#startdate)

## Properties

### budgetAmount

• `Optional` **budgetAmount**: ``null`` \| *number*

<div lang=\"ja\">金額です。<br> ※1,000単位、3,000以上999,999,999,999,000以内です。<br> このフィールドは、ADD時に必須となり、SET時に省略可能となります。</div> 

**`memberof`** AccountManagementServiceInvoice

___

### endDate

• `Optional` **endDate**: ``null`` \| *string*

<div lang=\"ja\">終了日です。※YYYYMMDD形式です。<br> ADDおよびSET時、このフィールドは省略可能となります。その際、ADD時のデフォルト設定値は20371231となり、『設定なし』と同義となります。<br> 20371231を指定した場合も『設定なし』となります。<br>SET時に『設定なし』に設定する場合は、20371231を指定してください。</div> 

**`memberof`** AccountManagementServiceInvoice

___

### startDate

• `Optional` **startDate**: ``null`` \| *string*

<div lang=\"ja\">開始日です。※YYYYMMDD形式です。<br> このフィールドは、レスポンスの際に返却されますが、リクエストの際には無視されます。※自動でADD時の日付が登録されます。</div> 

**`memberof`** AccountManagementServiceInvoice
