# Campaigns

### Get all campaigns
```$xslt
function getAllCampaigns(){
 
    const accountId = AdsUtilities.getCurrentAccountId();
     
    const campaigns = Display.CampaignService.get({
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
function getCampaignById(){
 
    const accountId = AdsUtilities.getCurrentAccountId();
     
    const campaigns = Display.CampaignService.get({
        "accountId": accountId,
        "campaignIds": [
                19881250, 19881249,//Multiple selections are possible
            ]
    }).rval;
     
    for (let i = 0; i < campaigns.totalNumEntries; i++){
        let campaign = campaigns.values[i].campaign;
         
        Logger.log('campaignId -> ' + campaign.campaignId + ', campaignName -> ' + campaign.campaignName);
    }
}
```

### Add a campaign
```$xslt
function addCampaign(){
 
    const accountId = AdsUtilities.getCurrentAccountId();
     
    const campaigns = Display.CampaignService.add({
        "accountId": accountId,
        "operand": [
            {
                "accountId": accountId,
                "budget": {
                    "amount": 2000,
                    "budgetDeliveryMethod": "STANDARD"
                },
                "campaignBiddingStrategy": {
                    "campaignBiddingStrategyType": "MAX_CPC",
                    "maxCpcBidValue": 1000,
                },
                "campaignGoal": "WEBSITE_TRAFFIC",
                "campaignName": "BBBBBB",
                "userStatus": "ACTIVE",
            }
        ]
    }).rval;
     
    for (let i = 0; i < Object.keys(campaigns.values).length; i++){
        let campaign = campaigns.values[i].campaign;
         
        Logger.log('campaignId -> ' + campaign.campaignId
            + ', campaignName -> ' + campaign.campaignName
            + ', budgetAmount -> ' + campaign.budget.amount
            + ', budgetDeliveryMethod -> ' + campaign.budget.budgetDeliveryMethod
            + ', campaignGoal -> ' + campaign.campaignGoal);
    }
}
```

### Pause a campaign
```$xslt
function pauseCampaign(){
 
    const accountId = AdsUtilities.getCurrentAccountId();
     
    const campaignsGet = Display.CampaignService.get({
        "accountId": accountId,
    }).rval;
 
    let campaignsArray = [];
     
    for (let i = 0; i < campaignsGet.totalNumEntries; i++){
        let campaign = campaignsGet.values[i].campaign;
         
        campaign.userStatus = "PAUSED"; 
        campaign.conversionOptimizer.conversionOptimizerType = null;//Because it cannot be set when it is SET and has a "campaignGoal"
         
        campaignsArray.push(campaign);
    }
     
    const campaignsSet = Display.CampaignService.set({
        "accountId": accountId,
        "operand": campaignsArray,
    }).rval;
     
    for (let i = 0; i < Object.keys(campaignsSet.values).length; i++){
        let campaign = campaignsSet.values[i].campaign;
         
        Logger.log('campaignId-> ' + campaign.campaignId + ', userStatus-> ' + campaign.userStatus);
    }
}
```

### Set campaign budget
```$xslt
function setCampaignBudget(){
 
    const accountId = AdsUtilities.getCurrentAccountId();
     
    const campaignsGet = Display.CampaignService.get({
        "accountId": accountId,
    }).rval;
 
    let campaignsArray = [];
     
    for (let i = 0; i < campaignsGet.totalNumEntries; i++){
        let campaign = campaignsGet.values[i].campaign;
         
        campaign.budget.amount = 3000;
        campaign.conversionOptimizer.conversionOptimizerType = null;//Because it cannot be set when it is SET and has a "campaignGoal"
         
        campaignsArray.push(campaign);
    }
     
    const campaignsSet = Display.CampaignService.set({
        "accountId": accountId,
        "operand": campaignsArray,
    }).rval;
     
    for (let i = 0; i < Object.keys(campaignsSet.values).length; i++){
        let campaign = campaignsSet.values[i].campaign;
         
        Logger.log('campaignId-> ' + campaign.campaignId + ', budgetAmount-> ' + campaign.budget.amount);
    }
}
``` 

