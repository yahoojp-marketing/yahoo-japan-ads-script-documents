# プレイスメントリスト / Placement Lists

### プレイスメントリストとURLの新規追加をする / Add list and url
```.js
function addListAndUrl() {
  
  const accountId = AdsUtilities.getCurrentAccountId();
  const placementUrlListArray = [
    {
      accountId: accountId,
      urlListName: 'urlListNameAAA',
      urls: [
        {
          placementUrl: 'xxxxx.co.jp',
        }
      ]
    },
    {
      accountId: accountId,
      urlListName: 'urlListNameBBB',
      urls: [
        {
          placementUrl: 'yyyyy.co.jp',
        },
        {
          placementUrl: 'zzzzz.co.jp',
        }
      ]
    }
  ];//Multiple selections are possible

  const placementUrlLists = Display.PlacementUrlListService.add({
    accountId: accountId,
    operand: placementUrlListArray,
  }).rval;
 
  for (let i = 0; i < Object.keys(placementUrlLists.values).length; i++){
    if (placementUrlLists.values[i].operationSucceeded) {
      let urlList = placementUrlLists.values[i].urlList;
      for (let j = 0; j < urlList.urls.length; j++) {
        Logger.log('urlListId-> ' + urlList.urlListId
          + ', urlListName-> ' + urlList.urlListName
          + ', placementUrl-> ' + urlList.urls[j].placementUrl 
          + ' have been added.');
      }
      
    } else {
      Logger.log('urlListName-> ' + placementUrlListArray[i].urlListName 
        + ' could not to be added.');
      
    }
  }
}
```

### プレイスメントURLの更新をする / Set url
```.js
function setUrl() {
  
  const accountId = AdsUtilities.getCurrentAccountId();
  const urlListIds = [1111111111, 2222222222];//Multiple selections are possible
  const placementUrls = [
    {
      placementUrl: 'xxxxx.co.jp',
    },
    {
      placementUrl: 'yyyyy.co.jp',
    }
  ];//Multiple selections are possible

  const placementUrlListsGet = Display.PlacementUrlListService.get({
    accountId: accountId,
    urlListIds: urlListIds,
  }).rval;
  
  if (placementUrlListsGet.totalNumEntries == 0) {
    Logger.log('PlacementUrlList does not exist.');
    return;
  }
  
  let placementUrlListArray = [];
  for (let i = 0; i < Object.keys(placementUrlListsGet.values).length; i++){
    let urlList = placementUrlListsGet.values[i].urlList;
    urlList.urls = urlList.urls.concat(placementUrls);
    placementUrlListArray.push(urlList);
  }
     
  const placementUrlListsSet = Display.PlacementUrlListService.set({
    accountId: accountId,
    operand: placementUrlListArray,
  }).rval;
     
  for (let i = 0; i < Object.keys(placementUrlListsSet.values).length; i++) {
    if (placementUrlListsSet.values[i].operationSucceeded) {
      let urlList = placementUrlListsSet.values[i].urlList;
      for (let j = 0; j < urlList.urls.length; j++){
        Logger.log('urlListId-> ' + urlList.urlListId
          + ', urlListName-> ' + urlList.urlListName
          + ' have placementUrl-> ' + urlList.urls[j].placementUrl);
      }
      
    } else {
      let urlList = placementUrlListsGet.values[i].urlList;
      Logger.log('urlListId-> ' + urlList.urlListId
        + ', urlListName-> ' + urlList.urlListName + ' could not set.');
      
    }
  }
}
```

### プレイスメントリストとURLの情報を取得する / Get list and url
```.js
function getListAndUrl() {
  
  const accountId = AdsUtilities.getCurrentAccountId();
  const urlListIds = [1111111111, 2222222222];//Empty when not specified

  const placementUrlLists = Display.PlacementUrlListService.get({
    accountId: accountId,
    urlListIds: urlListIds,
  }).rval;
  
  if (placementUrlLists.totalNumEntries == 0) {
    Logger.log('PlacementUrlList does not exist.');
    return;
  }
 
  for (let i = 0; i < placementUrlLists.totalNumEntries; i++){
    let urlList = placementUrlLists.values[i].urlList;
    for (let j = 0; j < urlList.urls.length; j++){
      Logger.log('urlListId-> ' + urlList.urlListId
        + ', urlListName-> ' + urlList.urlListName
        + ', placementUrl-> ' + urlList.urls[j].placementUrl);
    }
  }
}
```

### 広告グループにプレイスメントリストを付与する / Apply a list to an ad group
```.js
function applyListToAdGroup() {
  
  const accountId = AdsUtilities.getCurrentAccountId();
  const adGroupTargetArray = [
    {
      adGroupId: 111111111,
      bidMultiplier: 1.5,
      campaignId: 22222222,
      target: {
        placementTarget: {
          placementUrlListType: 'WHITE_LIST',
        },
        targetId: 3333333333,//urlListId
        targetType: 'PLACEMENT_TARGET',
      }
    },
    {
      adGroupId: 444444444,
      bidMultiplier: 1.5,
      campaignId: 55555555,
      target: {
        placementTarget: {
          placementUrlListType: 'WHITE_LIST',
        },
        targetId: 6666666666,//urlListId
        targetType: 'PLACEMENT_TARGET',
      }
    }
  ];//Multiple selections are possible

  const adGroupTargets = Display.AdGroupTargetService.add({
    accountId: accountId,
    operand: adGroupTargetArray,
  }).rval;

  for (let i = 0; i < Object.keys(adGroupTargets.values).length; i++) {
    if (adGroupTargets.values[i].operationSucceeded) {
      let adGroupTargetList = adGroupTargets.values[i].adGroupTargetList;
      let target = adGroupTargetList.target;
      Logger.log('adGroupId-> ' + adGroupTargetList.adGroupId
        + ', campaignId-> ' + adGroupTargetList.campaignId
        + ' linked to placementUrlListType-> ' + target.placementTarget.placementUrlListType
        + ', placementUrlListName-> ' + target.placementTarget.placementUrlListName
        + ', targetId-> ' + target.targetId
        + ', targetType-> ' + target.targetType
        + ', bidMultiplier-> ' + adGroupTargetList.bidMultiplier);

    } else {
      let target = adGroupTargetArray[i].target;
      Logger.log('adGroupId-> ' + adGroupTargetArray[i].adGroupId
        + ', campaignId-> ' + adGroupTargetArray[i].campaignId
        + ' could not link to placementUrlListType-> ' + target.placementTarget.placementUrlListType
        + ', targetId-> ' + target.targetId
        + ', targetType-> ' + target.targetType
        + ', bidMultiplier-> ' + adGroupTargetArray[i].bidMultiplier);
        
    }
  }
}
```
