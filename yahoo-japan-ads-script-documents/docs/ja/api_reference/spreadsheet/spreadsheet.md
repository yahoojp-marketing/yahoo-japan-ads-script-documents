# Spreadsheet


スプレッドシートへの操作を提供するクラスです。

## Table of contents

### Methods

- [copy](spreadsheet.md#copy)
- [getId](spreadsheet.md#getid)
- [getName](spreadsheet.md#getname)
- [getRange](spreadsheet.md#getrange)
- [getRangeByName](spreadsheet.md#getrangebyname)
- [getRangeList](spreadsheet.md#getrangelist)
- [getSheetByName](spreadsheet.md#getsheetbyname)
- [getSheets](spreadsheet.md#getsheets)
- [getUrl](spreadsheet.md#geturl)
- [insertSheet](spreadsheet.md#insertsheet)
- [rename](spreadsheet.md#rename)

## Methods

### copy

▸ **copy**(`name`: *string*): [*Spreadsheet*](spreadsheet.md)

スプレッドシートをコピーして、新しいスプレッドシートを返します。

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `name` | *string* | 新しいスプレッドシートの名前 |

**Returns:** [*Spreadsheet*](spreadsheet.md)

新しいスプレッドシートオブジェクト

___

### getId

▸ **getId**(): *string*

スプレッドシートのIDを返します。

**Returns:** *string*

スプレッドシートのID

___

### getName

▸ **getName**(): *string*

スプレッドシートの名前を返します。

**Returns:** *string*

スプレッドシートの名前

___

### getRange

▸ **getRange**(`a1Notation`: *string*): [*Range*](range.md)

A1表記またはR1C1表記で指定されたレンジオブジェクトを返します。

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `a1Notation` | *string* | A1表記またはR1C1表記で指定されたレンジ。 |

**Returns:** [*Range*](range.md)

指定された範囲のレンジオブジェクト

___

### getRangeByName

▸ **getRangeByName**(`name`: *string*): ``null`` \| [*Range*](range.md)

名前付きの範囲を返すか、指定された名前の範囲が見つからない場合はnullを返します。

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `name` | *string* | 取得する範囲の名前 |

**Returns:** ``null`` \| [*Range*](range.md)

指定された名前付き範囲のレンジオブジェクト

___

### getRangeList

▸ **getRangeList**(`a1Notations`: *string*[]): [*RangeList*](rangelist.md)

A1表記またはR1C1表記で指定された複数のレンジオブジェクトを返します。

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `a1Notations` | *string*[] | A1表記またはR1C1表記で指定されたレンジの配列。 |

**Returns:** [*RangeList*](rangelist.md)

指定された範囲のレンジリストオブジェクト

___

### getSheetByName

▸ **getSheetByName**(`name`: *string*): ``null`` \| [*Sheet*](sheet.md)

指定された名前のシートを返します。<br>同じ名前のシートが複数ある場合は、一番左のシートを返します。<br>指定された名前のシートがない場合、nullを返します。

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `name` | *string* | 取得するシートの名前 |

**Returns:** ``null`` \| [*Sheet*](sheet.md)

指定された名前のシートオブジェクト

___

### getSheets

▸ **getSheets**(): [*Sheet*](sheet.md)[]

スプレッドシート内のすべてのシートを返します。

**Returns:** [*Sheet*](sheet.md)[]

スプレッドシート内のすべてのシートの配列

___

### getUrl

▸ **getUrl**(): *string*

スプレッドシートのURLを返します。

**Returns:** *string*

スプレッドシートのURL

___

### insertSheet

▸ **insertSheet**(): [*Sheet*](sheet.md)

デフォルトのシート名を使用して、スプレッドシートに新しいシートを挿入します。

**Returns:** [*Sheet*](sheet.md)

新しいシートオブジェクト

▸ **insertSheet**(`sheetIndex`: *number*): [*Sheet*](sheet.md)

スプレッドシートの指定されたインデックスに新しいシートを挿入します。

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `sheetIndex` | *number* | 新しく作成するシートのインデックス。<br>スプレッドシートの最初のシートとしてシートを挿入するには、 0 に設定します。 |

**Returns:** [*Sheet*](sheet.md)

新しいシートオブジェクト

▸ **insertSheet**(`sheetIndex`: *number*, `options`: [*InsertSheetOptions*](insertsheetoptions.md)): [*Sheet*](sheet.md)

スプレッドシートの指定されたインデックスに新しいシートを挿入し、オプションの引数を使用します。

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `sheetIndex` | *number* | 新しく作成するシートのインデックス。<br>スプレッドシートの最初のシートとしてシートを挿入するには、 0 に設定します。 |
| `options` | [*InsertSheetOptions*](insertsheetoptions.md) | オプションの引数 |

**Returns:** [*Sheet*](sheet.md)

新しいシートオブジェクト

▸ **insertSheet**(`options`: [*InsertSheetOptions*](insertsheetoptions.md)): [*Sheet*](sheet.md)

デフォルトのシート名とオプションの引数を使用して、スプレッドシートに新しいシートを挿入します。

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `options` | [*InsertSheetOptions*](insertsheetoptions.md) | オプションの引数 |

**Returns:** [*Sheet*](sheet.md)

新しいシートオブジェクト

▸ **insertSheet**(`sheetName`: *string*): [*Sheet*](sheet.md)

スプレッドシートに指定された名前の新しいシートを挿入します。

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `sheetName` | *string* | 新しいシートの名前 |

**Returns:** [*Sheet*](sheet.md)

新しいシートオブジェクト

▸ **insertSheet**(`sheetName`: *string*, `sheetIndex`: *number*): [*Sheet*](sheet.md)

指定されたインデックスの指定された名前でスプレッドシートに新しいシートを挿入します。

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `sheetName` | *string* | 新しいシートの名前 |
| `sheetIndex` | *number* | 新しく作成するシートのインデックス。<br>スプレッドシートの最初のシートとしてシートを挿入するには、0に設定します。 |

**Returns:** [*Sheet*](sheet.md)

新しいシートオブジェクト

▸ **insertSheet**(`sheetName`: *string*, `sheetIndex`: *number*, `options`: [*InsertSheetOptions*](insertsheetoptions.md)): [*Sheet*](sheet.md)

指定されたインデックスの指定された名前でスプレッドシートに新しいシートを挿入し、オプションの引数を使用します。

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `sheetName` | *string* | 新しいシートの名前 |
| `sheetIndex` | *number* | 新しく作成するシートのインデックス。<br>スプレッドシートの最初のシートとしてシートを挿入するには、0に設定します。 |
| `options` | [*InsertSheetOptions*](insertsheetoptions.md) | オプションの引数 |

**Returns:** [*Sheet*](sheet.md)

新しいシートオブジェクト

▸ **insertSheet**(`sheetName`: *string*, `options`: [*InsertSheetOptions*](insertsheetoptions.md)): [*Sheet*](sheet.md)

指定された名前でスプレッドシートに新しいシートを挿入し、オプションの引数を使用します。

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `sheetName` | *string* | 新しいシートの名前 |
| `options` | [*InsertSheetOptions*](insertsheetoptions.md) | オプションの引数 |

**Returns:** [*Sheet*](sheet.md)

新しいシートオブジェクト

___

### rename

▸ **rename**(`newName`: *string*): *void*

スプレッドシートの名前を変更します。

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `newName` | *string* | スプレッドシートの新しい名前 |

**Returns:** *void*
