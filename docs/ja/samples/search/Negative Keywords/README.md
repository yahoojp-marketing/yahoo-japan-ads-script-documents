# Negative Keywords

### Add negative keyword to a campaign
```$xslt
function addNegativeKeywordToCampaign(){
     
    const accountId = AdsUtilities.getCurrentAccountId();
 
    const campaignCriterions = Search.CampaignCriterionService.add({
        "accountId": accountId,
        "operand": [//Multiple selections are possible
            {
                "accountId": accountId,
                "campaignId": 927192,
                "criterion": {
                    "criterionType": "KEYWORD",
                    "keyword": {
                        "keywordMatchType": "EXACT",
                        "text": "XXXXXX"
                    }
                },
                "use": "NEGATIVE"
            },
            {
                "accountId": accountId,
                "campaignId": 927192,
                "criterion": {
                    "criterionType": "KEYWORD",
                    "keyword": {
                        "keywordMatchType": "EXACT",
                        "text": "YYYYYY"
                    }
                },
                "use": "NEGATIVE"
            }
        ],
        "use": "NEGATIVE"
    }).rval;
     
    for (let i = 0; i < Object.keys(campaignCriterions.values).length; i++){
        let campaignCriterion = campaignCriterions.values[i].campaignCriterion;
         
        Logger.log('campaignId -> ' + campaignCriterion.campaignId
            + ', keywordText -> ' + campaignCriterion.criterion.keyword.text
            + ', use -> ' + campaignCriterion.use);
    }
}
```

### Add a negative keyword to an ad group
```$xslt
function addNegativeKeywordToAdGroup(){
     
    const accountId = AdsUtilities.getCurrentAccountId();
     
    const adGroupCriterions = Search.AdGroupCriterionService.add({
        "accountId": accountId,
        "operand": [
            {
                "adGroupId": 111111111,
                "campaignId": 222222,
                "criterion": {
                    "criterionType": "KEYWORD",
                    "keyword": {
                        "keywordMatchType": "EXACT",
                        "text": "AAABBBCCCDDD"
                    }
                },
                "use": "NEGATIVE",
            }
        ]
    }).rval;
 
    for (let i = 0; i < Object.keys(adGroupCriterions.values).length; i++){
        let adGroupCriterion = adGroupCriterions.values[i].adGroupCriterion;
         
        Logger.log('adGroupId-> ' + adGroupCriterion.adGroupId
            + ', campaignId-> ' + adGroupCriterion.campaignId
            + ', keywordText-> ' + adGroupCriterion.criterion.keyword.text
            + ', use-> ' + adGroupCriterion.use);
    }   
}
```

### Get negative keywords in a campaign
```$xslt
function getNegativeKeywordsInCampaign(){
     
    const accountId = AdsUtilities.getCurrentAccountId();
 
    const campaignCriterions = Search.CampaignCriterionService.get({
        "accountId": accountId,
        "campaignIds": [
            111111//Multiple selections are possible
        ],
    }).rval;
     
    for (let i = 0; i < campaignCriterions.totalNumEntries; i++){
        let campaignCriterion = campaignCriterions.values[i].campaignCriterion;
 
        Logger.log('campaignId -> ' + campaignCriterion.campaignId
            + ', keywordText -> ' + campaignCriterion.criterion.keyword.text
            + ', use -> ' + campaignCriterion.use);
    }
}
```

### Get negative keywords in an ad group
```$xslt

function getNegativeKeywordsInAdGroup(){
 
    const accountId = AdsUtilities.getCurrentAccountId();
     
    const adGroupCriterions = Search.AdGroupCriterionService.get({
        "accountId": accountId,
        "use": "NEGATIVE",
    }).rval;
     
    for (let i = 0; i < adGroupCriterions.totalNumEntries; i++){
        let adGroupCriterion = adGroupCriterions.values[i].adGroupCriterion;
         
        Logger.log('adGroupId-> ' + adGroupCriterion.adGroupId
            + ', keywordMatchType-> ' + adGroupCriterion.criterion.keyword.keywordMatchType
            + ', keywordText-> ' + adGroupCriterion.criterion.keyword.text
            + ', use-> ' + adGroupCriterion.use);
    }
}
```