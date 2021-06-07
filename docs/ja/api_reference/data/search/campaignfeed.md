# CampaignFeed


<div lang=\"ja\">CampaignFeedオブジェクトは、キャンペーンに紐づけられたFeedItem情報を表します。<br> SET時、このフィールドは必須です。</div> 

## Table of contents

### Properties

- [accountId](campaignfeed.md#accountid)
- [campaignId](campaignfeed.md#campaignid)
- [feedItemId](campaignfeed.md#feeditemid)
- [placeholderType](campaignfeed.md#placeholdertype)

## Properties

### accountId

• `Optional` **accountId**: ``null`` \| *number*

<div lang=\"ja\">アカウントIDです。</div> 

**`memberof`** CampaignFeed

___

### campaignId

• `Optional` **campaignId**: ``null`` \| *number*

<div lang=\"ja\">キャンペーンIDです。</div> 

**`memberof`** CampaignFeed

___

### feedItemId

• `Optional` **feedItemId**: ``null`` \| *number*

<div lang=\"ja\">FeedItem情報のIDです。<br> SET時、このフィールドは必須です。</div> 

**`memberof`** CampaignFeed

___

### placeholderType

• `Optional` **placeholderType**: ``null`` \| [*Quicklink*](./enums/campaignfeedserviceplaceholdertype.md#quicklink) \| [*Callextension*](./enums/campaignfeedserviceplaceholdertype.md#callextension) \| [*Callout*](./enums/campaignfeedserviceplaceholdertype.md#callout) \| [*StructuredSnippet*](./enums/campaignfeedserviceplaceholdertype.md#structuredsnippet) \| [*Unknown*](./enums/campaignfeedserviceplaceholdertype.md#unknown)

**`memberof`** CampaignFeed
