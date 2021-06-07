# PageFeedItemService


## Table of contents

### Methods

- [addDownloadJob](pagefeeditemservice.md#adddownloadjob)
- [download](pagefeeditemservice.md#download)
- [downloadErrorFile](pagefeeditemservice.md#downloaderrorfile)
- [get](pagefeeditemservice.md#get)
- [getJobStatus](pagefeeditemservice.md#getjobstatus)
- [getReviewSummary](pagefeeditemservice.md#getreviewsummary)
- [upload](pagefeeditemservice.md#upload)

## Methods

### addDownloadJob

▸ **addDownloadJob**(`pageFeedItemServiceDownloadJobOperation?`: [*PageFeedItemServiceDownloadJobOperation*](../../data/search/pagefeeditemservicedownloadjoboperation.md)): [*PageFeedItemServiceAddDownloadJobResponse*](../../data/search/pagefeeditemserviceadddownloadjobresponse.md)

<div lang=\"ja\">登録されているページフィードアイテムを一括でダウンロードするためジョブを登録します。</div> 

#### Parameters

| Name | Type |
| :------ | :------ |
| `pageFeedItemServiceDownloadJobOperation?` | [*PageFeedItemServiceDownloadJobOperation*](../../data/search/pagefeeditemservicedownloadjoboperation.md) |

**Returns:** [*PageFeedItemServiceAddDownloadJobResponse*](../../data/search/pagefeeditemserviceadddownloadjobresponse.md)

___

### download

▸ **download**(`pageFeedItemServiceDownloadSelector?`: [*PageFeedItemServiceDownloadSelector*](../../data/search/pagefeeditemservicedownloadselector.md)): *Uint8Array*

<div lang=\"ja\">ページフィードアイテムをダウンロードします。</div> 

#### Parameters

| Name | Type |
| :------ | :------ |
| `pageFeedItemServiceDownloadSelector?` | [*PageFeedItemServiceDownloadSelector*](../../data/search/pagefeeditemservicedownloadselector.md) |

**Returns:** *Uint8Array*

___

### downloadErrorFile

▸ **downloadErrorFile**(`pageFeedItemServiceDownloadSelector?`: [*PageFeedItemServiceDownloadSelector*](../../data/search/pagefeeditemservicedownloadselector.md)): *Uint8Array*

<div lang=\"ja\">ページフィードアイテムのエラーファイルをダウンロードします。</div> 

#### Parameters

| Name | Type |
| :------ | :------ |
| `pageFeedItemServiceDownloadSelector?` | [*PageFeedItemServiceDownloadSelector*](../../data/search/pagefeeditemservicedownloadselector.md) |

**Returns:** *Uint8Array*

___

### get

▸ **get**(`pageFeedItemServiceSelector?`: [*PageFeedItemServiceSelector*](../../data/search/pagefeeditemserviceselector.md)): [*PageFeedItemServiceGetResponse*](../../data/search/pagefeeditemservicegetresponse.md)

<div lang=\"ja\">ページフィードアイテム情報を取得します。</div> 

#### Parameters

| Name | Type |
| :------ | :------ |
| `pageFeedItemServiceSelector?` | [*PageFeedItemServiceSelector*](../../data/search/pagefeeditemserviceselector.md) |

**Returns:** [*PageFeedItemServiceGetResponse*](../../data/search/pagefeeditemservicegetresponse.md)

___

### getJobStatus

▸ **getJobStatus**(`pageFeedItemServiceJobStatusSelector?`: [*PageFeedItemServiceJobStatusSelector*](../../data/search/pagefeeditemservicejobstatusselector.md)): [*PageFeedItemServiceGetJobStatusResponse*](../../data/search/pagefeeditemservicegetjobstatusresponse.md)

<div lang=\"ja\">upload、downloadの処理状況を取得します。</div> 

#### Parameters

| Name | Type |
| :------ | :------ |
| `pageFeedItemServiceJobStatusSelector?` | [*PageFeedItemServiceJobStatusSelector*](../../data/search/pagefeeditemservicejobstatusselector.md) |

**Returns:** [*PageFeedItemServiceGetJobStatusResponse*](../../data/search/pagefeeditemservicegetjobstatusresponse.md)

___

### getReviewSummary

▸ **getReviewSummary**(`pageFeedItemServiceReviewSummarySelector?`: [*PageFeedItemServiceReviewSummarySelector*](../../data/search/pagefeeditemservicereviewsummaryselector.md)): [*PageFeedItemServiceGetReviewSummaryResponse*](../../data/search/pagefeeditemservicegetreviewsummaryresponse.md)

<div lang=\"ja\">登録されているページフィードアイテムの審査成績・状況のサマリーを取得します。</div> 

#### Parameters

| Name | Type |
| :------ | :------ |
| `pageFeedItemServiceReviewSummarySelector?` | [*PageFeedItemServiceReviewSummarySelector*](../../data/search/pagefeeditemservicereviewsummaryselector.md) |

**Returns:** [*PageFeedItemServiceGetReviewSummaryResponse*](../../data/search/pagefeeditemservicegetreviewsummaryresponse.md)

___

### upload

▸ **upload**(`accountId`: *number*, `uploadType`: ``"NEW_OR_REPLACE"`` \| ``"MODIFY"``, `feedId`: *number*, `file?`: *any*): [*PageFeedItemServiceUploadResponse*](../../data/search/pagefeeditemserviceuploadresponse.md)

<div lang=\"ja\">ページフィードアイテムのアップロード処理を実施します。</div> 

#### Parameters

| Name | Type |
| :------ | :------ |
| `accountId` | *number* |
| `uploadType` | ``"NEW_OR_REPLACE"`` \| ``"MODIFY"`` |
| `feedId` | *number* |
| `file?` | *any* |

**Returns:** [*PageFeedItemServiceUploadResponse*](../../data/search/pagefeeditemserviceuploadresponse.md)
