# Ad Groups

### Add an ad group
```.js

function addAdGroup(){
 
    const accountId = AdsUtilities.getCurrentAccountId();
 
    const adGroups = Display.AdGroupService.add({
        "accountId": accountId,
        "operand": [
            {
                "accountId": accountId,
                "adGroupName": "AAA_DESKTOP",
                "campaignId": 27462571,
                "device": [
                    "DESKTOP"
                ],
                "userStatus": "ACTIVE",
            }
        ]
    }).rval;
     
    for (let i = 0; i < Object.keys(adGroups.values).length; i++){
        let adGroup = adGroups.values[i].adGroup;
         
        Logger.log('adGroupId -> ' + adGroup.adGroupId
            + ', adGroupName -> ' + adGroup.adGroupName
            + ', campaignId -> ' + adGroup.campaignId);
    }
}
```

### Pause an ad group
```.js
function pauseAdGroup(){
 
    const accountId = AdsUtilities.getCurrentAccountId();
     
    const adGroupsGet = Display.AdGroupService.get({
        "accountId": accountId,
    }).rval;
 
    let adGroupsArray = [];
     
    for (let i = 0; i < adGroupsGet.totalNumEntries; i++){
        let adGroup = adGroupsGet.values[i].adGroup;
         
        adGroup.conversionOptimizer = null;//conversionOptimizer objects interfere with updates
        adGroup.userStatus = "PAUSED";
         
        adGroupsArray.push(adGroup);
    }
     
    const adGroupsSet = Display.AdGroupService.set({
        "accountId": accountId,
        "operand": adGroupsArray,
    }).rval;
     
    for (let i = 0; i < Object.keys(adGroupsSet.values).length; i++){
        let adGroup = adGroupsSet.values[i].adGroup;
         
        Logger.log('adGroupId-> ' + adGroup.adGroupId
            + ', adGroupName-> ' + adGroup.adGroupName
            + ', campaignId-> ' + adGroup.campaignId
            + ', campaignName-> ' + adGroup.campaignName
            + ', userStatus-> ' + adGroup.userStatus);
    }
}
```

### Set ad group bid
```.js
function setAdGroupBid(){
 
    const accountId = AdsUtilities.getCurrentAccountId();
     
    const adGroupsGet = Display.AdGroupService.get({
        "accountId": accountId,
    }).rval;
 
    let adGroupsArray = [];
    let bid = 3000;
     
    for (let i = 0; i < adGroupsGet.totalNumEntries; i++){
        let adGroup = adGroupsGet.values[i].adGroup;
         
        switch (adGroup.adGroupBiddingStrategy.campaignBiddingStrategyType) {
            case "MAX_VCPM":
                adGroup.adGroupBiddingStrategy.maxVcpmBidValue = bid;
                break;
            case "MAX_CPC":
                adGroup.adGroupBiddingStrategy.maxCpcBidValue = bid;
                break;
            case "MAX_CPV":
                adGroup.adGroupBiddingStrategy.maxCpvBidValue = bid;
                break;
            case "TARGET_CPA":
                adGroup.adGroupBiddingStrategy.targetCpaBidValue = bid;
                break;
            default:
                adGroup.adGroupBiddingStrategy.campaignBiddingStrategyType = "MAX_CPC";
                adGroup.adGroupBiddingStrategy.maxCpcBidValue = bid;
                break;
        }
        adGroup.conversionOptimizer = null;//conversionOptimizer objects interfere with updates
         
        adGroupsArray.push(adGroup);
    }
     
    const adGroupsSet = Display.AdGroupService.set({
        "accountId": accountId,
        "operand": adGroupsArray,
    }).rval;
     
    for (let i = 0; i < Object.keys(adGroupsSet.values).length; i++){
        let adGroup = adGroupsSet.values[i].adGroup;
 
        switch (adGroup.adGroupBiddingStrategy.campaignBiddingStrategyType) {
            case "MAX_VCPM":
                bid = adGroup.adGroupBiddingStrategy.maxVcpmBidValue;
                break;
            case "MAX_CPC":
                bid = adGroup.adGroupBiddingStrategy.maxCpcBidValue;
                break;
            case "MAX_CPV":
                bid = adGroup.adGroupBiddingStrategy.maxCpvBidValue;
                break;
            case "TARGET_CPA":
                bid = adGroup.adGroupBiddingStrategy.targetCpaBidValue;
                break;
            default:
                break;
        }
 
        Logger.log('adGroupId-> ' + adGroup.adGroupId
            + ', adGroupName-> ' + adGroup.adGroupName
            + ', campaignId-> ' + adGroup.campaignId
            + ', campaignName-> ' + adGroup.campaignName
            + ', campaignBiddingStrategyType-> ' + adGroup.adGroupBiddingStrategy.campaignBiddingStrategyType
            + ', bid-> ' + bid);
    }
}
```

### Get all ad group 
```.js
function getAllAdGroup(){
 
    const accountId = AdsUtilities.getCurrentAccountId();
     
    const adGroups = Display.AdGroupService.get({
        "accountId": accountId,
    }).rval;
 
    for (let i = 0; i < adGroups.totalNumEntries; i++){
        let adGroup = adGroups.values[i].adGroup;
         
        Logger.log('adGroupId-> ' + adGroup.adGroupId
            + ', adGroupName-> ' + adGroup.adGroupName
            + ', campaignId-> ' + adGroup.campaignId
            + ', campaignName-> ' + adGroup.campaignName);
    }
}
```

### Get all ad group by id
```.js

function getAllAdGroupById(){
 
    const accountId = AdsUtilities.getCurrentAccountId();
     
    const adGroups = Display.AdGroupService.get({
        "accountId": accountId,
        "adGroupIds": [
            211636354, 210346406,//Multiple selections are possible
        ]
    }).rval;
 
    for (let i = 0; i < adGroups.totalNumEntries; i++){
        let adGroup = adGroups.values[i].adGroup;
         
        Logger.log('adGroupId-> ' + adGroup.adGroupId
            + ', adGroupName-> ' + adGroup.adGroupName
            + ', campaignId-> ' + adGroup.campaignId
            + ', campaignName-> ' + adGroup.campaignName);
    }
}

```

