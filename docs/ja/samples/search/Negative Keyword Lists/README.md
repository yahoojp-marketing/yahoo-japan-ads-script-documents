# 対象外キーワードリスト / Negative Keyword Lists

### 全ての対象外キーワードリスト情報を取得する / Get all negative keyword lists
```.js
function getAllNegativeKeywordLists() {
 
  const accountId = AdsUtilities.getCurrentAccountId();
   
  const accountShareds = Search.AccountSharedService.get({
    accountId: accountId,
  }).rval;
  
  if (accountShareds.totalNumEntries == 0) {
    Logger.log('Negative KW lists does not exist.');
    return;
  }
 
  for (let i = 0; i < Object.keys(accountShareds.values).length; i++){   
    let accountShared = accountShareds.values[i].accountShared;
    Logger.log('memberCount-> ' + accountShared.memberCount + ', name-> ' + accountShared.name
      + ', referenceCount-> ' + accountShared.referenceCount + ', sharedListId-> ' + accountShared.sharedListId);
  }
}
```

### 対象外キーワードリストを新規追加する / Add negative keyword list
```.js
function addNegativeKeywordList() {
   
  const accountId = AdsUtilities.getCurrentAccountId();
  const accountSharedArray = [
    {
      name: 'listNameAAA',
    },
    {
      name: 'listNameBBB',
    },
    {
      name: 'listNameCCC',
    }
  ];//Multiple selections are possible
   
  const accountShareds = Search.AccountSharedService.add({
    accountId: accountId,
    operand: accountSharedArray,
  }).rval;
 
  for (let i = 0; i < Object.keys(accountShareds.values).length; i++){   
    if (accountShareds.values[i].operationSucceeded) {
      let accountShared = accountShareds.values[i].accountShared;
      Logger.log('name-> ' + accountShared.name + ', sharedListId-> ' + accountShared.sharedListId + ' has added.');
      
    } else {
      Logger.log('name-> ' + accountSharedArray[i].name + ' could not be added.');
      
    }
  }
}
```

### 対象外キーワードを更新する / Set negative keyword
```.js
function setNegativeKeyword() {
   
  const accountId = AdsUtilities.getCurrentAccountId();
  const sharedCriterionArray = [
    {
      keywordMatchType: 'EXACT',
      sharedListId: 11111,
      text: 'textAAA',
      use: 'NEGATIVE'
    },
    {
      keywordMatchType: 'PHRASE',
      sharedListId: 22222,
      text: 'textBBB',
      use: 'NEGATIVE'
    },
    {
      keywordMatchType: 'BROAD',
      sharedListId: 33333,
      text: 'textCCC',
      use: 'NEGATIVE'
    }
  ];//Multiple selections are possible
   
  const sharedCriterions = Search.SharedCriterionService.add({
    accountId: accountId,
    operand: sharedCriterionArray,
  }).rval;
   
  for (let i = 0; i < Object.keys(sharedCriterions.values).length; i++){
    if (sharedCriterions.values[i].operationSucceeded) {
      let sharedCriterion = sharedCriterions.values[i].sharedCriterion;
      Logger.log('criterionId-> ' + sharedCriterion.criterionId + ', text-> ' + sharedCriterion.text
        + ', keywordMatchType-> ' + sharedCriterion.keywordMatchType
        + ' have added as negativeKW to sharedListId-> ' + sharedCriterion.sharedListId);
      
    } else {
      Logger.log('text-> ' + sharedCriterionArray[i].text
        + ' colud not be added as negativeKW to sharedListId-> ' + sharedCriterionArray[i].sharedListId);

    }
  }
}
```

### キャンペーンに対象外キーワードリストを付与する / Apply a negative keyword list to a campaign
```.js
function applyNegativeKeywordListToCampaign() {
 
  const accountId = AdsUtilities.getCurrentAccountId();
  const campaignSharedSetArray = [
    {
      campaignId: 1111111,
      sharedListId: 22222,
    },
    {
      campaignId: 3333333,
      sharedListId: 44444,
    },
    {
      campaignId: 5555555,
      sharedListId: 66666,
    }
  ];//Multiple selections are possible
  
  const campaignSharedSets = Search.CampaignSharedSetService.add({
    accountId: accountId,
    operand: campaignSharedSetArray,
  }).rval;
   
  for (let i = 0; i < Object.keys(campaignSharedSets.values).length; i++){
    if (campaignSharedSets.values[i].operationSucceeded) {
      let campaignSharedSet = campaignSharedSets.values[i].campaignSharedSet;
      Logger.log('sharedListId-> ' + campaignSharedSet.sharedListId + ', sharedListName -> ' + campaignSharedSet.sharedListName
        + ' have linked to campaignId-> ' + campaignSharedSet.campaignId + ', campaignName -> ' + campaignSharedSet.campaignName);
        
    } else {
      Logger.log('sharedListId-> ' + campaignSharedSetArray[i].sharedListId
        + ' could not to be linked to campaignId-> ' + campaignSharedSetArray[i].campaignId);
        
    }
  }
}
```
