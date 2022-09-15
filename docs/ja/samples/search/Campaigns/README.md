# キャンペーン / Campaigns

### 全てのキャンペーン情報を取得する / Get all campaigns
```.js
function getAllCampaigns() {
     
  const accountId = AdsUtilities.getCurrentAccountId();
  
  const campaigns = Search.CampaignService.get({
    accountId: accountId,
    numberResults: 10000,//Max campaigns you can get is 10000.
  }).rval;
  
  if (campaigns.totalNumEntries == 0) {
    Logger.log('Target ID does not exist.');
    return;
  }

  for (let i = 0; i < Object.keys(campaigns.values).length; i++){   
    let campaign = campaigns.values[i].campaign;
    Logger.log('campaignId-> ' + campaign.campaignId + ', campaignName-> ' + campaign.campaignName);
  }
}
```

### 指定した全てのキャンペーン情報を取得する / Get a campaign by id
```.js
function getCampaignById() {
     
  const accountId = AdsUtilities.getCurrentAccountId();
  const campaignIds = [1111111, 2222222];//Multiple selections are possible
   
  const campaigns = Search.CampaignService.get({
    accountId: accountId,
    campaignIds: campaignIds,
  }).rval;
  
  if (campaigns.totalNumEntries == 0) {
    Logger.log('Target ID does not exist.');
    return;
  }

  for (let i = 0; i < Object.keys(campaigns.values).length; i++){   
    let campaign = campaigns.values[i].campaign;
    Logger.log('campaignId-> ' + campaign.campaignId + ', campaignName-> ' + campaign.campaignName);
  }
}
```

### キャンペーンを新規追加する / Add a campaign
```.js
function addCampaign() {
      
  const accountId = AdsUtilities.getCurrentAccountId();
  
  const campaignArray = [
    {
      biddingStrategyConfiguration: {
        biddingScheme: {
          biddingStrategyType: 'MANUAL_CPC',
        },
      },
      budget: {
        amount: 1000,
        budgetPeriod: 'DAILY',
      },
      campaignName: 'campaignNameAAA',
      userStatus: 'ACTIVE',
    },
    {
      biddingStrategyConfiguration: {
        biddingScheme: {
          biddingStrategyType: 'TARGET_SPEND',
        },
      },
      budget: {
        amount: 1000,
        budgetPeriod: 'DAILY',
      },
      campaignName: 'campaignNameBBB',
      userStatus: 'ACTIVE',
    },
    {
      biddingStrategyConfiguration: {
        biddingScheme: {
          biddingStrategyType: 'MAXIMIZE_CONVERSIONS',
          maximizeConversionsBiddingScheme: {
            targetCpa: 1000,//1-800000
          },
        },
      },
      budget: {
        amount: 1000,
        budgetPeriod: 'DAILY',
      },
      campaignName: 'campaignNameCCC',
      userStatus: 'ACTIVE',
    },
    {
      biddingStrategyConfiguration: {
        biddingScheme: {
          biddingStrategyType: 'MAXIMIZE_CONVERSION_VALUE',
          maximizeConversionValueBiddingScheme: {
            targetRoas: 1.0,//0.01-1000.00（1-100000%）
          },
        },
      },
      budget: {
        amount: 1000,
        budgetPeriod: 'DAILY',
      },
      campaignName: 'campaignNameDDD',
      userStatus: 'ACTIVE',
    },
    {
      biddingStrategyConfiguration: {
        biddingScheme: {
          biddingStrategyType: 'TARGET_IMPRESSION_SHARE',
          targetImpressionShareScheme: {
            location: 'ANYWHERE_ON_PAGE',
            bidCeiling: 1000,
            targetImpressionShare: 1.0,
          },
        },
      },
      budget: {
        amount: 1000,
        budgetPeriod: 'DAILY',
      },
      campaignName: 'campaignNameEEE',
      userStatus: 'ACTIVE',
    }
  ];//Multiple selections are possible
  
  const campaigns = Search.CampaignService.add({
    accountId: accountId,
    operand: campaignArray,
  }).rval;
    
  for (let i = 0; i < Object.keys(campaigns.values).length; i++){
    if (campaigns.values[i].operationSucceeded) {
      let campaign = campaigns.values[i].campaign;
      Logger.log('biddingStrategyType-> ' 
        + campaign.biddingStrategyConfiguration.biddingScheme.biddingStrategyType
        + ', campaignId-> ' + campaign.campaignId 
        + ', campaignName-> ' + campaign.campaignName + ' has been added.');
    
    } else {
      Logger.log('campaignName-> ' + campaignArray[i].campaignName 
        + ' could not be added.');

    }
  }
}
```

### キャンペーンを配信停止にする / Pause a campaign
```.js
function pauseCampaign() {
 
  const accountId = AdsUtilities.getCurrentAccountId();
  const campaignIds = [1111111, 2222222];//Empty when not specified
  
  const campaignsGet = Search.CampaignService.get({
    accountId: accountId,
    campaignIds: campaignIds,
    userStatuses: ['ACTIVE'],
  }).rval;

  if (campaignsGet.totalNumEntries == 0) {
    Logger.log('Target ID does not exist.');
    return;
  }

  let campaignArray = [];
  for (let i = 0; i < Object.keys(campaignsGet.values).length; i++){   
    let campaign = campaignsGet.values[i].campaign;
    campaign.userStatus = 'PAUSED';
    delete campaign.startDate;
    campaignArray.push(campaign);
  }
   
  const campaignsSet = Search.CampaignService.set({
    accountId: accountId,
    operand: campaignArray,
  }).rval;

  for (let i = 0; i < Object.keys(campaignsSet.values).length; i++){   
    if (campaignsSet.values[i].operationSucceeded) {
      let campaign = campaignsSet.values[i].campaign;
      Logger.log('campaignId-> ' + campaign.campaignId 
        + ', campaignName-> ' + campaign.campaignName + ' has been paused.');
      
    } else {
      let campaign = campaignsGet.values[i].campaign;
      Logger.log('campaignId-> ' + campaign.campaignId 
        + ', campaignName-> ' + campaign.campaignName + ' could not be stopped.');
      
    }
  }
}
```

### キャンペーン予算を更新する / Set campaign budget
```.js
function setCampaignBudget() {
     
  const accountId = AdsUtilities.getCurrentAccountId();
  const campaignIds = [1111111, 2222222];//Empty when not specified
  const budgetAmount = 1000;

  const campaignsGet = Search.CampaignService.get({
    accountId: accountId,
    campaignIds: campaignIds,
  }).rval;

  if (campaignsGet.totalNumEntries == 0) {
    Logger.log('Target ID does not exist.');
    return;
  }
  
  let campaignArray = [];
  for (let i = 0; i < Object.keys(campaignsGet.values).length; i++){   
    let campaign = campaignsGet.values[i].campaign;
    campaign.budget.amount = budgetAmount;
    delete campaign.startDate;
    campaignArray.push(campaign);
  }
   
  const campaignsSet = Search.CampaignService.set({
    accountId: accountId,
    operand: campaignArray,
  }).rval;

  for (let i = 0; i < Object.keys(campaignsSet.values).length; i++){
    if (campaignsSet.values[i].operationSucceeded) {
      let campaign = campaignsSet.values[i].campaign;
      Logger.log('campaignId-> ' + campaign.campaignId 
        + ', campaignName-> ' + campaign.campaignName
        + ' has been changed to budgetAmount-> ' + campaign.budget.amount);
      
    } else {
      let campaign = campaignsGet.values[i].campaign;
      Logger.log('campaignId-> ' + campaign.campaignId 
        + ', campaignName-> ' + campaign.campaignName 
        + ' budget could not be changed.');
      
    }
  } 
}
```
