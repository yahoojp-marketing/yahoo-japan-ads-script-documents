# Enumeration: AdGroupAdServiceAdType


<div lang=\"ja\"> AdGroupAdServiceAdTypeは、広告タイプを表します。<br> このフィールドは、ADD時は必須となり、SET時は省略可能となります。<br> なお、選択した配信先デバイスにより、指定可能な広告の文字数は異なる場合があります。 </div>  <dl class=term>   <dt class=\"term__item\">TEXT_SHORT_AD2</dt>   <dd class=\"term__desc\"><span lang=\"ja\">「タイトル14文字、説明文19文字」のショートテキスト広告です。<br>モバイルの場合にご利用いただけます。<br>※現在、こちらの広告タイプでは入稿できません。</span><span lang=\"en\">Short text ad is &#34;title is 14 characters&#34; and &#34;description is 19 characters&#34;.<br>It is available for Mobile.<br>∗Currently this ad type is not available for ad creation.</span></dd>   <dt class=\"term__item\">RESPONSIVE_IMAGE_AD</dt>   <dd class=\"term__desc\"><span lang=\"ja\">配信される広告表示枠の形に合わせて画像のサイズ変更およびトリミングが行われるレスポンシブ広告です。</span></dd>   <dt class=\"term__item\">STATIC_FRAME_AD</dt>   <dd class=\"term__desc\"><span lang=\"ja\">配信される広告表示枠の形に合わせて3種類のレイアウトが利用可能な広告枠サイズ固定広告です。</span></dd>   <dt class=\"term__item\">BANNER_VIDEO_AD</dt>   <dd class=\"term__desc\"><span lang=\"ja\">動画で構成される広告です。</span></dd>   <dt class=\"term__item\">RESPONSIVE_VIDEO_AD</dt>   <dd class=\"term__desc\"><span lang=\"ja\">入稿内容（テキスト、動画、ボタンなど）の構成要素を組み合わせ、多様なデバイスや広告掲載面に対応したクリエイティブを表示できる広告です。</span></dd>   <dt class=\"term__item\">DYNAMIC_AD</dt>   <dd class=\"term__desc\"><span lang=\"ja\">ウェブサイトや表示するデバイスに合わせて、画像の大きさや商品の組み合わせなど、さまざまな形式で商品を表示する広告です。</span></dd>   <dt class=\"term__item\">TEXT_LONG_AD1</dt>   <dd class=\"term__desc\"><span lang=\"ja\">「タイトル15文字、説明文19文字-19文字」のテキスト広告です。PC、スマートフォン・タブレット端末の場合にご利用いただけます。（推奨）</span><span lang=\"en\">Text ad is &#34;title is 15 characters&#34; and &#34;description is 19 characters / 19 characters&#34;.<br>It is available for PC, Smartphone and Tablet. (Recommended)</span></dd>   <dt class=\"term__item\">TEXT_LONG_AD2</dt>   <dd class=\"term__desc\"><span lang=\"ja\">「タイトル15文字、説明文33文字」のテキスト広告です。<br>PC、スマートフォン・タブレット端末の場合にご利用頂けます。</span><span lang=\"en\">Text ad is &#34;title is 15 characters&#34; and &#34;description is 33 characters&#34;.<br>It is available for PC, Smartphone and Tablet.</span></dd>   <dt class=\"term__item\">TEXT_SHORT_AD1</dt>   <dd class=\"term__desc\"><span lang=\"ja\">「タイトル12文字、説明文12文字」のショートテキスト広告です。<br>モバイルの場合にご利用いただけます。<br>※現在、こちらの広告タイプでは入稿できません。</span><span lang=\"en\">Short text ad is &#34;title is 12 characters&#34; and &#34;description is 12 characters&#34;.<br>It is available for Mobile.<br>∗Currently this ad type is not available for ad creation.</span></dd>   <dt class=\"term__item\">BANNER_IMAGE_AD</dt>   <dd class=\"term__desc\"><span lang=\"ja\">画像で構成される広告です。</span></dd>   <dt class=\"term__item\">POS_AD</dt>   <dd class=\"term__desc\"><span lang=\"ja\">「説明文33文字」の掲載位置指定テキストです。</span></dd>   <dt class=\"term__item\">UNKNOWN</dt>   <dd class=\"term__desc\"><span lang=\"ja\">未知の値です。</span></dd> </dl>

## Table of contents

### Enumeration members

- [BannerImageAd](adgroupadserviceadtype.md#bannerimagead)
- [BannerVideoAd](adgroupadserviceadtype.md#bannervideoad)
- [DynamicAd](adgroupadserviceadtype.md#dynamicad)
- [PosAd](adgroupadserviceadtype.md#posad)
- [ResponsiveImageAd](adgroupadserviceadtype.md#responsiveimagead)
- [ResponsiveVideoAd](adgroupadserviceadtype.md#responsivevideoad)
- [StaticFrameAd](adgroupadserviceadtype.md#staticframead)
- [TextLongAd1](adgroupadserviceadtype.md#textlongad1)
- [TextLongAd2](adgroupadserviceadtype.md#textlongad2)
- [TextShortAd1](adgroupadserviceadtype.md#textshortad1)
- [TextShortAd2](adgroupadserviceadtype.md#textshortad2)
- [Unknown](adgroupadserviceadtype.md#unknown)

## Enumeration members

### BannerImageAd

• **BannerImageAd**: = "BANNER\_IMAGE\_AD"

___

### BannerVideoAd

• **BannerVideoAd**: = "BANNER\_VIDEO\_AD"

___

### DynamicAd

• **DynamicAd**: = "DYNAMIC\_AD"

___

### PosAd

• **PosAd**: = "POS\_AD"

___

### ResponsiveImageAd

• **ResponsiveImageAd**: = "RESPONSIVE\_IMAGE\_AD"

___

### ResponsiveVideoAd

• **ResponsiveVideoAd**: = "RESPONSIVE\_VIDEO\_AD"

___

### StaticFrameAd

• **StaticFrameAd**: = "STATIC\_FRAME\_AD"

___

### TextLongAd1

• **TextLongAd1**: = "TEXT\_LONG\_AD1"

___

### TextLongAd2

• **TextLongAd2**: = "TEXT\_LONG\_AD2"

___

### TextShortAd1

• **TextShortAd1**: = "TEXT\_SHORT\_AD1"

___

### TextShortAd2

• **TextShortAd2**: = "TEXT\_SHORT\_AD2"

___

### Unknown

• **Unknown**: = "UNKNOWN"
