# Blob


バイナリ情報を表すクラスです。

## Table of contents

### Methods

- [getBytes](blob.md#getbytes)
- [getContentType](blob.md#getcontenttype)
- [getName](blob.md#getname)
- [setBytes](blob.md#setbytes)
- [setContentType](blob.md#setcontenttype)
- [setName](blob.md#setname)

## Methods

### getBytes

▸ **getBytes**(): *Uint8Array*

Blobのバイナリデータを取得します。

**Returns:** *Uint8Array*

バイナリデータ

___

### getContentType

▸ **getContentType**(): *string*

Blobのコンテンツタイプを取得します。

**Returns:** *string*

コンテンツタイプ

___

### getName

▸ **getName**(): *string*

Blob名を取得します。

**Returns:** *string*

Blob名

___

### setBytes

▸ **setBytes**(`bytes`: *Uint8Array*): [*Blob*](blob.md)

Blobにバイナリデータを設定します。

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `bytes` | *Uint8Array* | バイナリデータ |

**Returns:** [*Blob*](blob.md)

Blob

___

### setContentType

▸ **setContentType**(`contentType`: *string*): [*Blob*](blob.md)

Blobにコンテンツタイプを設定します。

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `contentType` | *string* | コンテンツタイプ |

**Returns:** [*Blob*](blob.md)

Blob

___

### setName

▸ **setName**(`name`: *string*): [*Blob*](blob.md)

Blob名を設定します。

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `name` | *string* | Blob名 |

**Returns:** [*Blob*](blob.md)

Blob
