# Folder


Google Driveのフォルダを表すクラスです。

## Table of contents

### Methods

- [createFile](folder.md#createfile)
- [createFolder](folder.md#createfolder)
- [getFiles](folder.md#getfiles)
- [getFilesByName](folder.md#getfilesbyname)
- [getFilesByType](folder.md#getfilesbytype)
- [getFolders](folder.md#getfolders)
- [getFoldersByName](folder.md#getfoldersbyname)
- [getId](folder.md#getid)
- [getName](folder.md#getname)

## Methods

### createFile

▸ **createFile**(`blob`: [*Blob*](../utility/blob.md)): [*File*](file.md)

指定されたBlobでGoogle Driveのフォルダ配下に新しいファイルを作成します。

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `blob` | [*Blob*](../utility/blob.md) | Blobデータ |

**Returns:** [*File*](file.md)

新しく作成されたファイル

▸ **createFile**(`name`: *string*, `content`: *string*): [*File*](file.md)

指定された名前とコンテンツでGoogle Driveのフォルダ配下に新しいファイルを作成します。

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `name` | *string* | ファイル名 |
| `content` | *string* | ファイルのコンテンツ |

**Returns:** [*File*](file.md)

新しく作成されたファイル

▸ **createFile**(`name`: *string*, `content`: *string*, `mimeType`: *string*): [*File*](file.md)

指定された名前とコンテンツとMIMEタイプでGoogle Driveのフォルダ配下に新しいファイルを作成します。

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `name` | *string* | ファイル名 |
| `content` | *string* | ファイルのコンテンツ |
| `mimeType` | *string* | ファイルのMIMEタイプ |

**Returns:** [*File*](file.md)

新しく作成されたファイル

___

### createFolder

▸ **createFolder**(`name`: *string*): [*Folder*](folder.md)

指定された名前でGoogle Driveのフォルダ配下に新しいフォルダを作成します。

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `name` | *string* | フォルダ |

**Returns:** [*Folder*](folder.md)

新しく作成されたフォルダ

___

### getFiles

▸ **getFiles**(): [*FileIterator*](fileiterator.md)

Google Driveのフォルダ内の全てのファイルを取得します。

**Returns:** [*FileIterator*](fileiterator.md)

ファイルのコレクション

___

### getFilesByName

▸ **getFilesByName**(`name`: *string*): [*FileIterator*](fileiterator.md)

指定されたファイル名でGoogle Driveのフォルダ内のファイルを取得します。

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `name` | *string* | ファイル名 |

**Returns:** [*FileIterator*](fileiterator.md)

指定されたファイル名のファイルコレクション

___

### getFilesByType

▸ **getFilesByType**(`mimeType`: *string*): [*FileIterator*](fileiterator.md)

指定されたMIMEタイプでGoogle Driveのフォルダ内のファイルを取得します。

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `mimeType` | *string* | MIMEタイプ |

**Returns:** [*FileIterator*](fileiterator.md)

指定されたMIMEタイプのファイルコレクション

___

### getFolders

▸ **getFolders**(): [*FolderIterator*](folderiterator.md)

Google Driveのフォルダ内の全てのフォルダを取得します。

**Returns:** [*FolderIterator*](folderiterator.md)

フォルダのコレクション

___

### getFoldersByName

▸ **getFoldersByName**(`name`: *string*): [*FolderIterator*](folderiterator.md)

指定されたフォルダ名でGoogle Driveのフォルダ内のフォルダを取得します。

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `name` | *string* | フォルダ名 |

**Returns:** [*FolderIterator*](folderiterator.md)

指定されたフォルダ名のフォルダコレクション

___

### getId

▸ **getId**(): *undefined* \| ``null`` \| *string*

フォルダのIDを取得します。

**Returns:** *undefined* \| ``null`` \| *string*

フォルダID

___

### getName

▸ **getName**(): *undefined* \| ``null`` \| *string*

フォルダ名を取得します。

**Returns:** *undefined* \| ``null`` \| *string*

フォルダ名
