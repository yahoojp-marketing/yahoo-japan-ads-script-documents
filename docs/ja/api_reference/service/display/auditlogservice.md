# AuditLogService


## Table of contents

### Methods

- [add](auditlogservice.md#add)
- [download](auditlogservice.md#download)
- [get](auditlogservice.md#get)

## Methods

### add

▸ **add**(`auditLogServiceOperation?`: [*AuditLogServiceOperation*](../../data/display/auditlogserviceoperation.md)): [*AuditLogServiceMutateResponse*](../../data/display/auditlogservicemutateresponse.md)

<div lang=\"ja\">操作履歴ファイルをダウンロードするためのジョブを登録します。</div> 

#### Parameters

| Name | Type |
| :------ | :------ |
| `auditLogServiceOperation?` | [*AuditLogServiceOperation*](../../data/display/auditlogserviceoperation.md) |

**Returns:** [*AuditLogServiceMutateResponse*](../../data/display/auditlogservicemutateresponse.md)

___

### download

▸ **download**(`auditLogServiceDownloadSelector?`: [*AuditLogServiceDownloadSelector*](../../data/display/auditlogservicedownloadselector.md)): *Uint8Array*

<div lang=\"ja\">操作履歴をダウンロードします。</div> 

#### Parameters

| Name | Type |
| :------ | :------ |
| `auditLogServiceDownloadSelector?` | [*AuditLogServiceDownloadSelector*](../../data/display/auditlogservicedownloadselector.md) |

**Returns:** *Uint8Array*

___

### get

▸ **get**(`auditLogServiceSelector?`: [*AuditLogServiceSelector*](../../data/display/auditlogserviceselector.md)): [*AuditLogServiceGetResponse*](../../data/display/auditlogservicegetresponse.md)

<div lang=\"ja\">操作履歴のダウンロード実行結果情報を取得します。</div> 

#### Parameters

| Name | Type |
| :------ | :------ |
| `auditLogServiceSelector?` | [*AuditLogServiceSelector*](../../data/display/auditlogserviceselector.md) |

**Returns:** [*AuditLogServiceGetResponse*](../../data/display/auditlogservicegetresponse.md)
