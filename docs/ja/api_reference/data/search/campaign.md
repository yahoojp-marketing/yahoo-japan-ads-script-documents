# Campaign


<div lang=\"ja\">Campaignオブジェクトは、キャンペーンの情報を表します。</div> 

## Table of contents

### Properties

- [accountId](campaign.md#accountid)
- [appId](campaign.md#appid)
- [appStore](campaign.md#appstore)
- [biddingStrategyConfiguration](campaign.md#biddingstrategyconfiguration)
- [biddingStrategyFailedReason](campaign.md#biddingstrategyfailedreason)
- [budget](campaign.md#budget)
- [campaignId](campaign.md#campaignid)
- [campaignName](campaign.md#campaignname)
- [campaignTrackId](campaign.md#campaigntrackid)
- [conversionOptimizerEligibility](campaign.md#conversionoptimizereligibility)
- [createdDate](campaign.md#createddate)
- [customParameters](campaign.md#customparameters)
- [endDate](campaign.md#enddate)
- [failedBiddingStrategyConfiguration](campaign.md#failedbiddingstrategyconfiguration)
- [labels](campaign.md#labels)
- [servingStatus](campaign.md#servingstatus)
- [settings](campaign.md#settings)
- [startDate](campaign.md#startdate)
- [trackingUrl](campaign.md#trackingurl)
- [type](campaign.md#type)
- [urlReviewData](campaign.md#urlreviewdata)
- [userStatus](campaign.md#userstatus)

## Properties

### accountId

• `Optional` **accountId**: ``null`` \| *number*

<div lang=\"ja\">アカウントIDです。<br> このフィールドは、レスポンスの際に返却されますが、リクエストの際には無視されます。</div> 

**`memberof`** Campaign

___

### appId

• `Optional` **appId**: ``null`` \| *string*

<div lang=\"ja\">アプリID（iOS）またはパッケージ名（Android）です。<br> ※アプリキャンペーンでiOSの場合、入力は数値のみです。<br> ADD時、campaignTypeがSTANDARD、またはDYNAMIC_ADS_FOR_SEARCH_SETTINGの場合、無視され、MOBILE_APPの場合、必須となります。</div> 

**`memberof`** Campaign

___

### appStore

• `Optional` **appStore**: ``null`` \| [*Ios*](./enums/campaignserviceappstore.md#ios) \| [*Android*](./enums/campaignserviceappstore.md#android) \| [*Unknown*](./enums/campaignserviceappstore.md#unknown)

**`memberof`** Campaign

___

### biddingStrategyConfiguration

• `Optional` **biddingStrategyConfiguration**: ``null`` \| [*CampaignServiceBiddingStrategy*](campaignservicebiddingstrategy.md)

**`memberof`** Campaign

___

### biddingStrategyFailedReason

• `Optional` **biddingStrategyFailedReason**: ``null`` \| [*Failure*](./enums/campaignservicebiddingstrategyfailedreason.md#failure) \| [*ConversionTrackingNotEnabled*](./enums/campaignservicebiddingstrategyfailedreason.md#conversiontrackingnotenabled) \| [*NotEnoughConversions*](./enums/campaignservicebiddingstrategyfailedreason.md#notenoughconversions) \| [*CannotCreateCampaignWithConversionOptimizer*](./enums/campaignservicebiddingstrategyfailedreason.md#cannotcreatecampaignwithconversionoptimizer) \| [*BiddingStrategyCannotBeOverridden*](./enums/campaignservicebiddingstrategyfailedreason.md#biddingstrategycannotbeoverridden) \| [*NotCpcCampaign*](./enums/campaignservicebiddingstrategyfailedreason.md#notcpccampaign) \| [*Unknown*](./enums/campaignservicebiddingstrategyfailedreason.md#unknown)

**`memberof`** Campaign

___

### budget

• `Optional` **budget**: ``null`` \| [*CampaignServiceBudget*](campaignservicebudget.md)

**`memberof`** Campaign

___

### campaignId

• `Optional` **campaignId**: ``null`` \| *number*

<div lang=\"ja\">キャンペーンIDです。<br> SET時およびREMOVE時、このフィールドは必須です。</div> 

**`memberof`** Campaign

___

### campaignName

• `Optional` **campaignName**: ``null`` \| *string*

<div lang=\"ja\">キャンペーン名です。<br>このフィールドは、ADD時に必須となり、SET時に省略可能となります。<br> ※入力制限：50文字以内です。</div> 

**`memberof`** Campaign

___

### campaignTrackId

• `Optional` **campaignTrackId**: ``null`` \| *number*

<div lang=\"ja\">トラッキング用キャンペーンIDです。<br> このフィールドは、レスポンスの際に返却されますが、リクエストの際には無視されます。</div> 

**`memberof`** Campaign

___

### conversionOptimizerEligibility

• `Optional` **conversionOptimizerEligibility**: ``null`` \| [*Enable*](./enums/campaignserviceconversionoptimizereligibility.md#enable) \| [*Disable*](./enums/campaignserviceconversionoptimizereligibility.md#disable) \| [*CampaignIsNotActive*](./enums/campaignserviceconversionoptimizereligibility.md#campaignisnotactive) \| [*NotCpcCampaign*](./enums/campaignserviceconversionoptimizereligibility.md#notcpccampaign) \| [*ConversionTrackingNotEnabled*](./enums/campaignserviceconversionoptimizereligibility.md#conversiontrackingnotenabled) \| [*NotEnoughConversions*](./enums/campaignserviceconversionoptimizereligibility.md#notenoughconversions) \| [*Unknown*](./enums/campaignserviceconversionoptimizereligibility.md#unknown)

**`memberof`** Campaign

___

### createdDate

• `Optional` **createdDate**: ``null`` \| *string*

<div lang=\"ja\">キャンペーンが作成された日です。<br>※フォーマット：yyyyMMdd</div> 

**`memberof`** Campaign

___

### customParameters

• `Optional` **customParameters**: ``null`` \| [*CampaignServiceCustomParameters*](campaignservicecustomparameters.md)

**`memberof`** Campaign

___

### endDate

• `Optional` **endDate**: ``null`` \| *string*

<div lang=\"ja\">キャンペーンの終了日です。<br> ADD時およびSET時、このフィールドは省略可能となります。ADD時のデフォルト設定値は20371231となります。<br> 過去の日付、開始日以前の日付は指定できません。<br>※YYYYMMDD形式です。</div> 

**`memberof`** Campaign

___

### failedBiddingStrategyConfiguration

• `Optional` **failedBiddingStrategyConfiguration**: ``null`` \| [*CampaignServiceBiddingStrategy*](campaignservicebiddingstrategy.md)

**`memberof`** Campaign

___

### labels

• `Optional` **labels**: ``null`` \| [*CampaignServiceLabel*](campaignservicelabel.md)[]

**`memberof`** Campaign

___

### servingStatus

• `Optional` **servingStatus**: ``null`` \| [*Serving*](./enums/campaignserviceservingstatus.md#serving) \| [*Ended*](./enums/campaignserviceservingstatus.md#ended) \| [*Pending*](./enums/campaignserviceservingstatus.md#pending) \| [*Stop*](./enums/campaignserviceservingstatus.md#stop) \| [*Unknown*](./enums/campaignserviceservingstatus.md#unknown)

**`memberof`** Campaign

___

### settings

• `Optional` **settings**: ``null`` \| [*CampaignServiceSettings*](campaignservicesettings.md)[]

**`memberof`** Campaign

___

### startDate

• `Optional` **startDate**: ``null`` \| *string*

<div lang=\"ja\">キャンペーンの開始日です。<br> ADD時およびSET時、このフィールドは省略可能となります。ADD時のデフォルト設定値は当日日付となります。<br> 過去の日付は指定できません。<br>※配信開始済みのキャンペーンは変更できません。<br> ※YYYYMMDD形式です。</div> 

**`memberof`** Campaign

___

### trackingUrl

• `Optional` **trackingUrl**: ``null`` \| *string*

<div lang=\"ja\">トラッキングURLです。<br> ADD時およびSET時、このフィールドは省略可能となります。<br> ※アプリキャンペーンがAndroidの場合、設定はできません。</div> 

**`memberof`** Campaign

___

### type

• `Optional` **type**: ``null`` \| [*Standard*](./enums/campaignservicetype.md#standard) \| [*MobileApp*](./enums/campaignservicetype.md#mobileapp) \| [*DynamicAdsForSearch*](./enums/campaignservicetype.md#dynamicadsforsearch) \| [*Unknown*](./enums/campaignservicetype.md#unknown)

**`memberof`** Campaign

___

### urlReviewData

• `Optional` **urlReviewData**: ``null`` \| [*CampaignServiceUrlReviewData*](campaignserviceurlreviewdata.md)

**`memberof`** Campaign

___

### userStatus

• `Optional` **userStatus**: ``null`` \| [*Active*](./enums/campaignserviceuserstatus.md#active) \| [*Paused*](./enums/campaignserviceuserstatus.md#paused) \| [*Unknown*](./enums/campaignserviceuserstatus.md#unknown)

**`memberof`** Campaign
