# プレイスメントリスト / Placement Lists

### プレイスメントリストとURLの新規追加をする / Add list and url
```.js
function addListAndUrl(){
     
    const accountId = AdsUtilities.getCurrentAccountId();
 
    const placementUrlLists = Display.PlacementUrlListService.add({
        "accountId": accountId,
        "operand": [
            {
                "accountId": accountId,
                "urlListName": "AAA",
                "urls": [
                    {
                        "placementUrl": "yahoo.co.jp",
                    }
                ]
            }
        ]
    }).rval;
 
    for (let i = 0; i < Object.keys(placementUrlLists.values).length; i++){
        let urlList = placementUrlLists.values[i].urlList;
         
        for (let j = 0; j < urlList.urls.length; j++){
            Logger.log('urlListId -> ' + urlList.urlListId
                + ', urlListName -> ' + urlList.urlListName
                + ', placementUrl -> ' + urlList.urls[j].placementUrl);
        }
    }
}
```

### プレイスメントURLの更新をする / Set url
```.js
function setUrl(){
     
    const accountId = AdsUtilities.getCurrentAccountId();
 
    const placementUrlListsGet = Display.PlacementUrlListService.get({
        "accountId": accountId,
        "urlListIds": [
          1000038400, 1000038360,//Multiple selections are possible
        ],
    }).rval;
     
    let placementUrlListArray = [];
 
    for (let i = 0; i < Object.keys(placementUrlListsGet.values).length; i++){
        let urlList = placementUrlListsGet.values[i].urlList;
         
        urlList.urls.push({
          "placementUrl": "news.yahoo.co.jp",
          "urlActiveFlg": "ACTIVE",
        });
         
        placementUrlListArray.push(urlList);
    }
     
    const placementUrlListsSet = Display.PlacementUrlListService.set({
        "accountId": accountId,
        "operand": placementUrlListArray,
    }).rval;
     
    for (let i = 0; i < Object.keys(placementUrlListsSet.values).length; i++){
        let urlList = placementUrlListsSet.values[i].urlList;
         
        for (let j = 0; j < urlList.urls.length; j++){
            Logger.log('urlListId -> ' + urlList.urlListId
                + ', urlListName -> ' + urlList.urlListName
                + ', placementUrl -> ' + urlList.urls[j].placementUrl);
        }
    }
}
```

### プレイスメントリストとURLの情報を取得する / Get list and url
```.js
function getListAndUrl(){
     
    const accountId = AdsUtilities.getCurrentAccountId();
 
    const placementUrlLists = Display.PlacementUrlListService.get({
        "accountId": accountId,
    }).rval;
 
    for (let i = 0; i < placementUrlLists.totalNumEntries; i++){
        let urlList = placementUrlLists.values[i].urlList;
         
        for (let j = 0; j < urlList.urls.length; j++){
            Logger.log('urlListId -> ' + urlList.urlListId
            + ', urlListName -> ' + urlList.urlListName
            + ', brandSafetyDenyListFlg -> ' + urlList.brandSafetyDenyListFlg
            + ', placementUrl -> ' + urlList.urls[j].placementUrl
            + ', urlActiveFlg -> ' + urlList.urls[j].urlActiveFlg);
        }
    }
}
```

### 広告グループにプレイスメントリストを付与する / Apply a list to an ad group
````.js
function applyListToAdGroup(){
     
    const accountId = AdsUtilities.getCurrentAccountId();
 
    const adGroupTargets = Display.AdGroupTargetService.add({
        "accountId": accountId,
        "operand": [
            {
                "adGroupId": 209780585,
                "bidMultiplier": 1.5,
                "campaignId": 27462584,
                "target": {
                    "placementTarget": {
                        "placementUrlListType": "WHITE_LIST",
                    },
                    "targetId": 1000038400,//urlListId
                    "targetType": "PLACEMENT_TARGET"
                }
            }
        ]
    }).rval;
 
    for (let i = 0; i < Object.keys(adGroupTargets.values).length; i++){
        let adGroupTargetList = adGroupTargets.values[i].adGroupTargetList;
         
        Logger.log('adGroupId -> ' + adGroupTargetList.adGroupId
            + ', campaignId -> ' + adGroupTargetList.campaignId
            + ', placementUrlListType -> ' + adGroupTargetList.target.placementTarget.placementUrlListType
            + ', placementUrlListName -> ' + adGroupTargetList.target.placementTarget.placementUrlListName
            + ', targetId -> ' + adGroupTargetList.target.targetId
            + ', targetType -> ' + adGroupTargetList.target.targetType
            + ', bidMultiplier -> ' + adGroupTargetList.bidMultiplier);
    }
}
```
