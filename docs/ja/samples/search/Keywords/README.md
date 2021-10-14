# キーワード / Keywords

### キーワードを新規追加する / Add a keywords
```.js
function addKeywords(){
     
    const accountId = AdsUtilities.getCurrentAccountId();
     
    const adGroupCriterions = Search.AdGroupCriterionService.add({
        "accountId": accountId,
        "operand": [//Multiple selections are possible
            {
                "adGroupId": 325526300,
                "biddableAdGroupCriterion": {
                    "userStatus": "ACTIVE"
                },
                "campaignId": 927192,
                "criterion": {
                    "criterionType": "KEYWORD",
                    "keyword": {
                        "keywordMatchType": "EXACT",
                        "text": "AAABBB"
                    }
                },
                "use": "BIDDABLE",
            },
            {
                "adGroupId": 325526300,
                "biddableAdGroupCriterion": {
                    "userStatus": "ACTIVE"
                },
                "campaignId": 927192,
                "criterion": {
                    "criterionType": "KEYWORD",
                    "keyword": {
                        "keywordMatchType": "EXACT",
                        "text": "CCCDDD"
                    }
                },
                "use": "BIDDABLE",
            }
        ]
    }).rval;
 
    for (let i = 0; i < Object.keys(adGroupCriterions.values).length; i++){
        let adGroupCriterion = adGroupCriterions.values[i].adGroupCriterion;
         
        Logger.log('adGroupId-> ' + adGroupCriterion.adGroupId
            + ', campaignId-> ' + adGroupCriterion.campaignId
            + ', keywordText-> ' + adGroupCriterion.criterion.keyword.text);
    }
}
```

### 広告グループ配下のキーワードを配信停止にする / Pause keyword in an ad group
```.js
function pauseKeywordInAdGroup(){
 
    const accountId = AdsUtilities.getCurrentAccountId();
     
    const adGroupCriterionsGet = Search.AdGroupCriterionService.get({
        "accountId": accountId,
        "adGroupIds": [
          325526300,//Multiple selections are possible
        ],
        "use": "BIDDABLE",
    }).rval;
     
    let adGroupCriterionArray = [];
     
    for (let i = 0; i < adGroupCriterionsGet.totalNumEntries; i++){
        let adGroupCriterion = adGroupCriterionsGet.values[i].adGroupCriterion;
         
        adGroupCriterion.biddableAdGroupCriterion.userStatus = "PAUSED";
         
        adGroupCriterionArray.push(adGroupCriterion);
    }
     
    const adGroupCriterionsSet = Search.AdGroupCriterionService.set({
        "accountId": accountId,
        "operand": adGroupCriterionArray,
    }).rval;
     
    for (let i = 0; i < Object.keys(adGroupCriterionsSet.values).length; i++){
        let adGroupCriterion = adGroupCriterionsSet.values[i].adGroupCriterion;
         
        adGroupCriterion.biddableAdGroupCriterion.userStatus = "PAUSED";
         
        Logger.log('adGroupId -> ' + adGroupCriterion.adGroupId
            + ', userStatus -> ' + adGroupCriterion.biddableAdGroupCriterion.userStatus
            + ', use -> ' + adGroupCriterion.use);
    }
}
```

### 指定した広告グループ配下の全てのキーワード情報を取得する / Get all keywords in an ad group
```.js
function getAllKeywordsInAdGroup(){
 
    const accountId = AdsUtilities.getCurrentAccountId();
     
    const adGroupCriterions = Search.AdGroupCriterionService.get({
        "accountId": accountId,
        "adGroupIds": [
            111111111, 222222222,//Multiple selections are possible
        ],
        "use": "BIDDABLE",
    }).rval;
     
    for (let i = 0; i < adGroupCriterions.totalNumEntries; i++){
        let adGroupCriterion = adGroupCriterions.values[i].adGroupCriterion;
         
        Logger.log('adGroupId-> ' + adGroupCriterion.adGroupId
            + ', keywordMaxCpc-> ' + adGroupCriterion.biddableAdGroupCriterion.bid.keywordMaxCpc
            + ', keywordMatchType-> ' + adGroupCriterion.criterion.keyword.keywordMatchType
            + ', keywordText-> ' + adGroupCriterion.criterion.keyword.text);
    }
}
```
