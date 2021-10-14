# 広告グループ / Ad Groups

### 広告グループを新規追加する / Add an ad group
```.js
function addAdGroup(){
     
    const accountId = AdsUtilities.getCurrentAccountId();
 
    const adGroups = Search.AdGroupService.add({
        "accountId": accountId,
        "operand": [
            {
                "adGroupName": "BBBBBB",
                "bid": {
                    bidSource: "ADGROUP",
                    maxCpc: 1000,//default:1
                },
                "campaignId": 111111,
                "userStatus": "ACTIVE",
            }
        ]
    }).rval;
     
    for (let i = 0; i < Object.keys(adGroups.values).length; i++) {
        let adGroup = adGroups.values[i].adGroup;
        Logger.log('adGroupId-> ' + adGroup.adGroupId + ', adGroupName-> ' + adGroup.adGroupName + ', bidMaxCpc-> ' + adGroup.bid.maxCpc);
    }
}
```

### 広告グループを配信停止にする / Pause an ad group
```.js
function pauseAdGroup(){
     
    const accountId = AdsUtilities.getCurrentAccountId();
 
    const adGroupsGet = Search.AdGroupService.get({
        "accountId": accountId,
    }).rval;
 
    let adGroupArray = [];
     
    for (let i = 0; i < adGroupsGet.totalNumEntries; i++) {
        let adGroupData = adGroupsGet.values[i].adGroup;
         
        adGroupData.userStatus = "PAUSED";
         
        adGroupArray.push(adGroupData);
    }
 
    const adGroupsSet = Search.AdGroupService.set({
        "accountId": accountId,
        "operand": adGroupArray,
    }).rval;
     
    for (let i = 0; i < Object.keys(adGroupsSet.values).length; i++) {
        let adGroup = adGroupsSet.values[i].adGroup;
         
        Logger.log('adGroupId-> ' + adGroup.adGroupId + ', adGroupName-> ' + adGroup.adGroupName + ', userStatus-> ' + adGroup.userStatus);
    }
}
```

### 広告グループの入札価格を更新する / Set ad group bid
```.js

function setAdGroupBid(){
     
    const accountId = AdsUtilities.getCurrentAccountId();
 
    let adGroupArray = [];
 
    const adGroupsGet = Search.AdGroupService.get({
        "accountId": accountId,
        "adGroupIds": [
            325446248,//Multiple selections are possible
        ],
    }).rval;
     
    for (let i = 0; i < adGroupsGet.totalNumEntries; i++) {
        let adGroup = adGroupsGet.values[i].adGroup;
         
        adGroup.bid.maxCpc = 2000;
         
        adGroupArray.push(adGroup);
    }
 
    const adGroupsSet = Search.AdGroupService.set({
        "accountId": accountId,
        "operand": adGroupArray,
    }).rval;
     
    for (let i = 0; i < Object.keys(adGroupsSet.values).length; i++) {
        let adGroup = adGroupsSet.values[i].adGroup;
         
        Logger.log('adGroupId-> ' + adGroup.adGroupId + ', adGroupName-> ' + adGroup.adGroupName + ', bidMaxCpc-> ' + adGroup.bid.maxCpc);
    }
}
```

### アカウント配下の全ての広告グループ情報を取得する / Get all ad group
```.js

function getAllAdGroup(){
     
    const accountId = AdsUtilities.getCurrentAccountId();
 
    const adGroups = Search.AdGroupService.get({
        "accountId": accountId,
    }).rval;
     
    for (let i = 0; i < adGroups.totalNumEntries; i++) {
        let adGroupData = adGroups.values[i].adGroup;
        Logger.log('adGroupId-> ' + adGroupData.adGroupId + ', adGroupName-> ' + adGroupData.adGroupName);
    }
}
```

### 指定した全ての広告グループ情報を取得する / Get all ad group by id
```.js
function getAllAdGroupById(){
     
    const accountId = AdsUtilities.getCurrentAccountId();
 
    const adGroups = Search.AdGroupService.get({
        "accountId": accountId,
        "adGroupIds": [
            111111111, 222222222,//Multiple selections are possible
        ],
    }).rval;
     
    for (let i = 0; i < adGroups.totalNumEntries; i++) {
        let adGroupData = adGroups.values[i].adGroup;
        Logger.log('adGroupId-> ' + adGroupData.adGroupId + ', adGroupName-> ' + adGroupData.adGroupName);
    }
}
```
