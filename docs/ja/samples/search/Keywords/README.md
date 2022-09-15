# キーワード / Keywords

### キーワードを新規追加する / Add a keywords
```.js
function addKeywords(){
  
  const accountId = AdsUtilities.getCurrentAccountId();
  const adGroupCriterionArray = [
    {
      adGroupId: 222222222,
      biddableAdGroupCriterion: {
        userStatus: 'ACTIVE',
      },
      campaignId: 1111111,
      criterion: {
        criterionType: 'KEYWORD',
        keyword: {
          keywordMatchType: 'EXACT',
          text: 'kwAAA',
        }
      },
      use: 'BIDDABLE',
    },
    {
      adGroupId: 444444444,
      biddableAdGroupCriterion: {
        userStatus: 'ACTIVE',
      },
      campaignId: 333333,
      criterion: {
        criterionType: 'KEYWORD',
        keyword: {
          keywordMatchType: 'PHRASE',
          text: 'kwBBB',
        }
      },
      use: 'BIDDABLE',
    },
    {
      adGroupId: 666666666,
      biddableAdGroupCriterion: {
        userStatus: 'ACTIVE',
      },
      campaignId: 5555555,
      criterion: {
        criterionType: 'KEYWORD',
        keyword: {
          keywordMatchType: 'BROAD',
          text: 'kwCCC',
        }
      },
      use: 'BIDDABLE',
    }
  ];//Multiple selections are possible
   
  const adGroupCriterions = Search.AdGroupCriterionService.add({
    accountId: accountId,
    operand: adGroupCriterionArray,
  }).rval;
  
  for (let i = 0; i < Object.keys(adGroupCriterions.values).length; i++){
    if (adGroupCriterions.values[i].operationSucceeded) {
      let adGroupCriterion = adGroupCriterions.values[i].adGroupCriterion;
      Logger.log('keywordText-> ' + adGroupCriterion.criterion.keyword.text
        + 'added to campaignId-> ' + adGroupCriterion.campaignId 
        + ', campaignName-> ' + adGroupCriterion.campaignName
        + ', adGroupId-> ' + adGroupCriterion.adGroupId 
        + ', adGroupName-> ' + adGroupCriterion.adGroupName);
        
    } else {
      Logger.log('keywordText-> ' + adGroupCriterionArray[i].criterion.keyword.text 
        + ' cannot be added');
    
    }
  }
}
```

### 広告グループ配下のキーワードを配信停止にする / Pause keyword in an ad group
```.js
function pauseKeywordInAdGroup(){
  
  const accountId = AdsUtilities.getCurrentAccountId();
  const adGroupIds = [111111111, 222222222];//Multiple selections are possible
  
  const adGroupCriterionsGet = Search.AdGroupCriterionService.get({
    accountId: accountId,
    adGroupIds: adGroupIds,
    use: 'BIDDABLE',
    userStatuses: ['ACTIVE'],
  }).rval;
  
  if (adGroupCriterionsGet.totalNumEntries == 0) {
    Logger.log('Target KW does not exist.');
    return;
  }
   
  let adGroupCriterionArray = [];
  for (let i = 0; i < Object.keys(adGroupCriterionsGet.values).length; i++){
    let adGroupCriterion = adGroupCriterionsGet.values[i].adGroupCriterion;
    adGroupCriterion.biddableAdGroupCriterion.userStatus = 'PAUSED';
    adGroupCriterionArray.push(adGroupCriterion);
  }
   
  const adGroupCriterionsSet = Search.AdGroupCriterionService.set({
    accountId: accountId,
    operand: adGroupCriterionArray,
  }).rval;
   
  for (let i = 0; i < Object.keys(adGroupCriterionsSet.values).length; i++){
    if (adGroupCriterionsSet.values[i].operationSucceeded) {
      let adGroupCriterion = adGroupCriterionsSet.values[i].adGroupCriterion;
      Logger.log('adGroupId-> ' + adGroupCriterion.adGroupId 
        + 'adGroupName-> ' + adGroupCriterion.adGroupName
        + ', kw-> ' + adGroupCriterion.criterion.keyword.text 
        + ' has been paused.');
      
    } else {
      let adGroupCriterion = adGroupCriterionsGet.values[i].adGroupCriterion;
      Logger.log('adGroupId-> ' + adGroupCriterion.adGroupId 
        + 'adGroupName-> ' + adGroupCriterion.adGroupName
        + ', kw-> ' + adGroupCriterion.criterion.keyword.text 
        + ' could not be stopped.');
      
    }
  }
}
```

### 指定した広告グループ配下の全てのキーワード情報を取得する / Get all keywords in an ad group
```.js
function getAllKeywordsInAdGroup(){
 
  const accountId = AdsUtilities.getCurrentAccountId();
  const adGroupIds = [111111111, 222222222];//Multiple selections are possible
  
  const adGroupCriterions = Search.AdGroupCriterionService.get({
    accountId: accountId,
    adGroupIds: adGroupIds,
    use: 'BIDDABLE',
  }).rval;

  if (adGroupCriterions.totalNumEntries == 0) {
    Logger.log('Target KW does not exist.');
    return;
  }
  
  for (let i = 0; i < Object.keys(adGroupCriterions.values).length; i++){
    let adGroupCriterion = adGroupCriterions.values[i].adGroupCriterion;
    Logger.log('adGroupId-> ' + adGroupCriterion.adGroupId 
      + ', adGroupName-> ' + adGroupCriterion.adGroupName
      + ', userStatus-> ' + adGroupCriterion.biddableAdGroupCriterion.userStatus
      + ', keywordMatchType-> ' + adGroupCriterion.criterion.keyword.keywordMatchType
      + ', keywordText-> ' + adGroupCriterion.criterion.keyword.text);
  }
}
```
