# Labels

### Get all labels
```.js
function getAllLabels() {
     
    const accountId = AdsUtilities.getCurrentAccountId();
     
    const labels = Search.LabelService.get({
        "accountId": accountId,
    }).rval;
 
    for (let i = 0; i < labels.totalNumEntries; i++){   
        let label = labels.values[i].label;
         
        Logger.log('labelId -> ' + label.labelId + ', labelName -> ' + label.labelName);
    }
}
```

### Add a label
```.js
function addLabel() {
     
    const accountId = AdsUtilities.getCurrentAccountId();
     
    const labels = Search.LabelService.add({
        "accountId": accountId,
        "operand": [
            {
                "labelName": "AAAAAA",
            }
        ]
    }).rval;
 
    for (let i = 0; i < Object.keys(labels.values).length; i++){   
        let label = labels.values[i].label;
         
        Logger.log('labelId -> ' + label.labelId + ', labelName -> ' + label.labelName);
    }
}
```

### Apply a label to a campaign
```.js
function applyLabelToCampaign(){
 
    const accountId = AdsUtilities.getCurrentAccountId();
     
    const campaignLabels = Search.CampaignLabelService.add({
        "accountId": accountId,
        "operand": [
            {
                "campaignId": 111111,
                "labelId": 222,
            }
        ]
    }).rval;
 
    for (let i = 0; i < Object.keys(campaignLabels.values).length; i++){   
        let campaignLabel = campaignLabels.values[i].campaignLabel;
         
        Logger.log('campaignId -> ' + campaignLabel.campaignId + ', labelId -> ' + campaignLabel.labelId);
    }
}
```

### Apply a label to an ad group
```.js
function applyLabelToAdGroup(){
 
    const accountId = AdsUtilities.getCurrentAccountId();
     
    const adGroupLabels = Search.AdGroupLabelService.add({
        "accountId": accountId,
        "operand": [
            {
              "adGroupId": 111111111,
              "campaignId": 222222,
              "labelId": 333
            }
        ]
    }).rval;
     
    for (let i = 0; i < Object.keys(adGroupLabels.values).length; i++){
        let adGroupLabel = adGroupLabels.values[i].adGroupLabel;
         
        Logger.log('adGroupId -> ' + adGroupLabel.adGroupId
            + ', campaignId -> ' + adGroupLabel.campaignId
            + ', labelId -> ' + adGroupLabel.labelId);
    }
}
```

### Apply a label to an ad
```.js
function applyLabelToAd(){
 
    const accountId = AdsUtilities.getCurrentAccountId();
     
    const adGroupAdLabels = Search.AdGroupAdLabelService.add({
        "accountId": accountId,
        "operand": [
            {
              "adGroupId": 111111111,
              "adId": 222222222,
              "campaignId": 333333,
              "labelId": 444
            }
        ]
    }).rval;
     
    for (let i = 0; i < Object.keys(adGroupAdLabels.values).length; i++){
        let adGroupAdLabel = adGroupAdLabels.values[i].adGroupAdLabel;
         
        Logger.log('adGroupId -> ' + adGroupAdLabel.adGroupId
            + ', adId -> ' + adGroupAdLabel.adId
            + ', campaignId -> ' + adGroupAdLabel.campaignId
            + ', labelId -> ' + adGroupAdLabel.labelId);
    }
}
```