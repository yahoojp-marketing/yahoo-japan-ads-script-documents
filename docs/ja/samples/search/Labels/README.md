# ラベル / Labels

### 全てのラベル情報を取得する / Get all labels
```.js
function getAllLabels() {
   
  const accountId = AdsUtilities.getCurrentAccountId();
   
  const labels = Search.LabelService.get({
    accountId: accountId,
  }).rval;
  
  if (labels.totalNumEntries == 0) {
    Logger.log('Target LABEL does not exist.');
    return;
  }
  
  for (let i = 0; i < Object.keys(labels.values).length; i++){
    let label = labels.values[i].label;
    Logger.log('labelId-> ' + label.labelId + ', labelName-> ' + label.labelName);
  }
}
```

### ラベルを新規追加する / Add a label
```.js
function addLabel() {
   
  const accountId = AdsUtilities.getCurrentAccountId();
  const labelArray = [
    {
      labelName: 'labelAAA',
    },
    {
      labelName: 'labelBBB',
    },
    {
      labelName: 'labelCCC',
    }
  ];//Multiple selections are possible
   
  const labels = Search.LabelService.add({
    accountId: accountId,
    operand: labelArray,
  }).rval;
 
  for (let i = 0; i < Object.keys(labels.values).length; i++){
    if (labels.values[i].operationSucceeded) {
      let label = labels.values[i].label;
      Logger.log('labelId-> ' + label.labelId + ', labelName-> ' + label.labelName + ' has added.');
      
    } else {
      Logger.log('labelName-> ' + labelArray[i].labelName + ' could not be added.');
      
    }
  }
}
```

### キャンペーンにラベルを付与する / Apply a label to a campaign
```.js
function applyLabelToCampaign() {
 
  const accountId = AdsUtilities.getCurrentAccountId();
  const campaignLabelArray = [
    {
      campaignId: 1111111,
      labelId: 22222,
    },
    {
      campaignId: 3333333,
      labelId: 44444,
    },
    {
      campaignId: 5555555,
      labelId: 66666,
    }
  ];//Multiple selections are possible
   
  const campaignLabels = Search.CampaignLabelService.add({
    accountId: accountId,
    operand: campaignLabelArray,
  }).rval;
 
  for (let i = 0; i < Object.keys(campaignLabels.values).length; i++){
    if (campaignLabels.values[i].operationSucceeded) {
      let campaignLabel = campaignLabels.values[i].campaignLabel;
      Logger.log('labelId->' + campaignLabel.labelId + ' have linked to campaignId-> ' + campaignLabel.campaignId);
    
    } else {
      Logger.log('labelId->' + campaignLabelArray[i].labelId + ' could not be linked to campaignId-> ' + campaignLabelArray[i].campaignId);
      
    }
  }
}
```

### 広告グループにラベルを付与する / Apply a label to an ad group
```.js
function applyLabelToAdGroup() {
 
  const accountId = AdsUtilities.getCurrentAccountId();
  const adGroupLabelArray = [
    {
      adGroupId: 111111111,
      campaignId: 2222222,
      labelId: 33333,
    },
    {
      adGroupId: 444444444,
      campaignId: 5555555,
      labelId: 66666,
    },
    {
      adGroupId: 777777777,
      campaignId: 8888888,
      labelId: 99999,
    }
  ];//Multiple selections are possible
   
  const adGroupLabels = Search.AdGroupLabelService.add({
    accountId: accountId,
    operand: adGroupLabelArray,
  }).rval;
   
  for (let i = 0; i < Object.keys(adGroupLabels.values).length; i++){
    if (adGroupLabels.values[i].operationSucceeded) {
      let adGroupLabel = adGroupLabels.values[i].adGroupLabel;
      Logger.log('labelId-> ' + adGroupLabel.labelId + ' have linked to adGroupId-> ' + adGroupLabel.adGroupId);
        
    } else {
      Logger.log('labelId-> ' + adGroupLabelArray[i].labelId + ' could not be linked to adGroupId-> ' + adGroupLabelArray[i].adGroupId);
      
    }
  }
}
```

### 広告にラベルを付与する / Apply a label to an ad
```.js
function applyLabelToAd() {
 
  const accountId = AdsUtilities.getCurrentAccountId();
  const adGroupAdLabelArray = [
    {
      adGroupId: 111111111,
      adId: 2222222222,
      campaignId: 3333333,
      labelId: 44444,
    },
    {
      adGroupId: 555555555,
      adId: 6666666666,
      campaignId: 7777777,
      labelId: 88888,
    }
  ];//Multiple selections are possible
   
  const adGroupAdLabels = Search.AdGroupAdLabelService.add({
    accountId: accountId,
    operand: adGroupAdLabelArray,
  }).rval;
   
  for (let i = 0; i < Object.keys(adGroupAdLabels.values).length; i++){
    if (adGroupAdLabels.values[i].operationSucceeded) {
      let adGroupAdLabel = adGroupAdLabels.values[i].adGroupAdLabel;
      Logger.log('labelId-> ' + adGroupAdLabel.labelId + ' have linked to adGroupId-> '
        + adGroupAdLabel.adGroupId + ', adId-> ' + adGroupAdLabel.adId);
        
    } else {
      Logger.log('labelId-> ' + adGroupAdLabelArray[i].labelId + ' could not be linked to adGroupId-> '
        + adGroupAdLabelArray[i].adGroupId + ', adId-> ' + adGroupAdLabelArray[i].adId);
      
    }
  }
}
```
