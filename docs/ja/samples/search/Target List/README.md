# ターゲットリスト / Target List

### ターゲットリスト情報を取得する / Get All target list
```.js
function getAllTargetList() {
   
  const accountId = AdsUtilities.getCurrentAccountId();
   
  const retargetingLists = Search.RetargetingListService.get({
    accountId: accountId,
  }).rval;
  
  if (retargetingLists.totalNumEntries == 0) {
    Logger.log('Target lists does not exist.');
    return;
  }
 
  for (let i = 0; i < Object.keys(retargetingLists.values).length; i++){   
    let targetList = retargetingLists.values[i].targetList;
    Logger.log('targetListId-> ' + targetList.targetListId + ', targetListName-> ' + targetList.targetListName
      + ', targetListType-> ' + targetList.targetListType);
  }  
}
```

### キャンペーンにターゲットリスト情報を付与する / Apply a target list to a campaign
```.js
function applyTargetListToCampaign() {
   
  const accountId = AdsUtilities.getCurrentAccountId();
  const campaignRetargetingListArray = [
    {
      bidMultiplier: 1.50,//default:1.00
      campaignId: 1111111,
      criterionTargetList: {
        targetListId: 222222,
      },
      excludedType: 'INCLUDED',
    },
    {
      campaignId: 3333333,
      criterionTargetList: {
        targetListId: 444444,
      },
    }
  ];//Multiple selections are possible
   
  const campaignRetargetingLists = Search.CampaignRetargetingListService.add({
    accountId: accountId,
    operand: campaignRetargetingListArray,
  }).rval;
   
  for (let i = 0; i < Object.keys(campaignRetargetingLists.values).length; i++){
    if (campaignRetargetingLists.values[i].operationSucceeded) {
      let campaignRetargetingList = campaignRetargetingLists.values[i].campaignRetargetingList;
      Logger.log('targetListId-> ' + campaignRetargetingList.criterionTargetList.targetListId
        + ', targetListName-> ' + campaignRetargetingList.criterionTargetList.targetListName
        + ' have linked as excludedType-> ' + campaignRetargetingList.excludedType
        + ', bidMultiplier-> ' + campaignRetargetingList.bidMultiplier
        + ' to campaignId-> ' + campaignRetargetingList.campaignId + ', campaignName-> ' + campaignRetargetingList.campaignName);
        
    } else {
      Logger.log('targetListId-> ' + campaignRetargetingListArray[i].criterionTargetList.targetListId
        + ' could not be linked to campaignId-> ' + campaignRetargetingListArray[i].campaignId);
      
    }
  }
}
```

### 広告グループにターゲットリスト情報を付与する / Apply a target list to an ad group
```.js
function applyTargetListToAdGroup() {
 
  const accountId = AdsUtilities.getCurrentAccountId();
  const adGroupRetargetingListArray = [
    {
      adGroupId: 111111111,
      bidMultiplier: 1.50,//default:1.00
      campaignId: 2222222,
      criterionTargetList: {
        targetListId: 333333,
      },
      excludedType: 'EXCLUDED',//default:INCLUDED
    },
    {
      adGroupId: 444444444,
      campaignId: 5555555,
      criterionTargetList: {
        targetListId: 666666,
      },
    }
  ];//Multiple selections are possible
  
  const adGroupRetargetingLists = Search.AdGroupRetargetingListService.add({
    accountId: accountId,
    operand: adGroupRetargetingListArray,
  }).rval;
  
  for (let i = 0; i < Object.keys(adGroupRetargetingLists.values).length; i++){
    if (adGroupRetargetingLists.values[i].operationSucceeded) {
      let adGroupRetargetingList = adGroupRetargetingLists.values[i].adGroupRetargetingList;
      Logger.log('targetListId-> ' + adGroupRetargetingList.criterionTargetList.targetListId
        + ', targetListName-> ' + adGroupRetargetingList.criterionTargetList.targetListName
        + ' have linked as excludedType-> ' + adGroupRetargetingList.excludedType
        + ', bidMultiplier-> ' + adGroupRetargetingList.bidMultiplier
        + ' to adGroupId-> ' + adGroupRetargetingList.adGroupId + ', adGroupName-> ' + adGroupRetargetingList.adGroupName);
        
    } else {
      Logger.log('targetListId-> ' + adGroupRetargetingListArray[i].criterionTargetList.targetListId
        + ' could not be linked to adGroupId-> ' + adGroupRetargetingListArray[i].adGroupId);
        
    }
  }
}
```
