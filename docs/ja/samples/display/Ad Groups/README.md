# 広告グループ / Ad Groups

### 広告グループを新規追加する / Add an ad group
```.js
function addAdGroup() {
  
  const accountId = AdsUtilities.getCurrentAccountId();
  const adGroupArray = [
    {
      accountId: accountId,
      adGroupName: 'adGroupAAA',
      campaignId: 11111111,
      device: ['DESKTOP'],
      userStatus: 'ACTIVE',
    },
    {
      accountId: accountId,
      adGroupName: 'adGroupBBB',
      campaignId: 22222222,
      device: ['SMARTPHONE', 'TABLET'],
      deviceApp: ['APP'],
      deviceOs: ['NONE'],
      userStatus: 'ACTIVE',
    },
    {
      accountId: accountId,
      adGroupName: 'adGroupCCC',
      campaignId: 33333333,
      device: ['NONE'],
      deviceApp: ['NONE'],
      deviceOs: ['NONE'],
      userStatus: 'ACTIVE',
    }
  ];//Multiple selections are possible
  
  const adGroups = Display.AdGroupService.add({
    accountId: accountId,
    operand: adGroupArray,
  }).rval;
     
  for (let i = 0; i < Object.keys(adGroups.values).length; i++){
    if (adGroups.values[i].operationSucceeded) {
      let adGroup = adGroups.values[i].adGroup;
      Logger.log('adGroupId-> ' + adGroup.adGroupId + ', adGroupName-> ' + adGroup.adGroupName
        + ' have been added as device-> ' + adGroup.device.join(', ') + ' to campaignId-> ' + adGroup.campaignId
        + ' campaignName-> ' + adGroup.campaignName);
        
    } else {
      Logger.log('adGroupName-> ' + adGroupArray[i].adGroupName
        + ' could not to be added to campaignId-> ' + adGroupArray[i].campaignId);
    }
  }
}
```

### 広告グループを配信停止にする / Pause an ad group
```.js
function pauseAdGroup() {
  
  const accountId = AdsUtilities.getCurrentAccountId();
  const adGroupIds = [111111111, 222222222, 333333333];//Empty when not specified
  
  const adGroupsGet = Display.AdGroupService.get({
    accountId: accountId,
    adGroupIds: adGroupIds,
  }).rval;
  
  if (adGroupsGet.totalNumEntries == 0) {
    Logger.log('Target ID does not exist.');
    return;
  }
  
  let adGroupsArray = [];
  for (let i = 0; i < Object.keys(adGroupsGet.values).length; i++){
    let adGroup = adGroupsGet.values[i].adGroup;
    adGroup.userStatus = 'PAUSED';
    adGroupsArray.push(adGroup);
  }
  
  const adGroupsSet = Display.AdGroupService.set({
    accountId: accountId,
    operand: adGroupsArray,
  }).rval;
  
  for (let i = 0; i < Object.keys(adGroupsSet.values).length; i++){
    if (adGroupsSet.values[i].operationSucceeded) {
      let adGroup = adGroupsSet.values[i].adGroup;
      Logger.log('adGroupId-> ' + adGroup.adGroupId + ', adGroupName-> ' + adGroup.adGroupName + ' have paused.');
        
    } else {
      let adGroup = adGroupsSet.values[i].adGroup;
      Logger.log('adGroupId-> ' + adGroup.adGroupId + ', adGroupName-> ' + adGroup.adGroupName
        + ' could not to be paused.');
      
    }
  }
}
```

### 広告グループの入札価格を変更する / Set ad group bid
```.js
function setAdGroupBid() {
  
  const accountId = AdsUtilities.getCurrentAccountId();
  const adGroupIds = [111111111, 222222222, 333333333];//Empty when not specified
  const bid = 3000;
  
  const adGroupsGet = Display.AdGroupService.get({
    accountId: accountId,
    adGroupIds: adGroupIds,
  }).rval;

  if (adGroupsGet.totalNumEntries == 0) {
    Logger.log('Target ID does not exist.');
    return;
  }
  
  let adGroupsArray = [];
  for (let i = 0; i < Object.keys(adGroupsGet.values).length; i++){
    let adGroup = adGroupsGet.values[i].adGroup;
    let type = adGroup.adGroupBiddingStrategy.campaignBiddingStrategyType;
    
    delete adGroup.adGroupBiddingStrategy;
    
    switch (type) {
      case 'MAX_VCPM':
        adGroup.adGroupBiddingStrategy = {
          campaignBiddingStrategyType: type,
          maxVcpmBidValue: bid,
        };
        break;
      case 'MAX_CPC':
        adGroup.adGroupBiddingStrategy = {
          campaignBiddingStrategyType: type,
          maxCpcBidValue: bid,
        };
        break;
      case 'MAX_CPV':
        adGroup.adGroupBiddingStrategy = {
          campaignBiddingStrategyType: type,
          maxCpvBidValue: bid,
        };
        break;
      case 'TARGET_CPA':
        adGroup.adGroupBiddingStrategy = {
          campaignBiddingStrategyType: type,
          targetCpaBidValue: bid,
        };
        break;
      default:
        continue;
    }
    
    adGroupsArray.push(adGroup);
  }
  
  if (adGroupsArray.length == 0) {
    Logger.log('Target ID does not exist.');
    return;
  }
  
  const adGroupsSet = Display.AdGroupService.set({
    accountId: accountId,
    operand: adGroupsArray,
  }).rval;
  
  for (let i = 0; i < Object.keys(adGroupsSet.values).length; i++){
    if (adGroupsSet.values[i].operationSucceeded) {
      let adGroup = adGroupsSet.values[i].adGroup;
      let type = adGroup.adGroupBiddingStrategy.campaignBiddingStrategyType;
      let bidValue;
      
      switch (type) {
        case 'MAX_VCPM':
          bidValue = adGroup.adGroupBiddingStrategy.maxVcpmBidValue;
          break;
        case 'MAX_CPC':
          bidValue = adGroup.adGroupBiddingStrategy.maxCpcBidValue;
          break;
        case 'MAX_CPV':
          bidValue = adGroup.adGroupBiddingStrategy.maxCpvBidValue;
          break;
        case 'TARGET_CPA':
          bidValue = adGroup.adGroupBiddingStrategy.targetCpaBidValue;
          break;
        default:
          break;
      }
      
      Logger.log('adGroupId-> ' + adGroup.adGroupId + ', adGroupName-> ' + adGroup.adGroupName
        + ' set as campaignBiddingStrategyType-> ' + type + ' to bid-> ' + bidValue);
        
    } else {
      let adGroup = adGroupsGet.values[i].adGroup;
      Logger.log('adGroupId-> ' + adGroup.adGroupId + ', adGroupName-> ' + adGroup.adGroupName
        + ' could not to be set to bid-> ' + bid);
        
    }
  }
}
```

### アカウント配下の全ての広告グループ情報を取得 / Get all ad group 
```.js
function getAllAdGroup() {

  const accountId = AdsUtilities.getCurrentAccountId();
  
  const adGroups = Display.AdGroupService.get({
    accountId: accountId,
  }).rval;

  if (adGroups.totalNumEntries == 0) {
    Logger.log('Target ID does not exist.');
    return;
  }
  
  for (let i = 0; i < Object.keys(adGroups.values).length; i++){
    let adGroup = adGroups.values[i].adGroup;
    Logger.log('adGroupId-> ' + adGroup.adGroupId + ', adGroupName-> ' + adGroup.adGroupName
      + ', campaignId-> ' + adGroup.campaignId + ', campaignName-> ' + adGroup.campaignName);
  }
}
```

### 指定した全ての広告グループ情報を取得する / Get all ad group by id
```.js
function getAllAdGroupById() {

  const accountId = AdsUtilities.getCurrentAccountId();
  const adGroupIds = [111111111, 222222222, 333333333];//Multiple selections are possible
  
  const adGroups = Display.AdGroupService.get({
    accountId: accountId,
    adGroupIds: adGroupIds,
  }).rval;

  if (adGroups.totalNumEntries == 0) {
    Logger.log('Target ID does not exist.');
    return;
  }
  
  for (let i = 0; i < Object.keys(adGroups.values).length; i++){
    let adGroup = adGroups.values[i].adGroup;
    Logger.log('adGroupId-> ' + adGroup.adGroupId + ', adGroupName-> ' + adGroup.adGroupName
      + ', campaignId-> ' + adGroup.campaignId + ', campaignName-> ' + adGroup.campaignName);
  }
}
```

