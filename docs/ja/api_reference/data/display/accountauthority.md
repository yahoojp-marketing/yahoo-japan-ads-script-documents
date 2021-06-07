# AccountAuthority


<div lang=\"ja\">AccountAuthorityオブジェクトは、アカウント権限情報を示します。<br> authoritiesで返却される値は、以下のとおりです。   <table border=\'1\'>     <tr>       <th>accountAuthorities</th>       <th>説明</th>       <th>権限種別</th>     </tr>     <tr>       <td>WEBSITE_TRAFFIC</td>       <td>運用型：サイト誘導</td>       <td>キャンペーン目的</td>     </tr>     <tr>       <td>VIDEO_VIEW</td>       <td>運用型：動画再生</td>       <td>キャンペーン目的</td>     </tr>     <tr>       <td>APP_PROMOTION</td>       <td>運用型：アプリ訴求</td>       <td>キャンペーン目的</td>     </tr>     <tr>       <td>CONVERSION</td>       <td>運用型：コンバージョン</td>       <td>キャンペーン目的</td>     </tr>     <tr>       <td>ITEM_LIST</td>       <td>運用型：商品リスト訴求</td>       <td>キャンペーン目的</td>     </tr>     <tr>       <td>BRAND_AWARENESS</td>       <td>運用型：ブランド認知</td>       <td>キャンペーン目的</td>     </tr>     <tr>       <td>BRAND_AWARENESS_GUARANTEED</td>       <td>予約型：ブランド認知</td>       <td>キャンペーン目的</td>     </tr>     <tr>       <td>SHOPPING_ADS</td>       <td>eコマース</td>       <td>キャンペーン掲載タイプ</td>     </tr>   </table> それぞれのキャンペーン目的の詳細については、<a href=\"https://ads-help.yahoo.co.jp/yahooads/display/articledetail?lan=ja&aid=51512\">目的別キャンペーン作成について</a>をご確認ください。 </div> 

## Table of contents

### Properties

- [accountId](accountauthority.md#accountid)
- [authorities](accountauthority.md#authorities)

## Properties

### accountId

• `Optional` **accountId**: ``null`` \| *number*

<div lang=\"ja\">アカウントIDです。</div> 

**`memberof`** AccountAuthority

___

### authorities

• `Optional` **authorities**: ``null`` \| *string*[]

<div lang=\"ja\">アカウント権限です。</div> 

**`memberof`** AccountAuthority
