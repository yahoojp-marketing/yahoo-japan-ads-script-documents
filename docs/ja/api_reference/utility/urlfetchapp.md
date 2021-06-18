# UrlFetchApp


URLへのリクエストを提供するUtilityです。

## Table of contents

### Methods

- [fetch](urlfetchapp.md#fetch)

## Methods

### fetch

▸ **fetch**(`url`: *string*): [*HTTPResponse*](httpresponse.md)

URLをフェッチします。

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `url` | *string* | 取得するURL |

**Returns:** [*HTTPResponse*](httpresponse.md)

HTTPレスポンスデータ

▸ **fetch**(`url`: *string*, `params`: [*UrlParams*](urlparams.md)): [*HTTPResponse*](httpresponse.md)

オプションの引数を使用してURLをフェッチします。

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `url` | *string* | 取得するURL |
| `params` | [*UrlParams*](urlparams.md) | オプションの引数 |

**Returns:** [*HTTPResponse*](httpresponse.md)

HTTPレスポンスデータ
