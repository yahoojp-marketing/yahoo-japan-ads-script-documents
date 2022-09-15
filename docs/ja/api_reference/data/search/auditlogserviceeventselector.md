# AuditLogServiceEventSelector


<div lang=\"ja\">AuditLogServiceEventSelectorオブジェクトは、操作履歴の取得対象を設定します。<br> このフィールドは、必須です。</div> 

## Table of contents

### Properties

- [entityType](auditlogserviceeventselector.md#entitytype)
- [eventTypes](auditlogserviceeventselector.md#eventtypes)

## Properties

### entityType

• `Optional` **entityType**: ``null`` \| *string*

<div lang=\"ja\">AuditLogServiceEntityTypeオブジェクトは、操作履歴に出力するエンティティの種類を表します。</div>  <dl class=term>   <dt class=\"term__item\">CAMPAIGN</dt>   <dd class=\"term__desc\"><span lang=\"ja\">キャンペーンです。</span></dd>   <dt class=\"term__item\">NEGATIVE_CAMPAIGN_CRITERION</dt>   <dd class=\"term__desc\"><span lang=\"ja\">対象外キーワードです（キャンペーン）。</span></dd>   <dt class=\"term__item\">CAMPAIGN_CRITERION</dt>   <dd class=\"term__desc\"><span lang=\"ja\">キャンペーンのターゲティング設定です。</span></dd>   <dt class=\"term__item\">AD_GROUP</dt>   <dd class=\"term__desc\"><span lang=\"ja\">広告グループです。</span></dd>   <dt class=\"term__item\">AD_GROUP_BID_MULTIPLIER</dt>   <dd class=\"term__desc\"><span lang=\"ja\">広告グループ入札価格調整率です。</span></dd>   <dt class=\"term__item\">BIDDABLE_AD_GROUP_CRITERION</dt>   <dd class=\"term__desc\"><span lang=\"ja\">入札キーワードです。</span></dd>   <dt class=\"term__item\">NEGATIVE_AD_GROUP_CRITERION</dt>   <dd class=\"term__desc\"><span lang=\"ja\">対象外キーワードです（広告グループ）。</span></dd>   <dt class=\"term__item\">AD</dt>   <dd class=\"term__desc\"><span lang=\"ja\">広告です。</span></dd>   <dt class=\"term__item\">FEED</dt>   <dd class=\"term__desc\"><span lang=\"ja\">Feedフォルダーです。</span></dd>   <dt class=\"term__item\">FEED_ITEM</dt>   <dd class=\"term__desc\"><span lang=\"ja\">広告表示オプションです。</span></dd>   <dt class=\"term__item\">CAMPAIGN_FEED</dt>   <dd class=\"term__desc\"><span lang=\"ja\">広告表示オプションです（キャンペーン）。</span></dd>   <dt class=\"term__item\">AD_GROUP_FEED</dt>   <dd class=\"term__desc\"><span lang=\"ja\">広告表示オプションです（広告グループ）。</span></dd>   <dt class=\"term__item\">SS_IO</dt>   <dd class=\"term__desc\"><span lang=\"ja\">アカウントです。</span></dd>   <dt class=\"term__item\">SS_CONVERSION</dt>   <dd class=\"term__desc\"><span lang=\"ja\">コンバージョントラッカー（コンバージョン測定）です。</span></dd>   <dt class=\"term__item\">BIDDING_STRATEGY</dt>   <dd class=\"term__desc\"><span lang=\"ja\">自動入札設定です。</span></dd>   <dt class=\"term__item\">NEGATIVE_CAMPAIGN_USER_LIST</dt>   <dd class=\"term__desc\"><span lang=\"ja\">対象外ターゲットリストです（キャンペーン）。</span></dd>   <dt class=\"term__item\">NEGATIVE_AD_GROUP_USER_LIST</dt>   <dd class=\"term__desc\"><span lang=\"ja\">対象外ターゲットリストです（広告グループ）。</span></dd>   <dt class=\"term__item\">AD_GROUP_USER_LIST</dt>   <dd class=\"term__desc\"><span lang=\"ja\">ターゲットリストです（広告グループ）。</span></dd>   <dt class=\"term__item\">TARGET_LIST</dt>   <dd class=\"term__desc\"><span lang=\"ja\">サイトリターゲテイングのターゲットリストです。</span></dd>   <dt class=\"term__item\">SHARED_SET</dt>   <dd class=\"term__desc\"><span lang=\"ja\">共有リストです。</span></dd>   <dt class=\"term__item\">SHARED_CRITERION</dt>   <dd class=\"term__desc\"><span lang=\"ja\">共有キーワードです。</span></dd>   <dt class=\"term__item\">CAMPAIGN_SHARED_SET</dt>   <dd class=\"term__desc\"><span lang=\"ja\">キャンペーン共有リストです。</span></dd>   <dt class=\"term__item\">AD_CUSTOMIZER</dt>   <dd class=\"term__desc\"><span lang=\"ja\">アドカスタマイザーです。</span></dd>   <dt class=\"term__item\">EXCLUDE_AD_CUSTOMIZER</dt>   <dd class=\"term__desc\"><span lang=\"ja\">アドカスタマイザーを除くすべての履歴です。</span></dd>   <dt class=\"term__item\">ASSET</dt>   <dd class=\"term__desc\"><span lang=\"ja\">アセット（広告表示オプション）です。</span></dd>   <dt class=\"term__item\">CAMPAIGN_ASSET</dt>   <dd class=\"term__desc\"><span lang=\"ja\">キャンペーンとアセット間の設定情報です。</span></dd>   <dt class=\"term__item\">AD_GROUP_ASSET</dt>   <dd class=\"term__desc\"><span lang=\"ja\">広告グループとアセット間の設定情報です。</span></dd>   <dt class=\"term__item\">ALL</dt>   <dd class=\"term__desc\"><span lang=\"ja\">すべての履歴です。</span></dd>   <dt class=\"term__item\">UNKNOWN</dt>   <dd class=\"term__desc\"><span lang=\"ja\">未知の値です。</span></dd> </dl>

**`memberof`** AuditLogServiceEventSelector

___

### eventTypes

• `Optional` **eventTypes**: ``null`` \| [*AuditLogServiceEventTypes*](./enums/auditlogserviceeventtypes.md)[]

**`memberof`** AuditLogServiceEventSelector
