# GuaranteedSimulationServicePrediction


<div lang=\"ja\"> GuaranteedSimulationServicePredictionオブジェクトは、GuaranteedSimulationオブジェクトで定義された条件に基づく配信シミュレーションの予測結果を表します。<br> - results: 予約確定前の配信シミュレーションの予測結果のデータセットです。<br> - requestedConditionResult: 指定された条件（sov, reach, vImps, lifetimeBudget）に関連する予約確定前の配信シミュレーションの予測結果です。<br> - reservedConditionResult: 指定された条件（sov, reach, vImps, lifetimeBudget）に関連する予約確定後の配信シミュレーションの予測結果です。 </div> 

## Table of contents

### Properties

- [requestedConditionResult](guaranteedsimulationserviceprediction.md#requestedconditionresult)
- [reservedConditionResult](guaranteedsimulationserviceprediction.md#reservedconditionresult)
- [results](guaranteedsimulationserviceprediction.md#results)

## Properties

### requestedConditionResult

• `Optional` **requestedConditionResult**: ``null`` \| [*GuaranteedSimulationServicePredictionResult*](guaranteedsimulationservicepredictionresult.md)

**`memberof`** GuaranteedSimulationServicePrediction

___

### reservedConditionResult

• `Optional` **reservedConditionResult**: ``null`` \| [*GuaranteedSimulationServicePredictionResult*](guaranteedsimulationservicepredictionresult.md)

**`memberof`** GuaranteedSimulationServicePrediction

___

### results

• `Optional` **results**: ``null`` \| [*GuaranteedSimulationServicePredictionResult*](guaranteedsimulationservicepredictionresult.md)[]

**`memberof`** GuaranteedSimulationServicePrediction
