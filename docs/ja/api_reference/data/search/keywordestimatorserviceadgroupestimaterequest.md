# KeywordEstimatorServiceAdGroupEstimateRequest


<div lang=\"ja\">AdGroupEstimateRequestオブジェクトは、見積もりを行う広告グループを格納するコンテナです。</div> 

## Table of contents

### Properties

- [adGroupId](keywordestimatorserviceadgroupestimaterequest.md#adgroupid)
- [keywordEstimateRequests](keywordestimatorserviceadgroupestimaterequest.md#keywordestimaterequests)
- [maxCpc](keywordestimatorserviceadgroupestimaterequest.md#maxcpc)

## Properties

### adGroupId

• `Optional` **adGroupId**: ``null`` \| *number*

<div lang=\"ja\">広告グループIDです。<br> ※campaignIdを指定していないとき、このフィールドを指定することはできません。</div> 

**`memberof`** KeywordEstimatorServiceAdGroupEstimateRequest

___

### keywordEstimateRequests

• **keywordEstimateRequests**: ``null`` \| [*KeywordEstimatorServiceKeywordEstimateRequest*](keywordestimatorservicekeywordestimaterequest.md)[]

<div lang=\"ja\">見積もりを行うキーワードのコンテナです。</div> 

**`memberof`** KeywordEstimatorServiceAdGroupEstimateRequest

___

### maxCpc

• `Optional` **maxCpc**: ``null`` \| *number*

<div lang=\"ja\">広告グループの見積もりに使用する上限クリック単価です。</div> 

**`memberof`** KeywordEstimatorServiceAdGroupEstimateRequest
