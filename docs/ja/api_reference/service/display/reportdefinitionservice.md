# ReportDefinitionService


## Table of contents

### Methods

- [add](reportdefinitionservice.md#add)
- [download](reportdefinitionservice.md#download)
- [get](reportdefinitionservice.md#get)
- [getReportFields](reportdefinitionservice.md#getreportfields)
- [remove](reportdefinitionservice.md#remove)

## Methods

### add

▸ **add**(`reportDefinitionServiceOperation?`: [*ReportDefinitionServiceOperation*](../../data/display/reportdefinitionserviceoperation.md)): [*ReportDefinitionServiceMutateResponse*](../../data/display/reportdefinitionservicemutateresponse.md)

<div lang=\"ja\">レポート定義を追加します。</div> 

#### Parameters

| Name | Type |
| :------ | :------ |
| `reportDefinitionServiceOperation?` | [*ReportDefinitionServiceOperation*](../../data/display/reportdefinitionserviceoperation.md) |

**Returns:** [*ReportDefinitionServiceMutateResponse*](../../data/display/reportdefinitionservicemutateresponse.md)

___

### download

▸ **download**(`reportDefinitionServiceDownloadSelector?`: [*ReportDefinitionServiceDownloadSelector*](../../data/display/reportdefinitionservicedownloadselector.md)): *Uint8Array*

<div lang=\"ja\">レポート定義に関する情報をダウンロードします。</div> 

#### Parameters

| Name | Type |
| :------ | :------ |
| `reportDefinitionServiceDownloadSelector?` | [*ReportDefinitionServiceDownloadSelector*](../../data/display/reportdefinitionservicedownloadselector.md) |

**Returns:** *Uint8Array*

___

### get

▸ **get**(`reportDefinitionServiceSelector?`: [*ReportDefinitionServiceSelector*](../../data/display/reportdefinitionserviceselector.md)): [*ReportDefinitionServiceGetResponse*](../../data/display/reportdefinitionservicegetresponse.md)

<div lang=\"ja\">レポート定義に関する情報を取得します。</div> 

#### Parameters

| Name | Type |
| :------ | :------ |
| `reportDefinitionServiceSelector?` | [*ReportDefinitionServiceSelector*](../../data/display/reportdefinitionserviceselector.md) |

**Returns:** [*ReportDefinitionServiceGetResponse*](../../data/display/reportdefinitionservicegetresponse.md)

___

### getReportFields

▸ **getReportFields**(`reportDefinitionServiceGetReportFields?`: [*ReportDefinitionServiceGetReportFields*](../../data/display/reportdefinitionservicegetreportfields.md)): [*ReportDefinitionServiceGetReportFieldsResponse*](../../data/display/reportdefinitionservicegetreportfieldsresponse.md)

<div lang=\"ja\">レポートタイプに対して使用可能なレポートのフィールドを返します。</div> 

#### Parameters

| Name | Type |
| :------ | :------ |
| `reportDefinitionServiceGetReportFields?` | [*ReportDefinitionServiceGetReportFields*](../../data/display/reportdefinitionservicegetreportfields.md) |

**Returns:** [*ReportDefinitionServiceGetReportFieldsResponse*](../../data/display/reportdefinitionservicegetreportfieldsresponse.md)

___

### remove

▸ **remove**(`reportDefinitionServiceOperation?`: [*ReportDefinitionServiceOperation*](../../data/display/reportdefinitionserviceoperation.md)): [*ReportDefinitionServiceMutateResponse*](../../data/display/reportdefinitionservicemutateresponse.md)

<div lang=\"ja\">レポート定義を削除します。</div> 

#### Parameters

| Name | Type |
| :------ | :------ |
| `reportDefinitionServiceOperation?` | [*ReportDefinitionServiceOperation*](../../data/display/reportdefinitionserviceoperation.md) |

**Returns:** [*ReportDefinitionServiceMutateResponse*](../../data/display/reportdefinitionservicemutateresponse.md)
