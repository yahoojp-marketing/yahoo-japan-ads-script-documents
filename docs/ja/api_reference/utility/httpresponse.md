# HTTPResponse


fetchのHTTPレスポンスデータです。

## Table of contents

### Methods

- [getContent](httpresponse.md#getcontent)
- [getContentText](httpresponse.md#getcontenttext)
- [getHeaders](httpresponse.md#getheaders)
- [getResponseCode](httpresponse.md#getresponsecode)

## Methods

### getContent

▸ **getContent**(): *Uint8Array*

フェッチ結果のバイナリデータを取得します。

**Returns:** *Uint8Array*

コンテンツのバイナリデータ

___

### getContentText

▸ **getContentText**(): *string*

フェッチ結果の文字列を取得します。

**Returns:** *string*

コンテンツの文字列(UTF-8)

▸ **getContentText**(`charset`: *string*): *string*

フェッチ結果を指定した文字コードで取得します。

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `charset` | *string* | 文字コード |

**Returns:** *string*

コンテンツの文字列

___

### getHeaders

▸ **getHeaders**(): *any*

フェッチ結果のヘッダーを取得します。

**Returns:** *any*

key/valueで構成されたjavascriptオブジェクト

___

### getResponseCode

▸ **getResponseCode**(): *number*

フェッチ結果のレスポンスコードを取得します。

**Returns:** *number*

レスポンスコード
