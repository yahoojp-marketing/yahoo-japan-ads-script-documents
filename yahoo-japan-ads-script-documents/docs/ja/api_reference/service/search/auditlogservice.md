# AuditLogService


## Table of contents

### Methods

- [addJob](auditlogservice.md#addjob)
- [download](auditlogservice.md#download)
- [get](auditlogservice.md#get)

## Methods

### addJob

▸ **addJob**(`auditLogServiceOperation?`: [*AuditLogServiceOperation*](../../data/search/auditlogserviceoperation.md)): [*AuditLogServiceAddJobResponse*](../../data/search/auditlogserviceaddjobresponse.md)

<div lang=\"ja\">操作履歴ファイルをダウンロードするためのジョブを登録します。</div> 

#### Parameters

| Name | Type |
| :------ | :------ |
| `auditLogServiceOperation?` | [*AuditLogServiceOperation*](../../data/search/auditlogserviceoperation.md) |

**Returns:** [*AuditLogServiceAddJobResponse*](../../data/search/auditlogserviceaddjobresponse.md)

___

### download

▸ **download**(`auditLogServiceDownloadSelector?`: [*AuditLogServiceDownloadSelector*](../../data/search/auditlogservicedownloadselector.md)): *Uint8Array*

<div lang=\"ja\">操作履歴をダウンロードします。</div> 

#### Parameters

| Name | Type |
| :------ | :------ |
| `auditLogServiceDownloadSelector?` | [*AuditLogServiceDownloadSelector*](../../data/search/auditlogservicedownloadselector.md) |

**Returns:** *Uint8Array*

___

### get

▸ **get**(`auditLogServiceSelector?`: [*AuditLogServiceSelector*](../../data/search/auditlogserviceselector.md)): [*AuditLogServiceGetResponse*](../../data/search/auditlogservicegetresponse.md)

<div lang=\"ja\">downloadの処理状況を取得します。</div> 

#### Parameters

| Name | Type |
| :------ | :------ |
| `auditLogServiceSelector?` | [*AuditLogServiceSelector*](../../data/search/auditlogserviceselector.md) |

**Returns:** [*AuditLogServiceGetResponse*](../../data/search/auditlogservicegetresponse.md)
