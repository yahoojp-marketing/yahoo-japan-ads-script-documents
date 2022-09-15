# AdsUtilities


Yahoo!広告 のUtilityです。

## Table of contents

### Methods

- [getCurrentAccountId](adsutilities.md#getcurrentaccountid)
- [getDisplayReport](adsutilities.md#getdisplayreport)
- [getProductType](adsutilities.md#getproducttype)
- [getSearchReport](adsutilities.md#getsearchreport)

## Methods

### getCurrentAccountId

▸ **getCurrentAccountId**(): *number*

アカウントIDを取得します。

**Returns:** *number*

アカウントID

___

### getDisplayReport

▸ **getDisplayReport**(`reportDefinition`: [*ReportDefinition*](../data/display/reportdefinition.md)): [*Reports*](reports.md)

Yahoo!広告 ディスプレイ広告 のレポートを取得します。

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `reportDefinition` | [*ReportDefinition*](../data/display/reportdefinition.md) | レポート定義情報<br>アカウントIDは未指定の場合、スクリプト所有者のアカウントIDが設定されます。 |

**Returns:** [*Reports*](reports.md)

レポートオブジェクト

___

### getProductType

▸ **getProductType**(): *string*

プロダクトタイプを取得します。<br />
DISPLAY: ディスプレイ広告<br />
SEARCH: 検索広告<br />
MCC: MCC

**Returns:** *string*

プロダクトタイプ

___

### getSearchReport

▸ **getSearchReport**(`reportDefinition`: [*ReportDefinition*](../data/search/reportdefinition.md)): [*Reports*](reports.md)

Yahoo!広告 検索広告 のレポートを取得します。

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `reportDefinition` | [*ReportDefinition*](../data/search/reportdefinition.md) | レポート定義情報<br>アカウントIDは未指定の場合、スクリプト所有者のアカウントIDが設定されます。 |

**Returns:** [*Reports*](reports.md)

レポートオブジェクト
