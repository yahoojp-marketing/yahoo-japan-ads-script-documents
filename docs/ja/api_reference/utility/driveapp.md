# DriveApp


Google Driveへの操作を提供するUtilityです。

## Table of contents

### Methods

- [createFile](driveapp.md#createfile)
- [createFolder](driveapp.md#createfolder)
- [getFileById](driveapp.md#getfilebyid)
- [getFiles](driveapp.md#getfiles)
- [getFilesByName](driveapp.md#getfilesbyname)
- [getFilesByType](driveapp.md#getfilesbytype)
- [getFolderById](driveapp.md#getfolderbyid)
- [getFolders](driveapp.md#getfolders)
- [getFoldersByName](driveapp.md#getfoldersbyname)
- [getRootFolder](driveapp.md#getrootfolder)

## Methods

### createFile

▸ **createFile**(`blob`: [*Blob*](../utility/blob.md)): [*File*](../google_drive/file.md)

指定されたBlobでGoogle Driveのルートにファイルを作成します。

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `blob` | [*Blob*](../utility/blob.md) | Blobデータ |

**Returns:** [*File*](../google_drive/file.md)

新しく作成されたファイル

▸ **createFile**(`name`: *string*, `content`: *string*): [*File*](../google_drive/file.md)

指定された名前とコンテンツでGoogle Driveのルートにファイルを作成します。

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `name` | *string* | ファイル名 |
| `content` | *string* | ファイルのコンテンツ |

**Returns:** [*File*](../google_drive/file.md)

新しく作成されたファイル

▸ **createFile**(`name`: *string*, `content`: *string*, `mimeType`: *string*): [*File*](../google_drive/file.md)

指定された名前とコンテンツとMIMEタイプでGoogle Driveのルートにファイルを作成します。

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `name` | *string* | ファイル名 |
| `content` | *string* | ファイルのコンテンツ |
| `mimeType` | *string* | ファイルのMIMEタイプ |

**Returns:** [*File*](../google_drive/file.md)

新しく作成されたファイル

___

### createFolder

▸ **createFolder**(`name`: *string*): [*Folder*](../google_drive/folder.md)

指定された名前でGoogle Driveのルートにフォルダを作成します。

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `name` | *string* | フォルダ |

**Returns:** [*Folder*](../google_drive/folder.md)

新しく作成されたフォルダ

___

### getFileById

▸ **getFileById**(`id`: *string*): [*File*](../google_drive/file.md)

指定されたIDでGoogle Driveのファイルを取得します。

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `id` | *string* | ファイルID |

**Returns:** [*File*](../google_drive/file.md)

指定されたIDのファイル

___

### getFiles

▸ **getFiles**(): [*FileIterator*](../google_drive/fileiterator.md)

Google Driveの全てのファイルを取得します。

**Returns:** [*FileIterator*](../google_drive/fileiterator.md)

ファイルのコレクション

___

### getFilesByName

▸ **getFilesByName**(`name`: *string*): [*FileIterator*](../google_drive/fileiterator.md)

指定されたファイル名でGoogle Driveのファイルを取得します。

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `name` | *string* | ファイル名 |

**Returns:** [*FileIterator*](../google_drive/fileiterator.md)

指定されたファイル名のファイルコレクション

___

### getFilesByType

▸ **getFilesByType**(`mimeType`: *string*): [*FileIterator*](../google_drive/fileiterator.md)

指定されたMIMEタイプでGoogle Driveのファイルを取得します。

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `mimeType` | *string* | MIMEタイプ |

**Returns:** [*FileIterator*](../google_drive/fileiterator.md)

指定されたMIMEタイプのファイルコレクション

___

### getFolderById

▸ **getFolderById**(`id`: *string*): [*Folder*](../google_drive/folder.md)

指定されたIDでGoogle Driveのフォルダを取得します。

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `id` | *string* | フォルダID |

**Returns:** [*Folder*](../google_drive/folder.md)

指定されたIDのフォルダ

___

### getFolders

▸ **getFolders**(): [*FolderIterator*](../google_drive/folderiterator.md)

Google Driveの全てのフォルダを取得します。

**Returns:** [*FolderIterator*](../google_drive/folderiterator.md)

フォルダのコレクション

___

### getFoldersByName

▸ **getFoldersByName**(`name`: *string*): [*FolderIterator*](../google_drive/folderiterator.md)

指定されたフォルダ名でGoogle Driveのフォルダを取得します。

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `name` | *string* | フォルダ名 |

**Returns:** [*FolderIterator*](../google_drive/folderiterator.md)

指定されたフォルダ名のフォルダコレクション

___

### getRootFolder

▸ **getRootFolder**(): [*Folder*](../google_drive/folder.md)

Google Driveのルートフォルダを取得します。

**Returns:** [*Folder*](../google_drive/folder.md)

ルートフォルダ
