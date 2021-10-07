# AdGroupAdServiceAd


<div lang=\"ja\">AdGroupAdServiceAdオブジェクトは、広告に関する情報を表します。<br> ADD時、このフィールドは必須となります。</div> 

## Table of contents

### Properties

- [adType](adgroupadservicead.md#adtype)
- [additionalAdvancedMobileUrls](adgroupadservicead.md#additionaladvancedmobileurls)
- [additionalAdvancedUrls](adgroupadservicead.md#additionaladvancedurls)
- [advancedMobileUrl](adgroupadservicead.md#advancedmobileurl)
- [advancedUrl](adgroupadservicead.md#advancedurl)
- [appAd](adgroupadservicead.md#appad)
- [customParameters](adgroupadservicead.md#customparameters)
- [description1](adgroupadservicead.md#description1)
- [devicePreference](adgroupadservicead.md#devicepreference)
- [displayUrl](adgroupadservicead.md#displayurl)
- [dynamicSearchLinkedAd](adgroupadservicead.md#dynamicsearchlinkedad)
- [extendedTextAd](adgroupadservicead.md#extendedtextad)
- [headline1](adgroupadservicead.md#headline1)
- [responsiveSearchAd](adgroupadservicead.md#responsivesearchad)
- [textAd2](adgroupadservicead.md#textad2)
- [trackingUrl](adgroupadservicead.md#trackingurl)
- [url](adgroupadservicead.md#url)

## Properties

### adType

• `Optional` **adType**: ``null`` \| [*TextAd2*](./enums/adgroupadserviceadtype.md#textad2) \| [*AppAd*](./enums/adgroupadserviceadtype.md#appad) \| [*ExtendedTextAd*](./enums/adgroupadserviceadtype.md#extendedtextad) \| [*DynamicSearchLinkedAd*](./enums/adgroupadserviceadtype.md#dynamicsearchlinkedad) \| [*ResponsiveSearchAd*](./enums/adgroupadserviceadtype.md#responsivesearchad) \| [*Unknown*](./enums/adgroupadserviceadtype.md#unknown)

**`memberof`** AdGroupAdServiceAd

___

### additionalAdvancedMobileUrls

• `Optional` **additionalAdvancedMobileUrls**: ``null`` \| [*AdGroupAdServiceAdditionalAdvancedMobileUrls*](adgroupadserviceadditionaladvancedmobileurls.md)[]

**`memberof`** AdGroupAdServiceAd

___

### additionalAdvancedUrls

• `Optional` **additionalAdvancedUrls**: ``null`` \| [*AdGroupAdServiceAdditionalAdvancedUrls*](adgroupadserviceadditionaladvancedurls.md)[]

**`memberof`** AdGroupAdServiceAd

___

### advancedMobileUrl

• `Optional` **advancedMobileUrl**: ``null`` \| *string*

<div lang=\"ja\">スマートフォン向けURLです。<br> ADD時、このフィールドは省略可能となります。※adTypeがDYNAMIC_SEARCH_LINKED_ADの場合は無視されます。</div> 

**`memberof`** AdGroupAdServiceAd

___

### advancedUrl

• `Optional` **advancedUrl**: ``null`` \| *string*

<div lang=\"ja\">最終リンク先URLです。<br> ADD時、このフィールドは必須となります。※adTypeがDYNAMIC_SEARCH_LINKED_ADの場合は無視されます。</div> 

**`memberof`** AdGroupAdServiceAd

___

### appAd

• `Optional` **appAd**: ``null`` \| [*AdGroupAdServiceAppAd*](adgroupadserviceappad.md)

**`memberof`** AdGroupAdServiceAd

___

### customParameters

• `Optional` **customParameters**: ``null`` \| [*AdGroupAdServiceCustomParameters*](adgroupadservicecustomparameters.md)

**`memberof`** AdGroupAdServiceAd

___

### description1

• `Optional` **description1**: ``null`` \| *string*

<div lang=\"ja\">説明文です。<br> ADD時、このフィールドは必須となります。※adTypeがRESPONSIVE_SEARCH_ADの場合は無視されます。</div> 

**`memberof`** AdGroupAdServiceAd

___

### devicePreference

• `Optional` **devicePreference**: ``null`` \| [*SmartPhone*](./enums/adgroupadservicedevicepreference.md#smartphone) \| [*Unknown*](./enums/adgroupadservicedevicepreference.md#unknown)

**`memberof`** AdGroupAdServiceAd

___

### displayUrl

• `Optional` **displayUrl**: ``null`` \| *string*

<div lang=\"ja\">表示URLです。<br> このフィールドは、レスポンスの際に返却されますが、リクエストの際には無視されます。</div> 

**`memberof`** AdGroupAdServiceAd

___

### dynamicSearchLinkedAd

• `Optional` **dynamicSearchLinkedAd**: ``null`` \| [*AdGroupAdServiceDynamicSearchLinkedAd*](adgroupadservicedynamicsearchlinkedad.md)

**`memberof`** AdGroupAdServiceAd

___

### extendedTextAd

• `Optional` **extendedTextAd**: ``null`` \| [*AdGroupAdServiceExtendedTextAd*](adgroupadserviceextendedtextad.md)

**`memberof`** AdGroupAdServiceAd

___

### headline1

• `Optional` **headline1**: ``null`` \| *string*

<div lang=\"ja\">タイトル文です。<br> ADD時、このフィールドは必須となります。※adTypeがDYNAMIC_SEARCH_LINKED_AD、またはRESPONSIVE_SEARCH_ADの場合は無視されます。</div> 

**`memberof`** AdGroupAdServiceAd

___

### responsiveSearchAd

• `Optional` **responsiveSearchAd**: ``null`` \| [*AdGroupAdServiceResponsiveSearchAd*](adgroupadserviceresponsivesearchad.md)

**`memberof`** AdGroupAdServiceAd

___

### textAd2

• `Optional` **textAd2**: ``null`` \| [*AdGroupAdServiceTextAd2*](adgroupadservicetextad2.md)

**`memberof`** AdGroupAdServiceAd

___

### trackingUrl

• `Optional` **trackingUrl**: ``null`` \| *string*

<div lang=\"ja\">トラッキングURLです。<br> ADD時、このフィールドは省略可能となります。</div> 

**`memberof`** AdGroupAdServiceAd

___

### url

• `Optional` **url**: ``null`` \| *string*

<div lang=\"ja\">移行前のリンク先URLです。<br> このフィールドは、レスポンスの際に返却されますが、リクエストの際には無視されます。</div> 

**`memberof`** AdGroupAdServiceAd
