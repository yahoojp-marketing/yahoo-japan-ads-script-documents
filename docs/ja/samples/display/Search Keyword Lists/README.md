# サーチキーワードリスト / Search Keyword Lists

### サーチキーワードリストとキーワードを新規追加をする / Add list and keyword
```.js
function addListAndKeyword() {
  
  const accountId = AdsUtilities.getCurrentAccountId();
  const searchKeywordListArray = [
    {
      accountId: accountId,
      searchKeyword: [
        {
          searchKeywordId: 1111111111,//Get in SearchKeywordIdeaService
        }
      ],
      searchKeywordListName: 'listNameAAA',
    },
    {
      accountId: accountId,
      searchKeyword: [
        {
          searchKeywordId: 2222222222,
        },
        {
          searchKeywordId: 3333333333,
        }
      ],
      searchKeywordListName: 'listNameBBB',
    }
  ];//Multiple selections are possible

  const searchKeywordLists = Display.SearchKeywordListService.add({
    accountId: accountId,
    operand: searchKeywordListArray,
  }).rval;
 
  for (let i = 0; i < Object.keys(searchKeywordLists.values).length; i++) {
    if (searchKeywordLists.values[i].operationSucceeded) {
      let searchKeywordList = searchKeywordLists.values[i].searchKeywordList;
      
      for (let j = 0; j < searchKeywordList.searchKeyword.length; j++) {
        let  searchKeyword = searchKeywordList.searchKeyword;
        Logger.log('searchKeywordId-> ' + searchKeywordList.searchKeyword[j].searchKeywordId
          + ' be added to searchKeywordListId-> ' + searchKeywordList.searchKeywordListId
          + ', searchKeywordListName-> ' + searchKeywordList.searchKeywordListName);
      }
      
    } else {
      for (let j = 0; j < searchKeywordListArray[i].searchKeyword.length; j++) {
        Logger.log('searchKeywordId-> ' + searchKeywordListArray[i].searchKeyword[j].searchKeywordId
          + ' could not to be added to searchKeywordListName-> ' 
          + searchKeywordListArray[i].searchKeywordListName);
      }
      
    }
  }
}
```

### キーワードの更新をする / Set keyword
```.js
function setKeyword() {
  
  const accountId = AdsUtilities.getCurrentAccountId();
  const searchKeywordListIds = [1111111111, 2222222222];//Empty when not specified
  const searchKeywordIds = [3333333333, 4444444444, 5555555555];//Multiple selections are possible

  const searchKeywordListsGet = Display.SearchKeywordListService.get({
    accountId: accountId,
    searchKeywordListIds: searchKeywordListIds,
  }).rval;

  if (searchKeywordListsGet.totalNumEntries == 0) {
    Logger.log('SearchKeywordListId does not exist.');
    return;
  }
  
  let searchKeywordIdsArray = [];
  for (let i = 0; i < searchKeywordIds.length; i++) {
    searchKeywordIdsArray.push({searchKeywordId: searchKeywordIds[i]});
  }
  
  let searchKeywordListArray = [];
  for (let i = 0; i < Object.keys(searchKeywordListsGet.values).length; i++){
    let searchKeywordList = searchKeywordListsGet.values[i].searchKeywordList;
    searchKeywordList.searchKeyword = searchKeywordIdsArray;
    searchKeywordListArray.push(searchKeywordList);
  }

  const searchKeywordListsSet = Display.SearchKeywordListService.set({
    accountId: accountId,
    operand: searchKeywordListArray,
  }).rval;
  
  for (let i = 0; i < Object.keys(searchKeywordListsSet.values).length; i++) {
    if (searchKeywordListsSet.values[i].operationSucceeded) {
      let searchKeywordList = searchKeywordListsSet.values[i].searchKeywordList;
      
      for (let j = 0; j < searchKeywordList.searchKeyword.length; j++) {
        Logger.log('searchKeywordId-> ' + searchKeywordList.searchKeyword[j].searchKeywordId
          + ' be added to searchKeywordListId-> ' + searchKeywordList.searchKeywordListId
          + ', searchKeywordListName-> ' + searchKeywordList.searchKeywordListName);    
      }
      
    } else {
      let searchKeywordList = searchKeywordListsGet.values[i].searchKeywordList;
      Logger.log('searchKeywordId-> ' + searchKeywordIds.join(', ')
        + ' could not to be added to searchKeywordListId-> ' + searchKeywordList.searchKeywordListId
        + ', searchKeywordListName-> ' + searchKeywordList.searchKeywordListName);    
      
    }
  }
}
```

### サーチキーワードリストとキーワード情報の取得をする / Get list and keyword
```.js
function getListAndKeyword() {
  
  const accountId = AdsUtilities.getCurrentAccountId();

  const searchKeywordLists = Display.SearchKeywordListService.get({
    accountId: accountId,
  }).rval;
  
  if (searchKeywordLists.totalNumEntries == 0) {
    Logger.log('SearchKeywordList does not exist.');
    return;
  }

  for (let i = 0; i < Object.keys(searchKeywordLists.values).length; i++) {
    let searchKeywordList = searchKeywordLists.values[i].searchKeywordList;
    
    for (let j = 0; j < searchKeywordList.searchKeyword.length; j++) {
      Logger.log('searchKeywordId-> ' + searchKeywordList.searchKeyword[j].searchKeywordId
        + ', searchKeywordListId-> ' + searchKeywordList.searchKeywordListId
        + ', searchKeywordListName-> ' + searchKeywordList.searchKeywordListName);
    }
  }
}
```

### 広告グループにサーチキーワードリストを付与する / Apply a list to an ad group
```.js
function applyListToAdGroupSerchKeywordList() {
  
  const accountId = AdsUtilities.getCurrentAccountId();
  const adGroupTargetArray = [
    {
      adGroupId: 111111111,
      campaignId: 22222222,
      target: {
        targetId: 3333333333,//searchKeywordListId
        targetType: 'SEARCH_TARGET',
      }
    },
    {
      adGroupId: 444444444,
      bidMultiplier: 1.5,
      campaignId: 55555555,
      target: {
        targetId: 6666666666,
        targetType: 'SEARCH_TARGET',
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
      Logger.log('adGroupId-> ' + adGroupTargetList.adGroupId
        + ', campaignId-> ' + adGroupTargetList.campaignId
        + ' be added searchKeywordListName-> ' + adGroupTargetList.target.searchTarget.searchKeywordListName
        + ', targetId-> ' + adGroupTargetList.target.targetId
        + ', targetType-> ' + adGroupTargetList.target.targetType
        + ', bidMultiplier-> ' + adGroupTargetList.bidMultiplier);
        
    } else {
      Logger.log('adGroupId-> ' + adGroupTargetArray[i].adGroupId
        + ', campaignId-> ' + adGroupTargetArray[i].campaignId
        + ' could not to be added targetId-> ' + adGroupTargetArray[i].target.targetId
        + ', targetType-> ' + adGroupTargetArray[i].target.targetType);
      
    }
  }
}
```
