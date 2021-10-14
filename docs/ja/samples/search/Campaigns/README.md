# キャンペーン / Campaigns

### 全てのキャンペーン情報を取得する / Get all campaigns
```.js
function getAllCampaigns() {
     
    const accountId = AdsUtilities.getCurrentAccountId();
     
    const campaigns = Search.CampaignService.get({
        "accountId": accountId,
    }).rval;
 
    for (let i = 0; i < campaigns.totalNumEntries; i++){   
        let campaign = campaigns.values[i].campaign;
         
        Logger.log('campaignId -> ' + campaign.campaignId + ', campaignName -> ' + campaign.campaignName);
    }
}
```

### 指定した全てのキャンペーン情報を取得する / Get a campaign by id
```.js
function getCampaignById() {
     
    const accountId = AdsUtilities.getCurrentAccountId();
     
    const campaigns = Search.CampaignService.get({
        "accountId": accountId,
        "campaignIds": [
            926449, 926240,//Multiple selections are possible
        ],
    }).rval;
 
    for (let i = 0; i < campaigns.totalNumEntries; i++){   
        let campaign = campaigns.values[i].campaign;
         
        Logger.log('campaignId -> ' + campaign.campaignId + ', campaignName -> ' + campaign.campaignName);
    }
}
```

### キャンペーンを新規追加する / Add a campaign
```.js
function addCampaign() {
      
    const accountId = AdsUtilities.getCurrentAccountId();
      
    const campaigns = Search.CampaignService.add({
        "accountId": accountId,
        "operand": [
            {
                "biddingStrategyConfiguration": {
                    "biddingScheme": {
                        "biddingStrategyType": "MANUAL_CPC",
                        "manualCpcBiddingScheme": {
                            "enhancedCpcEnabled": "FALSE"
                        },
                    },
                },
                "budget": {
                    "amount": 1000,
                    "budgetPeriod": "DAILY"
                },
                "campaignName": "FFF",
                "type": "STANDARD",
                "userStatus": "ACTIVE",
            }
        ]
    }).rval;
      
    for (let i = 0; i < Object.keys(campaigns.values).length; i++){
        let campaign = campaigns.values[i].campaign;
          
        Logger.log('biddingStrategyType -> ' + campaign.biddingStrategyConfiguration.biddingScheme.biddingStrategyType
            + ', amount -> ' + campaign.budget.amount
            + ', budgetPeriod -> ' + campaign.budget.budgetPeriod
            + ', campaignId -> ' + campaign.campaignId
            + ', campaignName -> ' + campaign.campaignName
            + ', type -> ' + campaign.type);
    }
}
```

### キャンペーンを配信停止にする / Pause a campaign
```.js
function pauseCampaign() {
 
    const accountId = AdsUtilities.getCurrentAccountId();
     
    const campaignsGet = Search.CampaignService.get({
        "accountId": accountId,
        "campaignIds": [
            111111, 222222,//Multiple selections are possible
        ],
    }).rval;
 
    let campaignArray = [];
 
    for (let i = 0; i < campaignsGet.totalNumEntries; i++){   
        let campaign = campaignsGet.values[i].campaign;
         
        campaign.userStatus = "PAUSED";
         
        campaignArray.push(campaign);
    }
     
    const campaignsSet = Search.CampaignService.set({
        "accountId": accountId,
        "operand": campaignArray,
    }).rval;
     
    for (let i = 0; i < Object.keys(campaignsSet.values).length; i++){   
        let campaign = campaignsSet.values[i].campaign;
         
        Logger.log('campaignId -> ' + campaign.campaignId + ', userStatus -> ' + campaign.userStatus);
    }
}
```

### キャンペーン予算を更新する / Set campaign budget
```.js
function setCampaignBudget() {
     
    const accountId = AdsUtilities.getCurrentAccountId();
     
    const campaignsGet = Search.CampaignService.get({
        "accountId": accountId,
        "campaignIds": [
            926575,//Multiple selections are possible
        ],
    }).rval;
 
    let campaignArray = [];
 
    for (let i = 0; i < campaignsGet.totalNumEntries; i++){   
        let campaign = campaignsGet.values[i].campaign;
        campaign.budget.amount = 2000;
        campaignArray.push(campaign);
    }
     
    const campaignsSet = Search.CampaignService.set({
        "accountId": accountId,
        "operand": campaignArray,
    }).rval;
 
    for (let i = 0; i < Object.keys(campaignsSet.values).length; i++){   
        let campaign = campaignsSet.values[i].campaign;
        Logger.log('campaignId -> ' + campaign.campaignId + ', budgetAmount -> ' + campaign.budget.amount);
    }
}
```
