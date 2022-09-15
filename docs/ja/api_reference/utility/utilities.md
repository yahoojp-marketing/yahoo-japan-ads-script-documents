# Utilities


様々な操作を提供するUtilityです。

## Table of contents

### Methods

- [base64Decode](utilities.md#base64decode)
- [base64Encode](utilities.md#base64encode)
- [formatDate](utilities.md#formatdate)
- [newBlob](utilities.md#newblob)
- [sleep](utilities.md#sleep)

## Methods

### base64Decode

▸ **base64Decode**(`encoded`: *string*): *Uint8Array*

Base64でエンコードされた文字列をバイナリにデコードします。

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `encoded` | *string* | Base64でエンコードされた文字列 |

**Returns:** *Uint8Array*

デコードバイナリ

___

### base64Encode

▸ **base64Encode**(`data`: *Uint8Array*): *string*

指定されたバイナリをBase64でエンコードします。

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `data` | *Uint8Array* | エンコードするバイナリデータ |

**Returns:** *string*

Base64でエンコードされた文字列

▸ **base64Encode**(`data`: *string*): *string*

指定された文字列をBase64でエンコードします。

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `data` | *string* | エンコードする文字列 |

**Returns:** *string*

Base64でエンコードされた文字列

___

### formatDate

▸ **formatDate**(`date`: Date, `timeZone`: *string*, `format`: *string*): *string*

指定された日付を文字列にフォーマット

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `date` | Date | 文字列としてフォーマットする日付 |
| `timeZone` | *string* | 結果の出力タイムゾーン |
| `format` | *string* | Javaの<a href="http://docs.oracle.com/javase/7/docs/api/java/text/SimpleDateFormat.html">SimpleDateFormat</a>に準じたフォーマット指定文字列 |

**Returns:** *string*

フォーマットされた日付文字列

___

### newBlob

▸ **newBlob**(`data`: *Uint8Array*): [*Blob*](blob.md)

バイナリデータから新しいBlobオブジェクトを作成します。<br>Blobは、Google Driveファイルの操作で利用するオブジェクトとなります。

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `data` | *Uint8Array* | バイナリデータ |

**Returns:** [*Blob*](blob.md)

Blobオブジェクト

▸ **newBlob**(`data`: *Uint8Array*, `contentType`: *string*): [*Blob*](blob.md)

バイナリデータと指定されたコンテンツタイプから新しいBlobオブジェクトを作成します。<br>Blobは、Google Driveファイルの操作で利用するオブジェクトとなります。

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `data` | *Uint8Array* | バイナリデータ |
| `contentType` | *string* | Blobのコンテンツタイプ |

**Returns:** [*Blob*](blob.md)

Blobオブジェクト

▸ **newBlob**(`data`: *Uint8Array*, `contentType`: *string*, `name`: *string*): [*Blob*](blob.md)

バイナリデータと指定されたコンテンツタイプ及び名前から新しいBlobオブジェクトを作成します。<br>Blobは、Google Driveファイルの操作で利用するオブジェクトとなります。

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `data` | *Uint8Array* | バイナリデータ |
| `contentType` | *string* | Blobのコンテンツタイプ |
| `name` | *string* | Blobの名前 |

**Returns:** [*Blob*](blob.md)

Blobオブジェクト

▸ **newBlob**(`data`: *string*): [*Blob*](blob.md)

文字列から新しいBlobオブジェクトを作成します。<br>Blobは、Google Driveファイルの操作で利用するオブジェクトとなります。

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `data` | *string* | Blobにする文字列(UTF-8を想定しています) |

**Returns:** [*Blob*](blob.md)

Blobオブジェクト

▸ **newBlob**(`data`: *string*, `contentType`: *string*): [*Blob*](blob.md)

文字列と指定されたコンテンツタイプから新しいBlobオブジェクトを作成します。<br>Blobは、Google Driveファイルの操作で利用するオブジェクトとなります。

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `data` | *string* | Blobにする文字列(UTF-8を想定しています) |
| `contentType` | *string* | Blobのコンテンツタイプ |

**Returns:** [*Blob*](blob.md)

Blobオブジェクト

▸ **newBlob**(`data`: *string*, `contentType`: *string*, `name`: *string*): [*Blob*](blob.md)

文字列と指定されたコンテンツタイプ及び名前から新しいBlobオブジェクトを作成します。<br>Blobは、Google Driveファイルの操作で利用するオブジェクトとなります。

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `data` | *string* | Blobにする文字列(UTF-8を想定しています) |
| `contentType` | *string* | Blobのコンテンツタイプ |
| `name` | *string* | Blobの名前 |

**Returns:** [*Blob*](blob.md)

Blobオブジェクト

___

### sleep

▸ **sleep**(`ms`: *number*): *void*

指定された時間スリープします。

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `ms` | *number* | スリープする時間（単位：ミリ秒） |

**Returns:** *void*
