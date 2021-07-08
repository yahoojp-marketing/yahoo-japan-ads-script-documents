# Sheet


スプレッドシートのシートへの操作を提供するクラスです。

## Table of contents

### Methods

- [appendRow](sheet.md#appendrow)
- [clear](sheet.md#clear)
- [getDataRange](sheet.md#getdatarange)
- [getIndex](sheet.md#getindex)
- [getLastColumn](sheet.md#getlastcolumn)
- [getLastRow](sheet.md#getlastrow)
- [getMaxColumns](sheet.md#getmaxcolumns)
- [getMaxRows](sheet.md#getmaxrows)
- [getName](sheet.md#getname)
- [getRange](sheet.md#getrange)
- [getRangeList](sheet.md#getrangelist)
- [getSheetId](sheet.md#getsheetid)
- [getSheetName](sheet.md#getsheetname)
- [getSheetValues](sheet.md#getsheetvalues)
- [insertColumnAfter](sheet.md#insertcolumnafter)
- [insertColumnBefore](sheet.md#insertcolumnbefore)
- [insertColumns](sheet.md#insertcolumns)
- [insertColumnsAfter](sheet.md#insertcolumnsafter)
- [insertColumnsBefore](sheet.md#insertcolumnsbefore)
- [insertRowAfter](sheet.md#insertrowafter)
- [insertRowBefore](sheet.md#insertrowbefore)
- [insertRows](sheet.md#insertrows)
- [insertRowsAfter](sheet.md#insertrowsafter)
- [insertRowsBefore](sheet.md#insertrowsbefore)
- [setName](sheet.md#setname)

## Methods

### appendRow

▸ **appendRow**(`rowContents`: *any*[]): [*Sheet*](sheet.md)

シートに指定された値で1行書き込みます。<br>値のある最後の行の次の行に対して書き込みを行います。

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `rowContents` | *any*[] | 後に挿入する値の配列 |

**Returns:** [*Sheet*](sheet.md)

このシートオブジェクト

___

### clear

▸ **clear**(): [*Sheet*](sheet.md)

このシートオブジェクトのセルの値、フォーマットをクリアします。

**Returns:** [*Sheet*](sheet.md)

このシートオブジェクト

▸ **clear**(`options`: [*SheetClearOptions*](sheetclearoptions.md)): [*Sheet*](sheet.md)

このシートオブジェクトのセルの値/フォーマットを指定されたオプションでクリアします。

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `options` | [*SheetClearOptions*](sheetclearoptions.md) | オプションの引数 |

**Returns:** [*Sheet*](sheet.md)

このシートオブジェクト

___

### getDataRange

▸ **getDataRange**(): [*Range*](range.md)

データが存在する範囲に対応するレンジオブジェクトを返却します。<br>A1からSheet.getLastColumn(), Sheet.getLastRow()で囲まれた範囲と同義となります。

**Returns:** [*Range*](range.md)

指定された範囲のレンジオブジェクト

___

### getIndex

▸ **getIndex**(): *number*

スプレッドシート内のシートの位置を取得します。<br>0 から始まります。

**Returns:** *number*

スプレッドシートでのシートの位置

___

### getLastColumn

▸ **getLastColumn**(): *number*

値のある最後の列の位置を返します。

**Returns:** *number*

値を含むシートの最後の列

___

### getLastRow

▸ **getLastRow**(): *number*

値のある最後の行の位置を返します。

**Returns:** *number*

値を含むシートの最後の行

___

### getMaxColumns

▸ **getMaxColumns**(): *number*

値に関係なく、シート内の現在の列数を返します。

**Returns:** *number*

シートの最大列数

___

### getMaxRows

▸ **getMaxRows**(): *number*

値に関係なく、シート内の現在の行数を返します。

**Returns:** *number*

シートの最大行数

___

### getName

▸ **getName**(): *string*

シートの名前を返します。

**Returns:** *string*

シートの名前

___

### getRange

▸ **getRange**(`row`: *number*, `column`: *number*, `numRows`: *number*, `numColumns`: *number*): [*Range*](range.md)

指定された行と列、行数と列数のレンジオブジェクトを返します。

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `row` | *number* | 範囲の開始行インデックス。<br>行のインデックス付けは 1 から始まります。 |
| `column` | *number* | 範囲の開始列インデックス。<br>列のインデックス付けは 1 から始まります。 |
| `numRows` | *number* | 範囲の行数 |
| `numColumns` | *number* | 範囲の列数 |

**Returns:** [*Range*](range.md)

指定された範囲のレンジオブジェクト

▸ **getRange**(`row`: *number*, `column`: *number*, `numRows`: *number*): [*Range*](range.md)

指定された行と列、行数のレンジオブジェクトを返します。<br>列数は1となります。

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `row` | *number* | 範囲の開始行インデックス。<br>行のインデックス付けは 1 から始まります。 |
| `column` | *number* | 範囲の開始列インデックス。<br>列のインデックス付けは 1 から始まります。 |
| `numRows` | *number* | 範囲の行数 |

**Returns:** [*Range*](range.md)

指定された範囲のレンジオブジェクト

▸ **getRange**(`row`: *number*, `column`: *number*): [*Range*](range.md)

指定された行と列の単一のレンジオブジェクトを返します。

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `row` | *number* | 範囲の開始行インデックス。<br>行のインデックス付けは 1 から始まります。 |
| `column` | *number* | 範囲の開始列インデックス。<br>列のインデックス付けは 1 から始まります。 |

**Returns:** [*Range*](range.md)

指定された範囲のレンジオブジェクト

▸ **getRange**(`a1Notation`: *string*): [*Range*](range.md)

A1表記またはR1C1表記で指定されたレンジオブジェクトを返します。

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `a1Notation` | *string* | A1表記またはR1C1表記で指定されたレンジ。 |

**Returns:** [*Range*](range.md)

指定された範囲のレンジオブジェクト

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

### getSheetId

▸ **getSheetId**(): *number*

シートのIDを返します。

**Returns:** *number*

シートのID

___

### getSheetName

▸ **getSheetName**(): *string*

シート名を返します。

**Returns:** *string*

シートの名前

___

### getSheetValues

▸ **getSheetValues**(`startRow`: *number*, `startColumn`: *number*, `numRows`: *number*, `numColumns`: *number*): *any*[][]

指定された行と列、行数と列数の範囲のセルの値を返します。

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `startRow` | *number* | - |
| `startColumn` | *number* | - |
| `numRows` | *number* | 範囲の行数 |
| `numColumns` | *number* | 範囲の列数 |

**Returns:** *any*[][]

セルの値の2次元配列

___

### insertColumnAfter

▸ **insertColumnAfter**(`afterPosition`: *number*): [*Sheet*](sheet.md)

指定された列位置の後に列を挿入します。

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `afterPosition` | *number* | 新しい列を追加する必要がある列位置 |

**Returns:** [*Sheet*](sheet.md)

このシートオブジェクト

___

### insertColumnBefore

▸ **insertColumnBefore**(`beforePosition`: *number*): [*Sheet*](sheet.md)

指定された列位置の前に列を挿入します。

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `beforePosition` | *number* | 新しい列を追加する必要がある列位置 |

**Returns:** [*Sheet*](sheet.md)

このシートオブジェクト

___

### insertColumns

▸ **insertColumns**(`columnIndex`: *number*): *void*

シートの指定された位置に列を挿入します。

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `columnIndex` | *number* | 列を挿入する場所を示すインデックス |

**Returns:** *void*

▸ **insertColumns**(`columnIndex`: *number*, `numColumns`: *number*): *void*

シートの指定された位置に複数の列を挿入します。

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `columnIndex` | *number* | 列を挿入する場所を示すインデックス |
| `numColumns` | *number* | 挿入する列の数 |

**Returns:** *void*

___

### insertColumnsAfter

▸ **insertColumnsAfter**(`afterPosition`: *number*, `howMany`: *number*): [*Sheet*](sheet.md)

指定された列位置の後に複数の列を挿入します。

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `afterPosition` | *number* | 新しい列を追加する必要がある列位置 |
| `howMany` | *number* | 挿入する列の数 |

**Returns:** [*Sheet*](sheet.md)

このシートオブジェクト

___

### insertColumnsBefore

▸ **insertColumnsBefore**(`beforePosition`: *number*, `howMany`: *number*): [*Sheet*](sheet.md)

指定された列位置の前に複数の列を挿入します。

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `beforePosition` | *number* | 新しい列を追加する必要がある列位置 |
| `howMany` | *number* | 挿入する列の数 |

**Returns:** [*Sheet*](sheet.md)

このシートオブジェクト

___

### insertRowAfter

▸ **insertRowAfter**(`afterPosition`: *number*): [*Sheet*](sheet.md)

指定された行位置の後に行を挿入します。

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `afterPosition` | *number* | 新しい行を追加する必要がある行位置 |

**Returns:** [*Sheet*](sheet.md)

このシートオブジェクト

___

### insertRowBefore

▸ **insertRowBefore**(`beforePosition`: *number*): [*Sheet*](sheet.md)

指定された行位置の前に行を挿入します。

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `beforePosition` | *number* | 新しい行を追加する必要がある行位置 |

**Returns:** [*Sheet*](sheet.md)

このシートオブジェクト

___

### insertRows

▸ **insertRows**(`rowIndex`: *number*): *void*

シートの指定された位置に行を挿入します。

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `rowIndex` | *number* | 行を挿入する場所を示すインデックス |

**Returns:** *void*

▸ **insertRows**(`rowIndex`: *number*, `numRows`: *number*): *void*

シートの指定された位置に複数の行を挿入します。

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `rowIndex` | *number* | 行を挿入する場所を示すインデックス |
| `numRows` | *number* | - |

**Returns:** *void*

___

### insertRowsAfter

▸ **insertRowsAfter**(`afterPosition`: *number*, `howMany`: *number*): [*Sheet*](sheet.md)

指定された行位置の後に複数の行を挿入します。

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `afterPosition` | *number* | 新しい行を追加する必要がある行位置 |
| `howMany` | *number* | 挿入する行の数 |

**Returns:** [*Sheet*](sheet.md)

このシートオブジェクト

___

### insertRowsBefore

▸ **insertRowsBefore**(`beforePosition`: *number*, `howMany`: *number*): [*Sheet*](sheet.md)

指定された行位置の前に複数の行を挿入します。

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `beforePosition` | *number* | 新しい行を追加する必要がある行位置 |
| `howMany` | *number* | 挿入する行の数 |

**Returns:** [*Sheet*](sheet.md)

このシートオブジェクト

___

### setName

▸ **setName**(`name`: *string*): [*Sheet*](sheet.md)

シート名を設定します。

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `name` | *string* | シートの新しい名前 |

**Returns:** [*Sheet*](sheet.md)

このシートオブジェクト
