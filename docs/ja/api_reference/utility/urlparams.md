# UrlParams


UrlFetchApp.fetchのparamsに指定するオブジェクトです。

## Table of contents

### Properties

- [contentType](urlparams.md#contenttype)
- [escaping](urlparams.md#escaping)
- [followRedirects](urlparams.md#followredirects)
- [headers](urlparams.md#headers)
- [method](urlparams.md#method)
- [muteHttpExceptions](urlparams.md#mutehttpexceptions)
- [payload](urlparams.md#payload)
- [validateHttpsCertificates](urlparams.md#validatehttpscertificates)

## Properties

### contentType

• `Optional` **contentType**: *string*

コンテンツタイプです。<br>デフォルトは application/x-www-form-urlencoded となります。<br>例）'application/xml; charset=utf-8'

___

### escaping

• `Optional` **escaping**: *boolean*

リクエストURLをURLエンコードしない場合、 false を設定します。<br>デフォルトは true となります。

___

### followRedirects

• `Optional` **followRedirects**: *boolean*

リダイレクトを自動的に行わない場合、 false を設定します。<br>デフォルトは true となります。

___

### headers

• `Optional` **headers**: *any*

リクエストのHTTPヘッダーです。<br>key/valueのjavascriptオブジェクトを指定します。

___

### method

• `Optional` **method**: ``"GET"`` \| ``"POST"`` \| ``"PUT"`` \| ``"DELETE"`` \| ``"PATCH"``

リクエストのHTTPメソッドです。<br>値は GET/POST/PUT/DELETE/PATCH のいずれかとなります。<br>デフォルトは GET となります。

___

### muteHttpExceptions

• `Optional` **muteHttpExceptions**: *boolean*

HTTPレスポンスコードがエラーの場合でも例外をスローされたくない場合、 true を設定します。<br>デフォルトは false となります。

___

### payload

• `Optional` **payload**: *any*

リクエストボディに設定するデータです。<br>文字列/key,valueのjavascriptオブジェクト/Uint8Arrayを指定することができます。

___

### validateHttpsCertificates

• `Optional` **validateHttpsCertificates**: *boolean*

無効な証明書を無視する場合、 false を設定します。<br>デフォルトは true となります。
