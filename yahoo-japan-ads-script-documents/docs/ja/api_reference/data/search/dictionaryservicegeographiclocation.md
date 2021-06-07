# DictionaryServiceGeographicLocation


<div lang=\"ja\">DictionaryServiceGeographicLocationオブジェクトは、地域情報を格納します。</div> 

## Table of contents

### Properties

- [child](dictionaryservicegeographiclocation.md#child)
- [code](dictionaryservicegeographiclocation.md#code)
- [fullName](dictionaryservicegeographiclocation.md#fullname)
- [geographicLocationStatus](dictionaryservicegeographiclocation.md#geographiclocationstatus)
- [name](dictionaryservicegeographiclocation.md#name)
- [order](dictionaryservicegeographiclocation.md#order)
- [parent](dictionaryservicegeographiclocation.md#parent)

## Properties

### child

• `Optional` **child**: ``null`` \| [*DictionaryServiceGeographicLocation*](dictionaryservicegeographiclocation.md)[]

**`memberof`** DictionaryServiceGeographicLocation

___

### code

• `Optional` **code**: ``null`` \| *string*

<div lang=\"ja\">地域コードです。</div> 

**`memberof`** DictionaryServiceGeographicLocation

___

### fullName

• `Optional` **fullName**: ``null`` \| *string*

<div lang=\"ja\">地域名(都道府県名からすべて)です。</div> 

**`memberof`** DictionaryServiceGeographicLocation

___

### geographicLocationStatus

• `Optional` **geographicLocationStatus**: ``null`` \| [*Active*](./enums/dictionaryservicegeographiclocationstatus.md#active) \| [*Obsolete*](./enums/dictionaryservicegeographiclocationstatus.md#obsolete) \| [*PhasingOut*](./enums/dictionaryservicegeographiclocationstatus.md#phasingout) \| [*Unknown*](./enums/dictionaryservicegeographiclocationstatus.md#unknown)

**`memberof`** DictionaryServiceGeographicLocation

___

### name

• `Optional` **name**: ``null`` \| *string*

<div lang=\"ja\">地域名(市区町村のみ)です。</div> 

**`memberof`** DictionaryServiceGeographicLocation

___

### order

• `Optional` **order**: ``null`` \| *string*

<div lang=\"ja\">並び順です。<br>下記の順序に基づいた連番となります。<br> 都道府県は北海道、青森、・・・・沖縄の順<br>都道府県配下の市区町村は五十音順</div> 

**`memberof`** DictionaryServiceGeographicLocation

___

### parent

• `Optional` **parent**: ``null`` \| *string*

<div lang=\"ja\">上位地域コードです。</div> 

**`memberof`** DictionaryServiceGeographicLocation
