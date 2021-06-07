# Enumeration: CampaignServiceServingStatus


<div lang=\"ja\">CampaignServiceServingStatusは、キャンペーンレベルの配信状況です。 ユーザーによる広告配信の調整に関わらず、キャンペーンとしての状態を表します。<br> このフィールドは、レスポンスの際に返却されますが、リクエストの際には無視されます。</div>  <dl class=term>   <dt class=\"term__item\">SERVING</dt>   <dd class=\"term__desc\"><span lang=\"ja\">キャンペーンは、現在配信されています。</span></dd>   <dt class=\"term__item\">ENDED</dt>   <dd class=\"term__desc\"><span lang=\"ja\">配信が終了しています。<br>設定されたキャンペーン期間後のため、現在配信されていません。</span><span lang=\"en\">The campaign has ended.<br>It is already past the delivery period, so the campaign is currently not serving ads.</span></dd>   <dt class=\"term__item\">PENDING</dt>   <dd class=\"term__desc\"><span lang=\"ja\">配信が開始していません。<br>設定されたキャンペーン期間前のため、現在まだ配信されていません。</span><span lang=\"en\">The campaign has not started.<br>It has not reached the delivery period, so the campaign is currently not serving ads.</span></dd>   <dt class=\"term__item\">STOP</dt>   <dd class=\"term__desc\"><span lang=\"ja\">キャンペーンは、現在配信されていません。</span><span lang=\"en\">The campaign has been suspended.<br>(Reason may from lack of allocated funds)</span></dd>   <dt class=\"term__item\">UNKNOWN</dt>   <dd class=\"term__desc\"><span lang=\"ja\">未知の値です。</span></dd> </dl>

## Table of contents

### Enumeration members

- [Ended](campaignserviceservingstatus.md#ended)
- [Pending](campaignserviceservingstatus.md#pending)
- [Serving](campaignserviceservingstatus.md#serving)
- [Stop](campaignserviceservingstatus.md#stop)
- [Unknown](campaignserviceservingstatus.md#unknown)

## Enumeration members

### Ended

• **Ended**: = "ENDED"

___

### Pending

• **Pending**: = "PENDING"

___

### Serving

• **Serving**: = "SERVING"

___

### Stop

• **Stop**: = "STOP"

___

### Unknown

• **Unknown**: = "UNKNOWN"
