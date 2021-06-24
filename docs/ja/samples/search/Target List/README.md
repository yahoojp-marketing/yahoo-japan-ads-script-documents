# Target List

### Get All target list
```$xslt
function getAllTargetList(){
     
    const accountId = AdsUtilities.getCurrentAccountId();
     
    const retargetingLists = Search.RetargetingListService.get({
        "accountId": accountId,
    }).rval;
 
    for (let i = 0; i < retargetingLists.totalNumEntries; i++){   
        let targetList = retargetingLists.values[i].targetList;
 
        Logger.log('targetListId -> ' + targetList.targetListId
            + ', targetListName -> ' + targetList.targetListName);
    }  
}
```

### Apply a target list to a campaign
```$xslt
function applyTargetListToCampaign(){
     
    const accountId = AdsUtilities.getCurrentAccountId();
     
    const campaignRetargetingLists = Search.CampaignRetargetingListService.add({
        "accountId": accountId,
        "operand": [
            {
                "bidMultiplier": 1.50,//default:1.00
                "campaignId": 926659,
                "criterionTargetList": {
                    "targetListId": 2081,
                },
            }
        ]
    }).rval;
     
    for (let i = 0; i < Object.keys(campaignRetargetingLists.values).length; i++){
        let campaignRetargetingList = campaignRetargetingLists.values[i].campaignRetargetingList;
         
        Logger.log('campaignId -> ' + campaignRetargetingList.campaignId
            + ', campaignName -> ' + campaignRetargetingList.campaignName
            + ', targetListId -> ' + campaignRetargetingList.criterionTargetList.targetListId
            + ', targetListName -> ' + campaignRetargetingList.criterionTargetList.targetListName
            + ', bidMultiplier -> ' + campaignRetargetingList.bidMultiplier
            + ', excludedType -> ' + campaignRetargetingList.excludedType);
    }
}
```

### Apply a target list to an ad group
```$xslt
function applyTargetListToAdGroup(){
 
    const accountId = AdsUtilities.getCurrentAccountId();
  
    const adGroupRetargetingLists = Search.AdGroupRetargetingListService.add({
        "accountId": accountId,
        "operand": [
            {
                "adGroupId": 325336260,
                "campaignId": 925767,
                "criterionTargetList": {
                    "targetListId": 2081,
                },
            }
        ]
    }).rval;
  
    for (let i = 0; i < Object.keys(adGroupRetargetingLists.values).length; i++){
        let adGroupRetargetingList = adGroupRetargetingLists.values[i].adGroupRetargetingList;
          
        Logger.log('adGroupId -> ' + adGroupRetargetingList.adGroupId
            + ', adGroupName -> ' + adGroupRetargetingList.adGroupName
            + ', bidMultiplier -> ' + adGroupRetargetingList.bidMultiplier
            + ', campaignId -> ' + adGroupRetargetingList.campaignId
            + ', campaignName -> ' + adGroupRetargetingList.campaignName
            + ', targetListId -> ' + adGroupRetargetingList.criterionTargetList.targetListId
            + ', targetListName -> ' + adGroupRetargetingList.criterionTargetList.targetListName);
    }
}
```