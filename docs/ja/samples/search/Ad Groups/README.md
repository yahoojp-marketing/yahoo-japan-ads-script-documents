# 広告グループ / Ad Groups

### 広告グループを新規追加する / Add an ad group
```.js
function addAdGroup(){
     
  const accountId = AdsUtilities.getCurrentAccountId();

  const adGroupArray = [
    {
      adGroupName: 'adGroupNameAAA',
      bid: {
        bidSource: 'ADGROUP',
        maxCpc: 1000,//default:1
      },
      campaignId: 1111111,
      userStatus: 'ACTIVE',
    }
  ];//Multiple selections are possible
  
  const adGroups = Search.AdGroupService.add({
    accountId: accountId,
    operand: adGroupArray,
  }).rval;

  for (let i = 0; i < Object.keys(adGroups.values).length; i++) {
    if (adGroups.values[i].operationSucceeded) {
      let adGroup = adGroups.values[i].adGroup;
      Logger.log('adGroupId-> ' + adGroup.adGroupId + ', adGroupName-> ' + adGroup.adGroupName
        + ', bidMaxCpc-> ' + adGroup.bid.maxCpc + ' has been added.');
      
    } else {
      Logger.log('adGroupName-> ' + adGroupArray[i].adGroupName + ' could not be added.');

    }
  }
}
```

### 広告グループを配信停止にする / Pause an ad group
```.js
function pauseAdGroup(){
     
  const accountId = AdsUtilities.getCurrentAccountId();
  const adGroupIds = [111111111, 222222222];//Empty when not specified
  
  const adGroupsGet = Search.AdGroupService.get({
    accountId: accountId,
    adGroupIds: adGroupIds,
    userStatuses: ['ACTIVE'],
  }).rval;
  
  if (adGroupsGet.totalNumEntries == 0) {
    Logger.log('Target ID does not exist.');
    return;
  }
  
  let adGroupArray = [];
  for (let i = 0; i < Object.keys(adGroupsGet.values).length; i++) {
    let adGroup = adGroupsGet.values[i].adGroup;
    adGroup.userStatus = 'PAUSED';
    adGroupArray.push(adGroup);
  }
  
  const adGroupsSet = Search.AdGroupService.set({
    accountId: accountId,
    operand: adGroupArray,
  }).rval;
   
  for (let i = 0; i < Object.keys(adGroupsSet.values).length; i++) {
    if (adGroupsSet.values[i].operationSucceeded) {
      let adGroup = adGroupsSet.values[i].adGroup;
      Logger.log('adGroupId-> ' + adGroup.adGroupId 
        + ', adGroupName-> ' + adGroup.adGroupName + ' has been paused.');
      
    } else {
      Logger.log('adGroupName-> ' + adGroupsGet.values[i].adGroup.adGroupName 
        + ' could not be stopped.');
      
    }
  }
}
```

### 広告グループの入札価格を更新する / Set ad group bid
```.js
function setAdGroupBid(){
  
  const accountId = AdsUtilities.getCurrentAccountId();
  const adGroupIds = [111111111, 222222222];//Empty when not specified
  const bidMaxCpc = 500;
  
  const adGroupsGet = Search.AdGroupService.get({
    accountId: accountId,
    adGroupIds: adGroupIds,
  }).rval;
  
  if (adGroupsGet.totalNumEntries == 0) {
    Logger.log('Target ID does not exist.');
    return;
  }
  
  let adGroupArray = [];
  for (let i = 0; i < Object.keys(adGroupsGet.values).length; i++) {
    let adGroup = adGroupsGet.values[i].adGroup;
    adGroup.bid.maxCpc = bidMaxCpc;
    adGroupArray.push(adGroup);
  }
  
  const adGroupsSet = Search.AdGroupService.set({
    accountId: accountId,
    operand: adGroupArray,
  }).rval;
   
  for (let i = 0; i < Object.keys(adGroupsSet.values).length; i++) {
    if (adGroupsSet.values[i].operationSucceeded) {
      let adGroup = adGroupsSet.values[i].adGroup;
      Logger.log('adGroupId-> ' + adGroup.adGroupId 
        + ', adGroupName-> ' + adGroup.adGroupName
        + ' has been changed to budgetAmount-> ' + adGroup.bid.maxCpc);
      
    } else {
      Logger.log('adGroupName-> ' + adGroupsGet.values[i].adGroup.adGroupName 
        + ' budget could not be changed.');
      
    }
  }
}
```

### アカウント配下の全ての広告グループ情報を取得する / Get all ad group
```.js
function getAllAdGroup(){
  
  const accountId = AdsUtilities.getCurrentAccountId();
  
  const adGroups = Search.AdGroupService.get({
    accountId: accountId,
    numberResults: 10000,//Max adGroups you can get is 10000.
  }).rval;
  
  if (adGroups.totalNumEntries == 0) {
    Logger.log('Ad group does not exist.');
    return;
  }
  
  for (let i = 0; i < Object.keys(adGroups.values).length; i++) {
    let adGroup = adGroups.values[i].adGroup;
    Logger.log('adGroupId-> ' + adGroup.adGroupId 
      + ', adGroupName-> ' + adGroup.adGroupName);
  }
}
```

### 指定した全ての広告グループ情報を取得する / Get all ad group by id
```.js
function getAllAdGroupById(){
  
  const accountId = AdsUtilities.getCurrentAccountId();
  const adGroupIds = [111111111, 222222222];//Multiple selections are possible
  
  const adGroups = Search.AdGroupService.get({
    accountId: accountId,
    adGroupIds: adGroupIds,
  }).rval;
  
  if (adGroups.totalNumEntries == 0) {
    Logger.log('Target ID does not exist.');
    return;
  }
  
  for (let i = 0; i < Object.keys(adGroups.values).length; i++) {
    let adGroup = adGroups.values[i].adGroup;
    Logger.log('adGroupId-> ' + adGroup.adGroupId 
      + ', adGroupName-> ' + adGroup.adGroupName);
  }
}
```
