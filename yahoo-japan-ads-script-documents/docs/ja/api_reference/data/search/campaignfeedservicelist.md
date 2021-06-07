# CampaignFeedServiceList


<div lang=\"ja\">CampaignFeedServiceListオブジェクトは、キャンペーンに関連付けられたFeedItem情報を表します。<br> 更新時にcampaignFeedを指定するとすべて上書きされ、未指定のcampaignFeedの属性情報は削除されます。 </div> 

## Table of contents

### Properties

- [accountId](campaignfeedservicelist.md#accountid)
- [campaignFeed](campaignfeedservicelist.md#campaignfeed)
- [campaignId](campaignfeedservicelist.md#campaignid)
- [placeholderType](campaignfeedservicelist.md#placeholdertype)

## Properties

### accountId

• `Optional` **accountId**: ``null`` \| *number*

<div lang=\"ja\">アカウントIDです。<br> SET時、このフィールドは必須です。</div> 

**`memberof`** CampaignFeedServiceList

___

### campaignFeed

• `Optional` **campaignFeed**: ``null`` \| [*CampaignFeed*](campaignfeed.md)[]

**`memberof`** CampaignFeedServiceList

___

### campaignId

• `Optional` **campaignId**: ``null`` \| *number*

<div lang=\"ja\">キャンペーンIDです。<br> SET時、このフィールドは必須です。</div> 

**`memberof`** CampaignFeedServiceList

___

### placeholderType

• `Optional` **placeholderType**: ``null`` \| [*Quicklink*](./enums/campaignfeedserviceplaceholdertype.md#quicklink) \| [*Callextension*](./enums/campaignfeedserviceplaceholdertype.md#callextension) \| [*Callout*](./enums/campaignfeedserviceplaceholdertype.md#callout) \| [*StructuredSnippet*](./enums/campaignfeedserviceplaceholdertype.md#structuredsnippet) \| [*Unknown*](./enums/campaignfeedserviceplaceholdertype.md#unknown)

**`memberof`** CampaignFeedServiceList
