# AdGroupAdServiceBid


<div lang=\"ja\"> AdGroupAdServiceBidオブジェクトは、入札最適化方法を格納するコンテナです。<br> SET時、このフィールドは省略可能となります。<br> ADD時、このフィールドは指定できません。 </div> 

## Table of contents

### Properties

- [biddingStrategyType](adgroupadservicebid.md#biddingstrategytype)
- [manualCPCAdGroupAdBid](adgroupadservicebid.md#manualcpcadgroupadbid)
- [manualCPVAdGroupAdBid](adgroupadservicebid.md#manualcpvadgroupadbid)

## Properties

### biddingStrategyType

• `Optional` **biddingStrategyType**: ``null`` \| [*ManualCpc*](./enums/adgroupadservicebiddingstrategytype.md#manualcpc) \| [*ManualCpv*](./enums/adgroupadservicebiddingstrategytype.md#manualcpv) \| [*Unknown*](./enums/adgroupadservicebiddingstrategytype.md#unknown)

**`memberof`** AdGroupAdServiceBid

___

### manualCPCAdGroupAdBid

• `Optional` **manualCPCAdGroupAdBid**: ``null`` \| [*AdGroupAdServiceManualCPCAdGroupAdBid*](adgroupadservicemanualcpcadgroupadbid.md)

**`memberof`** AdGroupAdServiceBid

___

### manualCPVAdGroupAdBid

• `Optional` **manualCPVAdGroupAdBid**: ``null`` \| [*AdGroupAdServiceManualCPVAdGroupAdBid*](adgroupadservicemanualcpvadgroupadbid.md)

**`memberof`** AdGroupAdServiceBid
