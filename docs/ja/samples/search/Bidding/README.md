# 自動入札 / Bidding

### 自動入札情報を取得する / Get bidding strategies
```.js
function getBiddingStrategies(){
     
    const accountId = AdsUtilities.getCurrentAccountId();
     
    const biddingStrategies = Search.BiddingStrategyService.get({
        "accountId": accountId,
        "biddingStrategyTypes": [
            "TARGET_CPA",
        ],
    }).rval;
 
    for (let i = 0; i < biddingStrategies.totalNumEntries; i++){
        let biddingStrategy = biddingStrategies.values[i].biddingStrategy;
 
        let targetCpa = biddingStrategy.biddingScheme.targetCpaBiddingScheme;
 
        Logger.log('biddingStrategyId-> ' + biddingStrategy.biddingStrategyId + ', type-> ' + biddingStrategy.type
            + ', bidCeiling-> ' + targetCpa.bidCeiling + ', bidFloor-> ' + targetCpa.bidFloor + ', targetCpa-> ' + targetCpa.targetCpa);
    }  
}
```

### 指定したキャンペーン配下の自動入札情報を更新する / Set campaign bidding strategy
```.js
function setCampaignBiddingStrategy(){
     
    const accountId = AdsUtilities.getCurrentAccountId();
 
    const campaignsGet = Search.CampaignService.get({
        "accountId": accountId,
        "campaignIds": [
            111111,//Multiple selections are possible
        ],
    }).rval;
 
    let campaignArray = [];
 
    for (let i = 0; i < campaignsGet.totalNumEntries; i++){   
        let campaign = campaignsGet.values[i].campaign;
         
        //biddingStrategyId cannot be set at the same time as biddingScheme
        campaign.biddingStrategyConfiguration.biddingScheme = null;
        campaign.biddingStrategyConfiguration.biddingStrategyId = 2222;
         
        campaignArray.push(campaign);
    }
     
    const campaignsSet = Search.CampaignService.set({
        "accountId": accountId,
        "operand": campaignArray,
    }).rval;
 
    for (let i = 0; i < Object.keys(campaignsSet.values).length; i++){   
        let campaign = campaignsSet.values[i].campaign;
        Logger.log('campaignId -> ' + campaign.campaignId
            + ', biddingStrategyId -> ' + campaign.biddingStrategyConfiguration.biddingStrategyId
            + ', biddingStrategyType -> ' + campaign.biddingStrategyConfiguration.biddingStrategyType);
    }
}
```
