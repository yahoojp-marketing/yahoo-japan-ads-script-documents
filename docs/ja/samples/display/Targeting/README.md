# ターゲティング / Targeting

### 地域ターゲティングと入札価格調整率の更新をする / Set location and bid modifiers
```.js
function setLocationAndBidModifiers(){
 
    let targetId;
      
    const dictionaries = Display.DictionaryService.getGeographicLocation({
        "lang": "JA",
    }).rval;
      
    for (let i = 0; i < dictionaries.totalNumEntries; i++){
        let geographicLocation = dictionaries.values[i].geographicLocation;
         
        if(geographicLocation.fullName == "北海道"){
            targetId = geographicLocation.code;
            break;
        }
    }
     
    const accountId = AdsUtilities.getCurrentAccountId();
 
    const adGroupTargets = Display.AdGroupTargetService.add({
        "accountId": accountId,
        "operand": [
            {
                "adGroupId": 209780511,
                "bidMultiplier": 1.5,
                "campaignId": 27462571,
                "target": {
                    "targetId": targetId,
                    "targetType": "GEO_TARGET"
                }
            }
        ]
    }).rval;
 
    for (let i = 0; i < Object.keys(adGroupTargets.values).length; i++){
        let adGroupTargetList = adGroupTargets.values[i].adGroupTargetList;
         
        Logger.log('adGroupId -> ' + adGroupTargetList.adGroupId
            + ', campaignId -> ' + adGroupTargetList.campaignId
            + ', geoNameJa -> ' + adGroupTargetList.target.geoTarget.geoNameJa
            + ', targetId -> ' + adGroupTargetList.target.targetId
            + ', targetType -> ' + adGroupTargetList.target.targetType
            + ', bidMultiplier -> ' + adGroupTargetList.bidMultiplier);
    }
}
```

### デバイスターゲティングと入札価格調整率の更新をする / Set device and bid modifiers
```.js
function setDeviceAndBidModifiers(){
 
    const accountId = AdsUtilities.getCurrentAccountId();
       
    const adGroupTargetsGet = Display.AdGroupTargetService.get({
        "accountId": accountId,
        "adGroupIds": [
            209780553, 209780551, 209780518,//Multiple selections are possible
        ],
        "campaignIds": [
            27462571
        ],
        "targetTypes": [
            "DEVICE_TARGET"
        ]
    }).rval;
 
    let adGroupTargetArray = [];
 
    for (let i = 0; i < adGroupTargetsGet.totalNumEntries; i++){
        let adGroupTargetList = adGroupTargetsGet.values[i].adGroupTargetList;
         
        switch (adGroupTargetList.target.deviceTarget.deviceType) {
            case "DESKTOP":
                adGroupTargetList.bidMultiplier = 1.0;
                break;
            case "SMARTPHONE":
                adGroupTargetList.bidMultiplier = 1.5;
                break;
            case "TABLET":
                adGroupTargetList.bidMultiplier = 2.0;
                break;
            default:
                break;
        }
        adGroupTargetArray.push(adGroupTargetList);
    }
 
    const adGroupTargetsSet = Display.AdGroupTargetService.set({
        "accountId": accountId,
        "operand": adGroupTargetArray,
    }).rval;
     
    for (let i = 0; i < Object.keys(adGroupTargetsSet.values).length; i++){
        let adGroupTargetList = adGroupTargetsSet.values[i].adGroupTargetList;
         
        Logger.log('adGroupId -> ' + adGroupTargetList.adGroupId
            + ', campaignId -> ' + adGroupTargetList.campaignId
            + ', bidMultiplier -> ' + adGroupTargetList.bidMultiplier
            + ', targetId -> ' + adGroupTargetList.target.targetId
            + ', deviceType -> ' + adGroupTargetList.target.deviceTarget.deviceType
            + ', targetType -> ' + adGroupTargetList.target.targetType);
    }
}
```

### 曜日時間帯ターゲティングと入札価格調整率の更新をする / Set schedule and bid modifiers
```.js
function setScheduleAndBidModifiers(){
     
    const accountId = AdsUtilities.getCurrentAccountId();
 
    const adGroupTargetsGet = Display.AdGroupTargetService.get({
        "accountId": accountId,
        "targetTypes": [
            "AD_SCHEDULE_TARGET"
        ]
    }).rval;
 
    let adGroupTargetArray = [];
 
    for (let i = 0; i < adGroupTargetsGet.totalNumEntries; i++){
        let adGroupTargetList = adGroupTargetsGet.values[i].adGroupTargetList;
 
        switch (adGroupTargetList.target.adScheduleTarget.dayOfWeek) {
            case "MONDAY":
                adGroupTargetList.bidMultiplier = 1.0;
                break;
            case "TUESDAY":
                adGroupTargetList.bidMultiplier = 1.5;
                break;
            case "WEDNESDAY":
                adGroupTargetList.bidMultiplier = 2.0;
                break;
            default:
                adGroupTargetList.bidMultiplier = 2.5;
                break;
        }
         
        adGroupTargetArray.push(adGroupTargetList);
    }
 
    const adGroupTargetsSet = Display.AdGroupTargetService.set({
        "accountId": accountId,
        "operand": adGroupTargetArray
    }).rval;
 
    for (let i = 0; i < Object.keys(adGroupTargetsSet.values).length; i++){
        let adGroupTargetList = adGroupTargetsSet.values[i].adGroupTargetList;
         
        Logger.log('adGroupId -> ' + adGroupTargetList.adGroupId
            + ', campaignId -> ' + adGroupTargetList.campaignId
            + ', dayOfWeek -> ' + adGroupTargetList.target.adScheduleTarget.dayOfWeek
            + ', targetType -> ' + adGroupTargetList.target.targetType
            + ', bidMultiplier -> ' + adGroupTargetList.bidMultiplier);
    }
}
```

### 年齢ターゲティングと入札価格調整率の更新をする / Set age and bid modifiers
```.js
function setAgeAndBidModifiers(){
     
    const accountId = AdsUtilities.getCurrentAccountId();
 
    const adGroupTargetsGet = Display.AdGroupTargetService.get({
        "accountId": accountId,
        "targetTypes": [
            "AGE_TARGET"
        ]
    }).rval;
     
    let adGroupTargetArray = [];
 
    for (let i = 0; i < adGroupTargetsGet.totalNumEntries; i++){
        let adGroupTargetList = adGroupTargetsGet.values[i].adGroupTargetList;
 
        switch (adGroupTargetList.target.ageTarget.age) {
            case "GT_RANGE20_24":
                adGroupTargetList.bidMultiplier = 1.2;
                break;
            case "GT_RANGE25_29":
                adGroupTargetList.bidMultiplier = 1.5;
                break;
            case "GT_RANGE30_34":
                adGroupTargetList.bidMultiplier = 2.0;
                break;
            default:
                adGroupTargetList.bidMultiplier = 1.0;
                break;
        }
         
        adGroupTargetArray.push(adGroupTargetList);
    }
     
    const adGroupTargetsSet = Display.AdGroupTargetService.set({
        "accountId": accountId,
        "operand": adGroupTargetArray
    }).rval;
 
    for (let i = 0; i < Object.keys(adGroupTargetsSet.values).length; i++){
        let adGroupTargetList = adGroupTargetsSet.values[i].adGroupTargetList;
         
        Logger.log('adGroupId -> ' + adGroupTargetList.adGroupId
            + ', campaignId -> ' + adGroupTargetList.campaignId
            + ', age -> ' + adGroupTargetList.target.ageTarget.age
            + ', estimateFlg -> ' + adGroupTargetList.target.ageTarget.estimateFlg
            + ', targetType -> ' + adGroupTargetList.target.targetType
            + ', bidMultiplier -> ' + adGroupTargetList.bidMultiplier);
    }
}
```
