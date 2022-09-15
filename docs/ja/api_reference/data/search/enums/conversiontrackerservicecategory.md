# Enumeration: ConversionTrackerServiceCategory


<div lang=\"ja\">ConversionTrackerServiceCategoryは、トラッキング対象のコンバージョントラッカー情報のカテゴリです。<br> このフィールドは、ADD時に必須となり、SET時に省略可能となります。<br> *conversionTrackerTypeがAPP_LINK_CONVERSIONの場合、ADDおよびSET時にappEventTypeによって指定できる値に制限があります。<br>  appEventTypeはConversionTrackerService/getAppEventTypeで取得されるappEvent.appEventTypeで確認できます。<br> ・first_openの場合はDOWNLOADのみ選択できます。<br> ・in_app_purchaseの場合はPURCHASEのみ選択できます。<br> ・その他の場合はDOWNLOAD以外の値を選択できます。<br> </div>  <dl class=term>   <dt class=\"term__item\">DEFAULT</dt>   <dd class=\"term__desc\"><span lang=\"ja\">その他です。</span></dd>   <dt class=\"term__item\">PAGE_VIEW</dt>   <dd class=\"term__desc\"><span lang=\"ja\">主要なページの閲覧です。<br>重要なページなど特定ページの閲覧数の測定を行います。</span></dd>   <dt class=\"term__item\">PURCHASE</dt>   <dd class=\"term__desc\"><span lang=\"ja\">購入/販売です。<br>商品の注文やサービスへのお申し込みなど、販売につながった測定を行います。</span><span lang=\"en\">Purchase/Sold.<br>It is used to measure sales such as order and application of the items or service.</span></dd>   <dt class=\"term__item\">SIGNUP</dt>   <dd class=\"term__desc\"><span lang=\"ja\">契約です。<br>会員やメールマガジンの登録数などの測定を行います。</span></dd>   <dt class=\"term__item\">LEAD</dt>   <dd class=\"term__desc\"><span lang=\"ja\">販売促進です。<br>資料請求数やサービス、商品に関する問い合わせ数などの測定を行います。<br>※ADDまたはSET時、このEnumは指定できません。</span><span lang=\"en\">Sales promotion. It is used to measure inquiries for catalog, service or merchandise.<br>*This Enum cannot be specified in ADD and SET operation.</span></dd>   <dt class=\"term__item\">DOWNLOAD</dt>   <dd class=\"term__desc\"><span lang=\"ja\">ダウンロードです。<br>※広告管理ツールおよびレポート上での表示は「その他」になります。</span><span lang=\"en\"> Download.<br> *This will be displayed as Others in Campaign Management Tool and Reports. </span></dd>   <dt class=\"term__item\">UNKNOWN</dt>   <dd class=\"term__desc\"><span lang=\"ja\">未知の値です。</span></dd> </dl>

## Table of contents

### Enumeration members

- [Default](conversiontrackerservicecategory.md#default)
- [Download](conversiontrackerservicecategory.md#download)
- [Lead](conversiontrackerservicecategory.md#lead)
- [PageView](conversiontrackerservicecategory.md#pageview)
- [Purchase](conversiontrackerservicecategory.md#purchase)
- [Signup](conversiontrackerservicecategory.md#signup)
- [Unknown](conversiontrackerservicecategory.md#unknown)

## Enumeration members

### Default

• **Default**: = "DEFAULT"

___

### Download

• **Download**: = "DOWNLOAD"

___

### Lead

• **Lead**: = "LEAD"

___

### PageView

• **PageView**: = "PAGE\_VIEW"

___

### Purchase

• **Purchase**: = "PURCHASE"

___

### Signup

• **Signup**: = "SIGNUP"

___

### Unknown

• **Unknown**: = "UNKNOWN"
