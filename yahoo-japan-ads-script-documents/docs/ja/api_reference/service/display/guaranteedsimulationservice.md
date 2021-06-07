# GuaranteedSimulationService


## Table of contents

### Methods

- [add](guaranteedsimulationservice.md#add)
- [get](guaranteedsimulationservice.md#get)
- [getAdCategory](guaranteedsimulationservice.md#getadcategory)
- [getPackage](guaranteedsimulationservice.md#getpackage)

## Methods

### add

▸ **add**(`guaranteedSimulationServiceOperation?`: [*GuaranteedSimulationServiceOperation*](../../data/display/guaranteedsimulationserviceoperation.md)): [*GuaranteedSimulationServiceMutateResponse*](../../data/display/guaranteedsimulationservicemutateresponse.md)

<div lang=\"ja\">   予約型キャンペーンの配信シミュレーションに関する情報を追加します。<br>   ※GuaranteedSimulationService/addによる配信シミュレーションの実施は、一部の利用者向けの限定機能となります。<br>   ※リクエスト制限は「最大5件/秒」固定です。サービス種別「campaign」とは別にカウントされます。 </div> 

#### Parameters

| Name | Type |
| :------ | :------ |
| `guaranteedSimulationServiceOperation?` | [*GuaranteedSimulationServiceOperation*](../../data/display/guaranteedsimulationserviceoperation.md) |

**Returns:** [*GuaranteedSimulationServiceMutateResponse*](../../data/display/guaranteedsimulationservicemutateresponse.md)

___

### get

▸ **get**(`guaranteedSimulationServiceSelector?`: [*GuaranteedSimulationServiceSelector*](../../data/display/guaranteedsimulationserviceselector.md)): [*GuaranteedSimulationServiceGetResponse*](../../data/display/guaranteedsimulationservicegetresponse.md)

<div lang=\"ja\">予約型キャンペーンの配信シミュレーション結果に関する情報を取得します。</div> 

#### Parameters

| Name | Type |
| :------ | :------ |
| `guaranteedSimulationServiceSelector?` | [*GuaranteedSimulationServiceSelector*](../../data/display/guaranteedsimulationserviceselector.md) |

**Returns:** [*GuaranteedSimulationServiceGetResponse*](../../data/display/guaranteedsimulationservicegetresponse.md)

___

### getAdCategory

▸ **getAdCategory**(`body?`: *object*): [*GuaranteedSimulationServiceGetAdCategoryResponse*](../../data/display/guaranteedsimulationservicegetadcategoryresponse.md)

<div lang=\"ja\">予約型キャンペーンの配信シミュレーションにおける広告カテゴリー一覧を取得します。</div> 

#### Parameters

| Name | Type |
| :------ | :------ |
| `body?` | *object* |

**Returns:** [*GuaranteedSimulationServiceGetAdCategoryResponse*](../../data/display/guaranteedsimulationservicegetadcategoryresponse.md)

___

### getPackage

▸ **getPackage**(`guaranteedSimulationServicePackageSelector?`: [*GuaranteedSimulationServicePackageSelector*](../../data/display/guaranteedsimulationservicepackageselector.md)): [*GuaranteedSimulationServiceGetPackageResponse*](../../data/display/guaranteedsimulationservicegetpackageresponse.md)

<div lang=\"ja\">予約型キャンペーンの配信シミュレーションのための商品一覧を取得します。</div> 

#### Parameters

| Name | Type |
| :------ | :------ |
| `guaranteedSimulationServicePackageSelector?` | [*GuaranteedSimulationServicePackageSelector*](../../data/display/guaranteedsimulationservicepackageselector.md) |

**Returns:** [*GuaranteedSimulationServiceGetPackageResponse*](../../data/display/guaranteedsimulationservicegetpackageresponse.md)
