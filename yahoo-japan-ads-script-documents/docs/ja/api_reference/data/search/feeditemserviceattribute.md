# FeedItemServiceAttribute


<div lang=\"ja\">FeedItemServiceAttributeオブジェクトは、フィードアイテムの属性情報の値を格納します。<br> このフィールドは、ADD時に必須となり、SET時に省略可能となり、REMOVE時に無視されます。<br> SET時にfeedItemAttributeを指定するとすべて上書きされます。 </div> 

## Table of contents

### Properties

- [feedAttributeId](feeditemserviceattribute.md#feedattributeid)
- [multipleFeedItemAttribute](feeditemserviceattribute.md#multiplefeeditemattribute)
- [placeholderField](feeditemserviceattribute.md#placeholderfield)
- [simpleFeedItemAttribute](feeditemserviceattribute.md#simplefeeditemattribute)

## Properties

### feedAttributeId

• `Optional` **feedAttributeId**: ``null`` \| *number*

<div lang=\"ja\">フィード属性IDです。<br> このフィールドは、ADDおよびSET時に無視されます。<br> ※アドカスタマイザーの場合は、ADDおよびSET時に必須となります。</div> 

**`memberof`** FeedItemServiceAttribute

___

### multipleFeedItemAttribute

• `Optional` **multipleFeedItemAttribute**: ``null`` \| [*FeedItemServiceMultipleFeedItemAttribute*](feeditemservicemultiplefeeditemattribute.md)

**`memberof`** FeedItemServiceAttribute

___

### placeholderField

• `Optional` **placeholderField**: ``null`` \| [*LinkText*](./enums/feeditemserviceplaceholderfield.md#linktext) \| [*LinkDescription1*](./enums/feeditemserviceplaceholderfield.md#linkdescription1) \| [*LinkDescription2*](./enums/feeditemserviceplaceholderfield.md#linkdescription2) \| [*AdvancedUrl*](./enums/feeditemserviceplaceholderfield.md#advancedurl) \| [*AdvancedMobileUrl*](./enums/feeditemserviceplaceholderfield.md#advancedmobileurl) \| [*TrackingUrl*](./enums/feeditemserviceplaceholderfield.md#trackingurl) \| [*CallPhoneNumber*](./enums/feeditemserviceplaceholderfield.md#callphonenumber) \| [*AdCustomizerInteger*](./enums/feeditemserviceplaceholderfield.md#adcustomizerinteger) \| [*AdCustomizerPrice*](./enums/feeditemserviceplaceholderfield.md#adcustomizerprice) \| [*AdCustomizerDate*](./enums/feeditemserviceplaceholderfield.md#adcustomizerdate) \| [*AdCustomizerString*](./enums/feeditemserviceplaceholderfield.md#adcustomizerstring) \| [*CalloutText*](./enums/feeditemserviceplaceholderfield.md#callouttext) \| [*AdditionalAdvancedUrls*](./enums/feeditemserviceplaceholderfield.md#additionaladvancedurls) \| [*AdditionalAdvancedMobileUrls*](./enums/feeditemserviceplaceholderfield.md#additionaladvancedmobileurls) \| [*StructuredSnippetHeader*](./enums/feeditemserviceplaceholderfield.md#structuredsnippetheader) \| [*StructuredSnippetValues*](./enums/feeditemserviceplaceholderfield.md#structuredsnippetvalues) \| [*Unknown*](./enums/feeditemserviceplaceholderfield.md#unknown)

**`memberof`** FeedItemServiceAttribute

___

### simpleFeedItemAttribute

• `Optional` **simpleFeedItemAttribute**: ``null`` \| [*FeedItemServiceSimpleFeedItemAttribute*](feeditemservicesimplefeeditemattribute.md)

**`memberof`** FeedItemServiceAttribute
