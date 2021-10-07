# Campaign


<div lang=\"ja\">Campaignオブジェクトは、キャンペーン情報を表します。</div> 

## Table of contents

### Properties

- [accountId](campaign.md#accountid)
- [appId](campaign.md#appid)
- [appName](campaign.md#appname)
- [budget](campaign.md#budget)
- [campaignBiddingStrategy](campaign.md#campaignbiddingstrategy)
- [campaignDeliveryType](campaign.md#campaigndeliverytype)
- [campaignGoal](campaign.md#campaigngoal)
- [campaignId](campaign.md#campaignid)
- [campaignName](campaign.md#campaignname)
- [conversionOptimizer](campaign.md#conversionoptimizer)
- [conversionTracker](campaign.md#conversiontracker)
- [createdDate](campaign.md#createddate)
- [customParameters](campaign.md#customparameters)
- [deviceOsType](campaign.md#deviceostype)
- [endDate](campaign.md#enddate)
- [feedId](campaign.md#feedid)
- [isRemoveTrackingUrl](campaign.md#isremovetrackingurl)
- [labels](campaign.md#labels)
- [servingStatus](campaign.md#servingstatus)
- [startDate](campaign.md#startdate)
- [trackingUrl](campaign.md#trackingurl)
- [userStatus](campaign.md#userstatus)
- [vendorName](campaign.md#vendorname)
- [viewableFrequencyCap](campaign.md#viewablefrequencycap)

## Properties

### accountId

• `Optional` **accountId**: ``null`` \| *number*

<div lang=\"ja\"> アカウントIDです。<br> このフィールドは、リクエストの場合は必須です。 </div> 

**`memberof`** Campaign

___

### appId

• `Optional` **appId**: ``null`` \| *string*

<div lang=\"ja\"> iOS:アプリIDです。<br> Android:パッケージ名です。<br> このフィールドは、ADD時に省略可能となり、SETおよびREMOVE時は無視されます。<br> ※campaignGoalが「APP_PROMOTION」の場合、ADD時に必須となります。 </div> 

**`memberof`** Campaign

___

### appName

• `Optional` **appName**: ``null`` \| *string*

<div lang=\"ja\"> アプリの名称です。<br> このフィールドは、ADD時に省略可能となり、SETおよびREMOVE時は無視されます。<br> ※campaignGoalが「APP_PROMOTION」の場合、ADD時に必須となります。 </div> 

**`memberof`** Campaign

___

### budget

• `Optional` **budget**: ``null`` \| [*CampaignServiceBudget*](campaignservicebudget.md)

**`memberof`** Campaign

___

### campaignBiddingStrategy

• `Optional` **campaignBiddingStrategy**: ``null`` \| [*CampaignServiceCampaignBiddingStrategy*](campaignservicecampaignbiddingstrategy.md)

**`memberof`** Campaign

___

### campaignDeliveryType

• `Optional` **campaignDeliveryType**: ``null`` \| *string*

<div lang=\"ja\"> キャンペーン掲載タイプです。<br> このフィールドは、ADDおよびSET時に省略可能となり、REMOVE時に無視されます。<br> CampaignDeliveryTypeを指定してのキャンペーン作成は、一部の利用者向けの機能となります。 </div> 

**`memberof`** Campaign

___

### campaignGoal

• `Optional` **campaignGoal**: ``null`` \| *string*

<div lang=\"ja\"> キャンペーン目的です。<br> ADD時、このフィールドは必須となります。<br> SETおよびREMOVE時、このフィールドは無視されます。<br> ※指定可能な値は、AccountAuthorityServiceのGET操作で得られるAccountAuthorityのauthoritiesフィールドをご確認ください。<br> </div> 

**`memberof`** Campaign

___

### campaignId

• `Optional` **campaignId**: ``null`` \| *number*

<div lang=\"ja\"> キャンペーンIDです。<br> このフィールドはSETおよびREMOVE時に必須となり、ADD時に無視されます。 </div> 

**`memberof`** Campaign

___

### campaignName

• `Optional` **campaignName**: ``null`` \| *string*

<div lang=\"ja\"> キャンペーン名です。<br> このフィールドは、ADD時は必須、SET時は省略可能となり、REMOVE時は無視されます。 </div> 

**`memberof`** Campaign

___

### conversionOptimizer

• `Optional` **conversionOptimizer**: ``null`` \| [*CampaignServiceConversionOptimizer*](campaignserviceconversionoptimizer.md)

**`memberof`** Campaign

___

### conversionTracker

• `Optional` **conversionTracker**: ``null`` \| [*CampaignServiceConversionTracker*](campaignserviceconversiontracker.md)

**`memberof`** Campaign

___

### createdDate

• `Optional` **createdDate**: ``null`` \| *string*

<div lang=\"ja\">キャンペーンが作成された日時です。<br>※フォーマット：yyyyMMdd</div> 

**`memberof`** Campaign

___

### customParameters

• `Optional` **customParameters**: ``null`` \| [*CampaignServiceCustomParameters*](campaignservicecustomparameters.md)

**`memberof`** Campaign

___

### deviceOsType

• `Optional` **deviceOsType**: ``null`` \| [*Android*](./enums/campaignservicedeviceostype.md#android) \| [*Ios*](./enums/campaignservicedeviceostype.md#ios) \| [*Unknown*](./enums/campaignservicedeviceostype.md#unknown)

**`memberof`** Campaign

___

### endDate

• `Optional` **endDate**: ``null`` \| *string*

<div lang=\"ja\"> 終了日です。<br> このフィールドは、ADDおよびSET時に省略可能となり、REMOVE時に無視されます。 </div> 

**`memberof`** Campaign

___

### feedId

• `Optional` **feedId**: ``null`` \| *number*

<div lang=\"ja\"> フィードIDです。<br> このフィールドは、ADD時に省略可能となり、SETおよびREMOVE時に無視されます。<br> ※動的ディスプレイ広告の場合、ADD時に必須となります。 </div> 

**`memberof`** Campaign

___

### isRemoveTrackingUrl

• `Optional` **isRemoveTrackingUrl**: ``null`` \| [*True*](./enums/campaignserviceisremoveflg.md#true) \| [*False*](./enums/campaignserviceisremoveflg.md#false) \| [*Unknown*](./enums/campaignserviceisremoveflg.md#unknown)

**`memberof`** Campaign

___

### labels

• `Optional` **labels**: ``null`` \| [*CampaignServiceLabel*](campaignservicelabel.md)[]

**`memberof`** Campaign

___

### servingStatus

• `Optional` **servingStatus**: ``null`` \| [*Serving*](./enums/campaignserviceservingstatus.md#serving) \| [*Ended*](./enums/campaignserviceservingstatus.md#ended) \| [*Pending*](./enums/campaignserviceservingstatus.md#pending) \| [*Unknown*](./enums/campaignserviceservingstatus.md#unknown)

**`memberof`** Campaign

___

### startDate

• `Optional` **startDate**: ``null`` \| *string*

<div lang=\"ja\"> 開始日です。<br> このフィールドは、ADDおよびSET時に省略可能となり、REMOVE時に無視されます。 </div> 

**`memberof`** Campaign

___

### trackingUrl

• `Optional` **trackingUrl**: ``null`` \| *string*

<div lang=\"ja\">トラッキングURLです。<br> ADD時およびSET時、このフィールドは省略可能となります。<br> ※SET時、こちらが審査中の場合、編集はできません。<br>※現在利用できません</div> 

**`memberof`** Campaign

___

### userStatus

• `Optional` **userStatus**: ``null`` \| [*Active*](./enums/campaignserviceuserstatus.md#active) \| [*Paused*](./enums/campaignserviceuserstatus.md#paused) \| [*Unknown*](./enums/campaignserviceuserstatus.md#unknown)

**`memberof`** Campaign

___

### vendorName

• `Optional` **vendorName**: ``null`` \| *string*

<div lang=\"ja\"> キャンペーンの広告効果測定ツールのベンダー名です。キャンペーン目的「アプリ訴求」の場合にのみ設定されます。<br> このフィールドはキャンペーン作成後、最初にリンク先URLを設定した広告が作成された時に設定されます。<br> キャンペーンに紐づく広告のリンク先URLには、このベンダー名に対応する広告効果測定ツールのURLのみが指定できます。<br> ADDおよびSET時、このフィールドは指定できません。<br> </div> 

**`memberof`** Campaign

___

### viewableFrequencyCap

• `Optional` **viewableFrequencyCap**: ``null`` \| [*CampaignServiceViewableFrequencyCap*](campaignserviceviewablefrequencycap.md)

**`memberof`** Campaign
