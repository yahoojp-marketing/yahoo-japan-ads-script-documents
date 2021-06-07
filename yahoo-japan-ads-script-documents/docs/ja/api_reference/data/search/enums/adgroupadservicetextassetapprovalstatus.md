# Enumeration: AdGroupAdServiceTextAssetApprovalStatus


<div lang=\"ja\">AdGroupAdServiceTextAssetApprovalStatusは、審査状況を表します。<br> このフィールドは、レスポンスの際に返却されますが、リクエストの際には無視されます。</div>  <dl class=term>   <dt class=\"term__item\">APPROVED</dt>   <dd class=\"term__desc\"><span lang=\"ja\">承認済です。</span></dd>   <dt class=\"term__item\">REVIEW</dt>   <dd class=\"term__desc\"><span lang=\"ja\">審査中です。<br>新しく追加した広告テキストアセットが審査中となり、広告テキストアセットは未掲載です。</span><span lang=\"en\">Under editorial review<br>Newly added ad text asset are under review, and not displayed yet</span></dd>   <dt class=\"term__item\">PRE_DISAPPROVED</dt>   <dd class=\"term__desc\"><span lang=\"ja\">掲載不可です。<br>新しく追加した広告テキストアセットが審査で承認されず非掲載です。</span><span lang=\"en\">The item was rejected<br>Newly added ad text asset have been rejected, so it cannot be displayed</span></dd>   <dt class=\"term__item\">UNKNOWN</dt>   <dd class=\"term__desc\"><span lang=\"ja\">未知の値です。</span></dd> </dl>

## Table of contents

### Enumeration members

- [Approved](adgroupadservicetextassetapprovalstatus.md#approved)
- [PreDisapproved](adgroupadservicetextassetapprovalstatus.md#predisapproved)
- [Review](adgroupadservicetextassetapprovalstatus.md#review)
- [Unknown](adgroupadservicetextassetapprovalstatus.md#unknown)

## Enumeration members

### Approved

• **Approved**: = "APPROVED"

___

### PreDisapproved

• **PreDisapproved**: = "PRE\_DISAPPROVED"

___

### Review

• **Review**: = "REVIEW"

___

### Unknown

• **Unknown**: = "UNKNOWN"
