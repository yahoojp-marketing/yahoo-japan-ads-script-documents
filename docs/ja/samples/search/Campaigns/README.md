# Campaigns

### Get all campaigns
```$xslt
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

### Get a campaign by id
```$xslt
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

### Add a campaign
```$xslt
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

### Pause a campaign
```$xslt
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

### Set campaign budget
```$xslt
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
