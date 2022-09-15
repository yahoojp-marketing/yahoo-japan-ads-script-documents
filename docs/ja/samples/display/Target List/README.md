# ターゲットリスト / Target List

### ターゲットリスト情報の取得をする / Get All target list
```.js
function getAllTargetList() {
  
  const accountId = AdsUtilities.getCurrentAccountId();
  
  const retargetingLists = Display.RetargetingListService.get({
    accountId: accountId,
  }).rval;

  if (retargetingLists.totalNumEntries == 0) {
    Logger.log('RetargetingList does not exist.');
    return;
  }
  
  for (let i = 0; i < Object.keys(retargetingLists.values).length; i++){
    let retargetingList = retargetingLists.values[i].retargetingList;
    Logger.log('targetListId-> ' + retargetingList.targetListId
      + ', targetListName-> ' + retargetingList.targetListName
      + ', sourceAccountId-> ' + retargetingList.sourceAccountId
      + ', sourceAccountName-> ' + retargetingList.sourceAccountName);
  } 
}
```

### 広告グループにターゲットリスト情報を付与する / Apply a target list to an ad group
```.js
function applyTargetListToAdGroup() {
  
  const accountId = AdsUtilities.getCurrentAccountId();
  const adGroupTargetArray = [
    {
      adGroupId: 111111111,
      campaignId: 22222222,
      target: {
        targetId: 3333333333,//targetListId
        targetType: 'SITE_RETARGETING',
      }
    },
    {
      adGroupId: 444444444,
      bidMultiplier: 1.5,
      campaignId: 55555555,
      target: {
        targetId: 6666666666,//targetListId
        targetType: 'SITE_RETARGETING',
      }
    }
  ];//Multiple selections are possible
 
  const adGroupTargets = Display.AdGroupTargetService.add({
    accountId: accountId,
    operand: adGroupTargetArray,
  }).rval;

  for (let i = 0; i < Object.keys(adGroupTargets.values).length; i++) {
    if (adGroupTargets.values[i].operationSucceeded) {
      let adGroupTargetList = adGroupTargets.values[i].adGroupTargetList;
      Logger.log('adGroupId-> ' + adGroupTargetList.adGroupId
        + ', campaignId-> ' + adGroupTargetList.campaignId
        + ' linked to targetListName-> ' + adGroupTargetList.target.siteRetargetingTarget.targetListName
        + ', targetId-> ' + adGroupTargetList.target.targetId
        + ', targetType-> ' + adGroupTargetList.target.targetType
        + ', bidMultiplier-> ' + adGroupTargetList.bidMultiplier);
      
    } else {
      Logger.log('adGroupId-> ' + adGroupTargetArray[i].adGroupId
        + ', campaignId-> ' + adGroupTargetArray[i].campaignId
        + ' could not to linked to targetId-> ' + adGroupTargetArray[i].target.targetId
        + ', targetType-> ' + adGroupTargetArray[i].target.targetType);
        
    }
  }
}
```
