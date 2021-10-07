# Search Keyword Lists

### Add list and keyword
```.js
function addListAndKeyword(){
     
    const accountId = AdsUtilities.getCurrentAccountId();
 
    const searchKeywordLists = Display.SearchKeywordListService.add({
        "accountId": accountId,
        "operand": [
            {
                "accountId": accountId,
                "keywordFrequency": "ONCE_OR_MORE",
                "keywordRecency": "WITHIN_7DAYS",
                "searchKeyword": [
                    {
                        "searchKeywordId": 1000020101//Get in SearchKeywordIdeaService
                    }
                ],
                "searchKeywordListDescription": "BBBBBB",
                "searchKeywordListName": "BBB"
            }
        ]
    }).rval;
 
    for (let i = 0; i < Object.keys(searchKeywordLists.values).length; i++){
        let searchKeywordList = searchKeywordLists.values[i].searchKeywordList;
         
        for (let j = 0; j < searchKeywordList.searchKeyword.length; j++){
            let  searchKeyword = searchKeywordList.searchKeyword;
 
            Logger.log('deliveryStatus -> ' + searchKeywordList.deliveryStatus
                + ', keywordFrequency -> ' + searchKeywordList.keywordFrequency
                + ', keywordRecency -> ' + searchKeywordList.keywordRecency
                + ', searchKeywordId -> ' + searchKeywordList.searchKeyword[j].searchKeywordId
                + ', searchKeywordListDescription -> ' + searchKeywordList.searchKeywordListDescription
                + ', searchKeywordListId -> ' + searchKeywordList.searchKeywordListId
                + ', searchKeywordListDescription -> ' + searchKeywordList.searchKeywordListDescription
                + ', searchKeywordListName -> ' + searchKeywordList.searchKeywordListName);    
        }
    }
}
```

### Set keyword
```.js
function setKeyword(){
     
    const accountId = AdsUtilities.getCurrentAccountId();
 
    const searchKeywordListsGet = Display.SearchKeywordListService.get({
        "accountId": accountId,
        "searchKeywordListIds": [
          1000116542
        ],
    }).rval;
     
    let searchKeywordListArray = [];
     
    for (let i = 0; i < searchKeywordListsGet.totalNumEntries; i++){
        let searchKeywordList = searchKeywordListsGet.values[i].searchKeywordList;
         
        for (let j = 0; j < searchKeywordList.searchKeyword.length; j++){
             
            if (searchKeywordList.searchKeyword[j].searchKeywordId == 1000020101){
                searchKeywordList.searchKeyword[j].searchKeywordId = 1000020104;
            }
        }
         
        searchKeywordListArray.push(searchKeywordList);
    }
     
    const searchKeywordListsSet = Display.SearchKeywordListService.set({
        "accountId": accountId,
        "operand": searchKeywordListArray
    }).rval;
 
    for (let i = 0; i < Object.keys(searchKeywordListsSet).length; i++){
        let searchKeywordList = searchKeywordListsSet.values[i].searchKeywordList;
         
        for (let j = 0; j < searchKeywordList.searchKeyword.length; j++){
            let  searchKeyword = searchKeywordList.searchKeyword;
 
            Logger.log('deliveryStatus -> ' + searchKeywordList.deliveryStatus
                + ', keywordFrequency -> ' + searchKeywordList.keywordFrequency
                + ', keywordRecency -> ' + searchKeywordList.keywordRecency
                + ', searchKeywordId -> ' + searchKeywordList.searchKeyword[j].searchKeywordId
                + ', searchKeywordListDescription -> ' + searchKeywordList.searchKeywordListDescription
                + ', searchKeywordListId -> ' + searchKeywordList.searchKeywordListId
                + ', searchKeywordListName -> ' + searchKeywordList.searchKeywordListName);    
        }
    }
}
```

### Get list and keyword
```.js
function getListAndKeyword(){
     
    const accountId = AdsUtilities.getCurrentAccountId();
 
    const searchKeywordLists = Display.SearchKeywordListService.get({
        "accountId": accountId,
    }).rval;
 
    for (let i = 0; i < searchKeywordLists.totalNumEntries; i++){
        let searchKeywordList = searchKeywordLists.values[i].searchKeywordList;
         
        for (let j = 0; j < searchKeywordList.searchKeyword.length; j++){
            Logger.log('deliveryStatus -> ' + searchKeywordList.deliveryStatus
                + ', keywordFrequency -> ' + searchKeywordList.keywordFrequency
                + ', keywordRecency -> ' + searchKeywordList.keywordRecency
                + ', searchKeywordId -> ' + searchKeywordList.searchKeyword[j].searchKeywordId
                + ', searchKeywordListDescription -> ' + searchKeywordList.searchKeywordListDescription
                + ', searchKeywordListId -> ' + searchKeywordList.searchKeywordListId
                + ', searchKeywordListName -> ' + searchKeywordList.searchKeywordListName);
        }
    }
}
```

### Apply a list to an ad group
```.js
function applyListToAdGroupSerchKeywordList(){
     
    const accountId = AdsUtilities.getCurrentAccountId();
 
    const adGroupTargets = Display.AdGroupTargetService.add({
        "accountId": accountId,
        "operand": [
            {
                "adGroupId": 209780585,
                "bidMultiplier": 1.5,
                "campaignId": 27462584,
                "target": {
                    "searchTarget": {
                        //"searchKeywordListName": "",
                    },
                    "targetId": 1000116541,//searchKeywordListId
                    "targetType": "SEARCH_TARGET"
                }
            }
        ]
    }).rval;
 
    for (let i = 0; i < Object.keys(adGroupTargets.values).length; i++){
        let adGroupTargetList = adGroupTargets.values[i].adGroupTargetList;
         
        Logger.log('adGroupId -> ' + adGroupTargetList.adGroupId
            + ', campaignId -> ' + adGroupTargetList.campaignId
            + ', searchKeywordListName -> ' + adGroupTargetList.target.searchTarget.searchKeywordListName
            + ', targetId -> ' + adGroupTargetList.target.targetId
            + ', targetType -> ' + adGroupTargetList.target.targetType
            + ', bidMultiplier -> ' + adGroupTargetList.bidMultiplier);
    }
}
```