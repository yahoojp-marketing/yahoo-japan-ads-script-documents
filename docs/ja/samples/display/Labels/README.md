# ラベル / Labels

### 全てのラベル情報の取得をする / Get all labels
```.js
function getAllLabels() {
     
  const accountId = AdsUtilities.getCurrentAccountId();
  
  const labels = Display.LabelService.get({
    accountId: accountId,
  }).rval;
  
  if (labels.totalNumEntries == 0) {
    Logger.log('Label does not exist.');
    return;
  }

  for (let i = 0; i < Object.keys(labels.values).length; i++){
    let label = labels.values[i].label;
    Logger.log('labelId-> ' + label.labelId
      + ', labelName-> ' + label.labelName);
  }
}
```

### ラベルの新規追加をする / Add a label
```.js
function addLabel() {
  
  const accountId = AdsUtilities.getCurrentAccountId();
  const labelArray = [
    {
      labelName: 'labelNameAAA',
    },
    {
      color: '#FF0000',
      description: 'labelDescriptionBBB',
      labelName: 'labelNameBBB',
    }
  ];//Multiple selections are possible
  
  const labels = Display.LabelService.add({
    accountId: accountId,
    operand: labelArray,
  }).rval;
  
  for (let i = 0; i < Object.keys(labels.values).length; i++){
    if (labels.values[i].operationSucceeded) {
      let label = labels.values[i].label;
      Logger.log('labelId-> ' + label.labelId
        + ', labelName-> ' + label.labelName
        + ' have added as description-> ' + label.description
        + ', color-> ' + label.color);
          
    } else {
      Logger.log('labelName-> ' + labelArray[i].labelName + ' could not to be added');
          
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
      campaignId: 11111111,
      labelId: 2222222222,
    },
    {
      campaignId: 33333333,
      labelId: 4444444444,
    }
  ];//Multiple selections are possible
     
  const campaignLabels = Display.CampaignLabelService.add({
    accountId: accountId,
    operand: campaignLabelArray,
  }).rval;
  
  for (let i = 0; i < Object.keys(campaignLabels.values).length; i++){
    if (campaignLabels.values[i].operationSucceeded) {
      let campaignLabel = campaignLabels.values[i].campaignLabel;
      Logger.log('campaignId-> ' + campaignLabel.campaignId
        + ' linked to labelId-> ' + campaignLabel.labelId);

    } else {
      Logger.log('campaignId-> ' + campaignLabelArray[i].campaignId
        + ' could not link to labelId-> ' + campaignLabelArray[i].labelId);
        
    }
  }
}
```

### 広告グループにラベルを付与する / Apply a label to an ad group
```.js
function applyLabelToAdGroup() {
  
  const accountId = AdsUtilities.getCurrentAccountId();
  const adGroupArray = [
    {
      adGroupId: 111111111,
      campaignId: 22222222,
      labelId: 3333333333,
    },
    {
      adGroupId: 444444444,
      campaignId: 55555555,
      labelId: 6666666666,
    }
  ];//Multiple selections are possible
  
  const adGroupLabels = Display.AdGroupLabelService.add({
    accountId: accountId,
    operand: adGroupArray
  }).rval;
  
  for (let i = 0; i < Object.keys(adGroupLabels.values).length; i++){
    if (adGroupLabels.values[i].operationSucceeded) {
      let adGroupLabel = adGroupLabels.values[i].adGroupLabel;
      Logger.log('adGroupId-> ' + adGroupLabel.adGroupId
        + ', campaignId-> ' + adGroupLabel.campaignId
        + ' linked to labelId-> ' + adGroupLabel.labelId);
          
    } else {
      Logger.log('adGroupId-> ' + adGroupArray[i].adGroupId
        + ', campaignId-> ' + adGroupArray[i].campaignId
        + ' could not link to labelId-> ' + adGroupArray[i].labelId);
        
    }
  }
}
```

### 広告にラベルを付与する / Apply a label to an ad
```.js
function applyLabelToAd() {
  
  const accountId = AdsUtilities.getCurrentAccountId();
  const adGroupAdArray = [
    {
      adGroupId: 111111111,
      adId: 2222222222,
      campaignId: 33333333,
      labelId: 4444444444,
    },
    {
      adGroupId: 555555555,
      adId: 6666666666,
      campaignId: 77777777,
      labelId: 8888888888,
    }
  ];//Multiple selections are possible
  
  const adGroupAdLabels = Display.AdGroupAdLabelService.add({
    accountId: accountId,
    operand: adGroupAdArray,
  }).rval;
   
  for (let i = 0; i < Object.keys(adGroupAdLabels.values).length; i++){
    if (adGroupAdLabels.values[i].operationSucceeded) {
      let adGroupAdLabel = adGroupAdLabels.values[i].adGroupAdLabel;
      Logger.log('adGroupId-> ' + adGroupAdLabel.adGroupId
        + ', adId-> ' + adGroupAdLabel.adId
        + ' linked to labelId-> ' + adGroupAdLabel.labelId);
          
    } else {
      Logger.log('adGroupId-> ' + adGroupAdArray[i].adGroupId
        + ', adId-> ' + adGroupAdArray[i].adId
        + ' could not link to labelId-> ' + adGroupAdArray[i].labelId);
          
    }
  }
}
```

