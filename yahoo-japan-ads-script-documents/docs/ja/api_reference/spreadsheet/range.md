# Range


スプレッドシートのセル範囲への操作を提供するクラスです。

## Table of contents

### Methods

- [clear](range.md#clear)
- [getValues](range.md#getvalues)
- [setValues](range.md#setvalues)

## Methods

### clear

▸ **clear**(): [*Range*](range.md)

このレンジオブジェクトが示す範囲のセルの値、フォーマット、データ検証ルールをクリアします。

**Returns:** [*Range*](range.md)

このレンジオブジェクト

___

### getValues

▸ **getValues**(): *any*[][]

このレンジオブジェクトが示す範囲のセルの値を返します。<br>配列は1次元目が行を表し、2次元めが列を表します。

**Returns:** *any*[][]

セルの値の2次元配列

___

### setValues

▸ **setValues**(`values`: *any*[][]): [*Range*](range.md)

このレンジオブジェクトが示す範囲のセルに値を書き込みます。

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `values` | *any*[][] | 書き込む値の2次元配列 |

**Returns:** [*Range*](range.md)

このレンジオブジェクト
