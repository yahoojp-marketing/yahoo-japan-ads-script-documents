# キャンペーン / Campaigns

### 全てのキャンペーン情報の取得をする / Get all campaigns
```.js
function getAllCampaigns() {
 
  const accountId = AdsUtilities.getCurrentAccountId();
     
  const campaigns = Display.CampaignService.get({
    accountId: accountId,
  }).rval;
  
  if (campaigns.totalNumEntries == 0) {
    Logger.log('Campaign does not exist.');
    return;
  }
  
  for (let i = 0; i < Object.keys(campaigns.values).length; i++){
    let campaign = campaigns.values[i].campaign;
    Logger.log('campaignId -> ' + campaign.campaignId
      + ', campaignName -> ' + campaign.campaignName);
  }
}
```

### 指定のキャンペーン情報の取得をする / Get a campaign by id
```.js
function getCampaignById() {
 
  const accountId = AdsUtilities.getCurrentAccountId();
  const campaignIds = [11111111, 22222222, 33333333];//Multiple selections are possible
  
  const campaigns = Display.CampaignService.get({
    accountId: accountId,
    campaignIds: campaignIds,
  }).rval;

  if (campaigns.totalNumEntries == 0) {
    Logger.log('Campaign does not exist.');
    return;
  }
  
  for (let i = 0; i < Object.keys(campaigns.values).length; i++){
    let campaign = campaigns.values[i].campaign;
    Logger.log('campaignId -> ' + campaign.campaignId 
      + ', campaignName -> ' + campaign.campaignName);
  }
}
```

### キャンペーンの新規追加をする / Add a campaign
```.js
function addCampaign() {
 
  const accountId = AdsUtilities.getCurrentAccountId();
  const campaignArray = [
    {
      accountId: accountId,
      budget: {
        amount: 1000,
      },
      campaignBiddingStrategy: {
        campaignBiddingStrategyType: 'MAXIMIZE_CONVERSIONS',
      },
      campaignGoal: 'CONVERSION',
      campaignName: 'campaignAAA',
      userStatus: 'ACTIVE',
    },
    {
      accountId: accountId,
      budget: {
        amount: 2000,
      },
      campaignBiddingStrategy: {
        campaignBiddingStrategyType: 'MAXIMIZE_CLICKS',
      },
      campaignGoal: 'WEBSITE_TRAFFIC',
      campaignName: 'campaignBBB',
      userStatus: 'ACTIVE',
    },
    {
      accountId: accountId,
      budget: {
        amount: 3000,
      },
      campaignBiddingStrategy: {
        campaignBiddingStrategyType: 'MAXIMIZE_VIEW',
      },
      campaignGoal: 'VIDEO_VIEW',
      campaignName: 'campaignCCC',
      userStatus: 'ACTIVE',
    },
    {
      accountId: accountId,
      budget: {
        amount: 4000,
      },
      campaignBiddingStrategy: {
        campaignBiddingStrategyType: 'MAX_CPC',
        maxCpcBidValue: 1000,
      },
      campaignGoal: 'WEBSITE_TRAFFIC',
      campaignName: 'campaignDDD',
      userStatus: 'ACTIVE',
    },
    {
      accountId: accountId,
      budget: {
        amount: 5000,
      },
      campaignBiddingStrategy: {
        campaignBiddingStrategyType: 'TARGET_CPA',
        targetCpaBidValue: 1000,
      },
      campaignGoal: 'CONVERSION',
      campaignName: 'campaignEEE',
      userStatus: 'ACTIVE',
    }
  ];//Multiple selections are possible
  
  const campaigns = Display.CampaignService.add({
    accountId: accountId,
    operand: campaignArray,
  }).rval;
     
  for (let i = 0; i < Object.keys(campaigns.values).length; i++){
    if (campaigns.values[i].operationSucceeded) {
      let campaign = campaigns.values[i].campaign;
      Logger.log('campaignId-> ' + campaign.campaignId
        + ', campaignName-> ' + campaign.campaignName
        + ' be added as amount -> ' + campaign.budget.amount
        + ', campaignType -> ' + campaign.campaignBiddingStrategy.campaignBiddingStrategyType
        + ', campaignGoal -> ' + campaign.campaignGoal);
      
    } else {
      Logger.log('campaignName-> ' + campaignArray[i].campaignName
        + ' could not to added as amount-> ' + campaignArray[i].budget.amount
        + ', campaignType-> ' + campaignArray[i].campaignBiddingStrategy.campaignBiddingStrategyType
        + ', campaignGoal-> ' + campaignArray[i].campaignGoal);
        
    }
  }
}
```

### キャンペーンを配信停止にする / Pause a campaign
```.js
function pauseCampaign() {
  
  const accountId = AdsUtilities.getCurrentAccountId();
  const campaignIds = [11111111, 22222222, 33333333];//Empty when not specified
  
  const campaignsGet = Display.CampaignService.get({
    accountId: accountId,
    campaignIds: campaignIds,
  }).rval;
  
  let campaignsArray = [];
  for (let i = 0; i < Object.keys(campaignsGet.values).length; i++){
    let campaign = campaignsGet.values[i].campaign;
    campaign.userStatus = 'PAUSED'; 
    campaignsArray.push(campaign);
  }
  
  const campaignsSet = Display.CampaignService.set({
    accountId: accountId,
    operand: campaignsArray,
  }).rval;
  
  for (let i = 0; i < Object.keys(campaignsSet.values).length; i++){
    if (campaignsSet.values[i].operationSucceeded) {
      let campaign = campaignsSet.values[i].campaign;
      Logger.log('campaignId-> ' + campaign.campaignId
        + ', campaignName-> ' + campaign.campaignName + ' have been stopped.');
      
    } else {
      let campaign = campaignsGet.values[i].campaign;
      Logger.log('campaignId-> ' + campaign.campaignId
        + ', campaignName-> ' + campaign.campaignName + ' could not to be stopped.');
        
    }
  }
}
```

### キャンペーン予算の更新をする / Set campaign budget
```.js
function setCampaignBudget(){
  
  const accountId = AdsUtilities.getCurrentAccountId();
  const campaignIds = [11111111, 22222222, 33333333];//Empty when not specified
  
  const campaignsGet = Display.CampaignService.get({
    accountId: accountId,
    campaignIds: campaignIds,
  }).rval;
  
  let campaignsArray = [];
  for (let i = 0; i < Object.keys(campaignsGet.values).length; i++){
    let campaign = campaignsGet.values[i].campaign;
    campaign.budget.amount = 3000;
    campaignsArray.push(campaign);
  }
  
  const campaignsSet = Display.CampaignService.set({
    accountId: accountId,
    operand: campaignsArray,
  }).rval;
  
  for (let i = 0; i < Object.keys(campaignsSet.values).length; i++){
    if (campaignsSet.values[i].operationSucceeded) {
      let campaign = campaignsSet.values[i].campaign;
      Logger.log('campaignId-> ' + campaign.campaignId
        + ', campaignName-> ' + campaign.campaignName
        + ' set amount-> ' + campaign.budget.amount);
        
    } else {
      let campaign = campaignsGet.values[i].campaign;
      Logger.log('campaignId-> ' + campaign.campaignId
        + ', campaignName-> ' + campaign.campaignName
        + ' could not set amount-> ' + campaign.budget.amount);
        
    }
  }
}
``` 

