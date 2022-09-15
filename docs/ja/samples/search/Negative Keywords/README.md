# 対象外キーワード / Negative Keywords

### キャンペーンに対象外キーワードを追加する / Add negative keyword to a campaign
```.js
function addNegativeKeywordToCampaign() {
   
  const accountId = AdsUtilities.getCurrentAccountId();
  const campaignCriterionArray = [
    {
      accountId: accountId,
      campaignId: 1111111,
      criterion: {
        criterionType: 'KEYWORD',
        keyword: {
          keywordMatchType: 'EXACT',
          text: 'textXXX',
        }
      },
      use: 'NEGATIVE'
    },
    {
      accountId: accountId,
      campaignId: 2222222,
      criterion: {
        criterionType: 'KEYWORD',
        keyword: {
          keywordMatchType: 'PHRASE',
          text: 'textYYY',
        }
      },
      use: 'NEGATIVE'
    },
    {
      accountId: accountId,
      campaignId: 3333333,
      criterion: {
        criterionType: 'KEYWORD',
        keyword: {
          keywordMatchType: 'BROAD',
          text: 'textZZZ',
        }
      },
      use: 'NEGATIVE',
    }
  ];//Multiple selections are possible
 
  const campaignCriterions = Search.CampaignCriterionService.add({
    accountId: accountId,
    operand: campaignCriterionArray,
    use: 'NEGATIVE',
  }).rval;
   
  for (let i = 0; i < Object.keys(campaignCriterions.values).length; i++){
    if (campaignCriterions.values[i].operationSucceeded) {
      let campaignCriterion = campaignCriterions.values[i].campaignCriterion;
      Logger.log('text-> ' + campaignCriterion.criterion.keyword.text
        + ' have added as negativeKW to campaignId-> ' + campaignCriterion.campaignId + ', campaignName-> ' + campaignCriterion.campaignName);
        
    } else {
      Logger.log('text-> ' + campaignCriterionArray[i].criterion.keyword.text
        + ' could not be added as negativeKW to campaignId-> ' + campaignCriterionArray[i].campaignId);

    }
  }
}
```

### 広告グループに対象外キーワードを追加する / Add a negative keyword to an ad group
```.js
function addNegativeKeywordToAdGroup() {
   
  const accountId = AdsUtilities.getCurrentAccountId();
  const adGroupCriterionArray = [
    {
      adGroupId: 111111111,
      campaignId: 2222222,
      criterion: {
        criterionType: 'KEYWORD',
        keyword: {
          keywordMatchType: 'EXACT',
          text: 'nkw1',
        }
      },
      use: 'NEGATIVE',
    },
    {
      adGroupId: 333333333,
      campaignId: 4444444,
      criterion: {
        criterionType: 'KEYWORD',
        keyword: {
          keywordMatchType: 'PHRASE',
          text: 'nkw2',
        }
      },
      use: 'NEGATIVE',
    },
    {
      adGroupId: 555555555,
      campaignId: 6666666,
      criterion: {
        criterionType: 'KEYWORD',
        keyword: {
          keywordMatchType: 'BROAD',
          text: 'nkw3',
        }
      },
      use: 'NEGATIVE',
    }
  ];
   
  const adGroupCriterions = Search.AdGroupCriterionService.add({
    accountId: accountId,
    operand: adGroupCriterionArray,
  }).rval;
 
  for (let i = 0; i < Object.keys(adGroupCriterions.values).length; i++){
    if (adGroupCriterions.values[i].operationSucceeded) {
      let adGroupCriterion = adGroupCriterions.values[i].adGroupCriterion;
      Logger.log('text-> ' + adGroupCriterion.criterion.keyword.text + ' have added as negativeKW to adGroupId-> '
        + adGroupCriterion.adGroupId + ', adGroupName-> ' + adGroupCriterion.adGroupName
        + ' campaignId-> ' + adGroupCriterion.campaignId + ', campaignName-> ' + adGroupCriterion.campaignName);
      
    } else {
      Logger.log('text-> ' + adGroupCriterionArray[i].criterion.keyword.text + ' could not be added as negativeKW to campaignId-> '
        + adGroupCriterionArray[i].campaignId + ', adGroupId-> ' + adGroupCriterionArray[i].adGroupId);
        
    }
  }   
}
```

### キャンペーン配下の対象外キーワード情報を取得する / Get negative keywords in a campaign
```.js
function getNegativeKeywordsInCampaign() {
   
  const accountId = AdsUtilities.getCurrentAccountId();
  const campaignIds = [1111111, 2222222, 3333333];//Empty when not specified
 
  const campaignCriterions = Search.CampaignCriterionService.get({
    accountId: accountId,
    campaignIds: campaignIds,
  }).rval;
  
  if (campaignCriterions.totalNumEntries == 0) {
    Logger.log('Negative KW does not exist.');
    return;
  }

  for (let i = 0; i < Object.keys(campaignCriterions.values).length; i++){
    let campaignCriterion = campaignCriterions.values[i].campaignCriterion;
    Logger.log('campaignId-> ' + campaignCriterion.campaignId + ', campaignName->' + campaignCriterion.campaignName
      + ', keywordMatchType-> ' + campaignCriterion.criterion.keyword.keywordMatchType + ', text-> ' + campaignCriterion.criterion.keyword.text);
  }
}
```

### 広告グループ配下の対象外キーワード情報を取得する / Get negative keywords in an ad group
```.js
function getNegativeKeywordsInAdGroup() {
 
  const accountId = AdsUtilities.getCurrentAccountId();
  const adGroupIds = [111111111, 222222222, 333333333];//Empty when not specified
   
  const adGroupCriterions = Search.AdGroupCriterionService.get({
    accountId: accountId,
    adGroupIds: adGroupIds,
    use: 'NEGATIVE',
  }).rval;
  
  if (adGroupCriterions.totalNumEntries == 0) {
    Logger.log('Negative KW does not exist.');
    return;
  }

  for (let i = 0; i < Object.keys(adGroupCriterions.values).length; i++){
    let adGroupCriterion = adGroupCriterions.values[i].adGroupCriterion;
    Logger.log('adGroupId-> ' + adGroupCriterion.adGroupId + ', adGroupName-> ' + adGroupCriterion.adGroupName
      + ', keywordMatchType-> ' + adGroupCriterion.criterion.keyword.keywordMatchType + ', text-> ' + adGroupCriterion.criterion.keyword.text);
  }
}
```
