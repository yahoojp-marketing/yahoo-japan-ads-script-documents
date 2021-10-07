# Negative Keyword Lists

### Get all negative keyword lists
```.js
function getAllNegativeKeywordLists(){
 
    const accountId = AdsUtilities.getCurrentAccountId();
     
    const accountShareds = Search.AccountSharedService.get({
        "accountId": accountId,
    }).rval;
 
    for (let i = 0; i < accountShareds.totalNumEntries; i++){   
        let accountShared = accountShareds.values[i].accountShared;
         
        Logger.log('memberCount -> ' + accountShared.memberCount
            + ', name -> ' + accountShared.name
            + ', referenceCount -> ' + accountShared.referenceCount
            + ', sharedListId -> ' + accountShared.sharedListId);
         
    }
}
```

### Add negative keyword list
```.js
function addNegativeKeywordList(){
     
    //const accountId = AdsUtilities.getCurrentAccountId();
     
    const accountShareds = Search.AccountSharedService.add({
        "accountId": accountId,
        "operand": [
            {
                "name": "LIST_NAME_AAAA",
            }
        ]
    }).rval;
 
    for (let i = 0; i < Object.keys(accountShareds.values).length; i++){   
        let accountShared = accountShareds.values[i].accountShared;
         
        Logger.log('memberCount -> ' + accountShared.memberCount
            + ', name -> ' + accountShared.name
            + ', referenceCount -> ' + accountShared.referenceCount
            + ', sharedListId -> ' + accountShared.sharedListId);
    }
}
```

### Set negative keyword
```.js
function setNegativeKeyword(){
     
    const accountId = AdsUtilities.getCurrentAccountId();
     
    const sharedCriterions = Search.SharedCriterionService.add({
        "accountId": accountId,
        "operand": [
            {
                "keywordMatchType": "EXACT",
                "sharedListId": 6475,
                "text": "MMMMMM",
                "use": "NEGATIVE"
            },
            {
                "keywordMatchType": "EXACT",
                "sharedListId": 6475,
                "text": "NNNNNN",
                "use": "NEGATIVE"
            }
        ]
    }).rval;
     
    for (let i = 0; i < Object.keys(sharedCriterions.values).length; i++){
        let sharedCriterion = sharedCriterions.values[i].sharedCriterion;
         
        Logger.log('criterionId -> ' + sharedCriterion.criterionId
            + ', keywordMatchType -> ' + sharedCriterion.keywordMatchType
            + ', sharedListId -> ' + sharedCriterion.sharedListId
            + ', text -> ' + sharedCriterion.text
            + ', use -> ' + sharedCriterion.use);
    }
}
```

### Apply a negative keyword list to a campaign
```.js
function applyNegativeKeywordListToCampaign(){
 
    const accountId = AdsUtilities.getCurrentAccountId();
     
    const campaignSharedSets = Search.CampaignSharedSetService.add({
        "accountId": accountId,
        "operand": [
            {
                "campaignId": 926575,
                "sharedListId": 6438,
            }
        ]
    }).rval;
     
    for (let i = 0; i < Object.keys(campaignSharedSets.values).length; i++){   
        let campaignSharedSet = campaignSharedSets.values[i].campaignSharedSet;
         
        Logger.log('campaignId -> ' + campaignSharedSet.campaignId
            + ', campaignName -> ' + campaignSharedSet.campaignName
            + ', sharedListId -> ' + campaignSharedSet.sharedListId
            + ', sharedListName -> ' + campaignSharedSet.sharedListName);
    }
}
```
