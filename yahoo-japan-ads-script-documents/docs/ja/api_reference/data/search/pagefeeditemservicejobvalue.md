# PageFeedItemServiceJobValue


<div lang=\"ja\">PageFeedItemServiceJobValueは、upload、downloadの処理状況を格納するコンテナです。</div> 

## Table of contents

### Properties

- [downloadJob](pagefeeditemservicejobvalue.md#downloadjob)
- [errors](pagefeeditemservicejobvalue.md#errors)
- [operationSucceeded](pagefeeditemservicejobvalue.md#operationsucceeded)
- [uploadJob](pagefeeditemservicejobvalue.md#uploadjob)

## Properties

### downloadJob

• `Optional` **downloadJob**: ``null`` \| [*PageFeedItemServiceDownloadJob*](pagefeeditemservicedownloadjob.md)

**`memberof`** PageFeedItemServiceJobValue

___

### errors

• `Optional` **errors**: ``null`` \| [*ModelError*](modelerror.md)[]

**`memberof`** PageFeedItemServiceJobValue

___

### operationSucceeded

• `Optional` **operationSucceeded**: ``null`` \| *boolean*

<div lang=\"ja\">処理結果です。trueの場合は、処理は成功しました。falseの場合は処理が失敗しています。</div> 

**`memberof`** PageFeedItemServiceJobValue

___

### uploadJob

• `Optional` **uploadJob**: ``null`` \| [*PageFeedItemServiceUploadJob*](pagefeeditemserviceuploadjob.md)

**`memberof`** PageFeedItemServiceJobValue
