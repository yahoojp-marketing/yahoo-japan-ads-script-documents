# ConversionGroup


<div lang=\"ja\">ConversionGroupオブジェクトは、コンバージョングループ情報を表します。</div> 

## Table of contents

### Properties

- [accountId](conversiongroup.md#accountid)
- [conversionGroupId](conversiongroup.md#conversiongroupid)
- [conversionGroupName](conversiongroup.md#conversiongroupname)
- [conversions](conversiongroup.md#conversions)

## Properties

### accountId

• `Optional` **accountId**: ``null`` \| *number*

<div lang=\"ja\"> アカウントIDです。<br> このフィールドは、レスポンスの際に返却されますが、リクエストの際には無視されます。 </div> 

**`memberof`** ConversionGroup

___

### conversionGroupId

• `Optional` **conversionGroupId**: ``null`` \| *number*

<div lang=\"ja\"> コンバージョングループIDです。<br> このフィールドは、ADD時は無視され、SETおよびREMOVE時は必須となります。 </div> 

**`memberof`** ConversionGroup

___

### conversionGroupName

• `Optional` **conversionGroupName**: ``null`` \| *string*

<div lang=\"ja\"> コンバージョングループ名です。<br> このフィールドは、ADD時は必須となり、SET時は省略可能となります。 </div> 

**`memberof`** ConversionGroup

___

### conversions

• `Optional` **conversions**: ``null`` \| [*ConversionGroupServiceConversion*](conversiongroupserviceconversion.md)[]

**`memberof`** ConversionGroup
