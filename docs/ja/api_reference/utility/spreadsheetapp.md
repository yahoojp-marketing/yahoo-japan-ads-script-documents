# SpreadsheetApp


スプレッドシートへの操作を提供するUtilityです。

## Table of contents

### Methods

- [create](spreadsheetapp.md#create)
- [openById](spreadsheetapp.md#openbyid)
- [openByUrl](spreadsheetapp.md#openbyurl)

## Methods

### create

▸ **create**(`name`: *string*): [*Spreadsheet*](../spreadsheet/spreadsheet.md)

指定された名前で新しいスプレッドシートを作成します。

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `name` | *string* | スプレッドシートの名前 |

**Returns:** [*Spreadsheet*](../spreadsheet/spreadsheet.md)

新しいスプレッドシートのオブジェクト

___

### openById

▸ **openById**(`id`: *string*): [*Spreadsheet*](../spreadsheet/spreadsheet.md)

指定されたIDでスプレッドシートを開きます。

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `id` | *string* | スプレッドシートのID |

**Returns:** [*Spreadsheet*](../spreadsheet/spreadsheet.md)

新しいスプレッドシートのオブジェクト

___

### openByUrl

▸ **openByUrl**(`url`: *string*): [*Spreadsheet*](../spreadsheet/spreadsheet.md)

指定されたURLでスプレッドシートを開きます。

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `url` | *string* | スプレッドシートのURL |

**Returns:** [*Spreadsheet*](../spreadsheet/spreadsheet.md)

新しいスプレッドシートのオブジェクト
