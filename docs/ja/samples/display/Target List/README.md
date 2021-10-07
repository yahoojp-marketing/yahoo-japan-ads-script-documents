# Target List

### Get All target list
```.js
function getAllTargetList(){
     
    const accountId = AdsUtilities.getCurrentAccountId();
     
    const retargetingLists = Display.RetargetingListService.get({
        "accountId": accountId,
    }).rval;
 
    for (let i = 0; i < retargetingLists.totalNumEntries; i++){
        let retargetingList = retargetingLists.values[i].retargetingList;
         
        Logger.log('description-> ' + retargetingList.description
            + ', targetListId-> ' + retargetingList.targetListId
            + ', targetListName-> ' + retargetingList.targetListName
            + ', sourceAccountId-> ' + retargetingList.sourceAccountId
            + ', sourceAccountName-> ' + retargetingList.sourceAccountName);
    } 
}
```

### Apply a target list to an ad group
```.js
function applyTargetListToAdGroup(){
     
    const accountId = AdsUtilities.getCurrentAccountId();
 
    const adGroupTargets = Display.AdGroupTargetService.add({
        "accountId": accountId,
        "operand": [
            {
                "adGroupId": 209780518,
                "bidMultiplier": 1.5,
                "campaignId": 27462571,
                "target": {
                    "targetId": 1000337112,//targetListId
                    "targetType": "SITE_RETARGETING"
                }
            }
        ]
    }).rval;
 
    for (let i = 0; i < Object.keys(adGroupTargets.values).length; i++){
        let adGroupTargetList = adGroupTargets.values[i].adGroupTargetList;
         
        Logger.log('adGroupId -> ' + adGroupTargetList.adGroupId
            + ', bidMultiplier -> ' + adGroupTargetList.bidMultiplier
            + ', campaignId -> ' + adGroupTargetList.campaignId
            + ', targetListName -> ' + adGroupTargetList.target.siteRetargetingTarget.targetListName
            + ', targetType -> ' + adGroupTargetList.target.targetType
            + ', targetId -> ' + adGroupTargetList.target.targetId);
    }
}
```