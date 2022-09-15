# 自動入札 / Bidding

### ポートフォリオ入札設定を取得する / Get bidding strategies
```.js
function getBiddingStrategy(){
   
  const accountId = AdsUtilities.getCurrentAccountId();
   
  const biddingStrategies = Search.BiddingStrategyService.get({
    accountId: accountId,
  }).rval;
  
  if (biddingStrategies.totalNumEntries == 0) {
    Logger.log('Target ID does not exist.');
    return;
  }
 
  for (let i = 0; i < Object.keys(biddingStrategies.values).length; i++){
    let biddingStrategy = biddingStrategies.values[i].biddingStrategy;
    let type = biddingStrategy.biddingScheme.type;
    Logger.log('biddingStrategyId-> ' + biddingStrategy.biddingStrategyId
      + ', biddingStrategyName-> ' + biddingStrategy.biddingStrategyName + ', type-> ' + type);
  }  
}
```

### 指定したキャンペーンをポートフォリオ入札設定する / Set campaign bidding strategy
```.js
function setCampaignBiddingStrategy(){
   
  const accountId = AdsUtilities.getCurrentAccountId();
  const campaignIds = [1111111, 2222222];//Empty when not specified
  const biddingStrategyId = 33333;
 
  const campaignsGet = Search.CampaignService.get({
    accountId: accountId,
    campaignIds: campaignIds,
  }).rval;
  
  if (campaignsGet.totalNumEntries == 0) {
    Logger.log('Target ID does not exist.');
    return;
  }
  
  const biddingStrategies = Search.BiddingStrategyService.get({
    accountId: accountId,
    biddingStrategyIds: [biddingStrategyId],
  }).rval;

  if(biddingStrategies.totalNumEntries == 0) {
    Logger.log('Target ID of bidding strategy does not exist.');
    return;
  }
  const type = biddingStrategies.values[0].biddingStrategy.biddingScheme.type;
 
  let campaignArray = [];
  for (let i = 0; i < Object.keys(campaignsGet.values).length; i++){   
    let campaign = campaignsGet.values[i].campaign;
    delete campaign.startDate;
    //biddingStrategyId cannot be set at the same time as biddingScheme
    campaign.biddingStrategyConfiguration.biddingScheme = null;
    campaign.biddingStrategyConfiguration.biddingStrategyId = biddingStrategyId;
    campaignArray.push(campaign);
  }

  const campaignsSet = Search.CampaignService.set({
    accountId: accountId,
    operand: campaignArray,
  }).rval;
 
  for (let i = 0; i < Object.keys(campaignsSet.values).length; i++){
    if (campaignsSet.values[i].operationSucceeded) {
      let campaign = campaignsSet.values[i].campaign;
      let biddingStrategy = campaign.biddingStrategyConfiguration;
      Logger.log('campaignId-> ' + campaign.campaignId + ', campaignName-> ' + campaign.campaignName
        + ' has been changed to biddingStrategyId-> ' + biddingStrategy.biddingStrategyId
        + ', biddingStrategyName-> ' + biddingStrategy.biddingStrategyName + ', type-> ' + type);
        
    } else {
      let campaign = campaignsGet.values[i].campaign;
      Logger.log('campaignId-> ' + campaign.campaignId + ', campaignName-> ' + campaign.campaignName + ' could not be changed.');

    }
  }
}
```

### ポートフォリオ入札設定を追加する / Add bidding strategies
```.js
function addCampaignBiddingStrategy() {
  
  const accountId = AdsUtilities.getCurrentAccountId();
  const biddingStrategyArray = [
    {
      accountId: accountId,
      biddingScheme: {
        targetRoasBiddingScheme: {
          targetRoas: 0.5,
        },
        type: 'TARGET_ROAS',
      },
      biddingStrategyName: 'biddingStrategyNameAAA',
    },
    {
      accountId: accountId,
      biddingScheme: {
        targetSpendBiddingScheme: {
          bidCeiling: 1000,
        },
        type: 'TARGET_SPEND',
      },
      biddingStrategyName: 'biddingStrategyNameBBB',
    },
    {
      accountId: accountId,
      biddingScheme: {
        targetCpaBiddingScheme: {
          targetCpa: 200,
        },
        type: 'TARGET_CPA',
      },
      biddingStrategyName: 'biddingStrategyNameCCC',
    },
    {
      accountId: accountId,
      biddingScheme: {
        targetImpressionShareScheme: {
          location: 'ANYWHERE_ON_PAGE',
          bidCeiling: 100,
          targetImpressionShare: 100,
        },
        type: 'TARGET_IMPRESSION_SHARE',
      },
      biddingStrategyName: 'biddingStrategyNameDDD',
    }
  ];//Multiple selections are possible
  
  const biddingStrategies = Search.BiddingStrategyService.add({
    accountId: accountId,
    operand: biddingStrategyArray,
  }).rval;
  
  for (let i = 0; i < Object.keys(biddingStrategies.values).length; i++) {
    if (biddingStrategies.values[i].operationSucceeded) {
      let biddingStrategy = biddingStrategies.values[i].biddingStrategy;
      Logger.log('biddingStrategyId-> ' + biddingStrategy.biddingStrategyId 
        + ', biddingStrategyName-> ' + biddingStrategy.biddingStrategyName
        + ', type-> ' + biddingStrategy.biddingScheme.type + ' has been added.');
        
    } else {
      Logger.log('biddingStrategyName-> ' + biddingStrategyArray[i].biddingStrategyName + ' could not be added.');
      
    }
  }
}
```

