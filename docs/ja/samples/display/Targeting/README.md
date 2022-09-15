# ターゲティング / Targeting

### 地域ターゲティングと入札価格調整率の更新をする / Set location and bid modifiers
```.js
function setLocationAndBidModifiers() {

  const dictionaries = Display.DictionaryService.getGeographicLocation({
    lang: 'JA',
  }).rval;

  const geoName = '東京都';

  let targetId;
  for (let i = 0; i < dictionaries.totalNumEntries; i++){
    let geographicLocation = dictionaries.values[i].geographicLocation;
    if (geographicLocation.fullName == geoName){
      targetId = geographicLocation.code;
      break;
    }
  }

  if (targetId == undefined) {
    Logger.log('code of ' + geoName + ' is not found');
    return;
  }
  
  const accountId = AdsUtilities.getCurrentAccountId();

  const adGroupTargetArray = [
    {
      adGroupId: 111111111,
      campaignId: 22222222,
        target: {
          targetId: targetId,
          targetType: 'GEO_TARGET',
        }
    },
    {
      adGroupId: 333333333,
      bidMultiplier: 1.5,
      campaignId: 44444444,
        target: {
          targetId: targetId,
          targetType: 'GEO_TARGET',
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
        + ' set as geoNameJa-> ' + adGroupTargetList.target.geoTarget.geoNameJa
        + ', targetId-> ' + adGroupTargetList.target.targetId
        + ', targetType-> ' + adGroupTargetList.target.targetType
        + ', bidMultiplier-> ' + adGroupTargetList.bidMultiplier);
      
    } else {
      Logger.log('adGroupId-> ' + adGroupTargetArray[i].adGroupId
        + ', campaignId-> ' + adGroupTargetArray[i].campaignId
        + ' could not set as geoNameJa-> ' + geoName
        + ', targetId-> ' + adGroupTargetArray[i].target.targetId
        + ', targetType-> ' + adGroupTargetArray[i].target.targetType);
        
    }
  }
}
```

### デバイスターゲティングと入札価格調整率の更新をする / Set device and bid modifiers
```.js
function setDeviceAndBidModifiers() {

  const accountId = AdsUtilities.getCurrentAccountId();
  const adGroupIds = [111111111, 222222222, 333333333];//Empty when not specified
  const devices = ['DESKTOP', 'SMARTPHONE', 'TABLET'];//Multiple selections are possible

  const adGroupsGet = Display.AdGroupService.get({
    accountId: accountId,
    adGroupIds: adGroupIds,
  }).rval;

  if (adGroupsGet.totalNumEntries == 0) {
    Logger.log('AdGroup does not exist.');
    return;
  }

  let adGroupArray = [];
  for (let i = 0; i < Object.keys(adGroupsGet.values).length; i++) {
    let adGroup = adGroupsGet.values[i].adGroup;
    adGroup.device = devices;
    adGroupArray.push(adGroup);
  }

  Display.AdGroupService.set({
    accountId: accountId,
    operand: adGroupArray,
  }).rval;

  const adGroupTargetsGet = Display.AdGroupTargetService.get({
    accountId: accountId,
    adGroupIds: adGroupIds,
    targetTypes: ['DEVICE_TARGET'],
  }).rval;
  
  if (adGroupTargetsGet.totalNumEntries == 0) {
    Logger.log('AdGroupTarget does not exist.');
    return;
  }
 
  let adGroupTargetArray = [];
  for (let i = 0; i < adGroupTargetsGet.totalNumEntries; i++){
    let adGroupTargetList = adGroupTargetsGet.values[i].adGroupTargetList;
    
    switch (adGroupTargetList.target.deviceTarget.deviceType) {
      case 'DESKTOP':
        adGroupTargetList.bidMultiplier = 1.0;
        break;
      case 'SMARTPHONE':
        adGroupTargetList.bidMultiplier = 1.5;
        break;
      case 'TABLET':
        adGroupTargetList.bidMultiplier = 2.0;
        break;
      default:
        break;
    }
    adGroupTargetArray.push(adGroupTargetList);
  }
 
  const adGroupTargetsSet = Display.AdGroupTargetService.set({
    accountId: accountId,
    operand: adGroupTargetArray,
  }).rval;
  
  for (let i = 0; i < Object.keys(adGroupTargetsSet.values).length; i++) {
    if (adGroupTargetsSet.values[i].operationSucceeded) {
      let adGroupTargetList = adGroupTargetsSet.values[i].adGroupTargetList;
      Logger.log('adGroupId-> ' + adGroupTargetList.adGroupId
        + ', campaignId-> ' + adGroupTargetList.campaignId
        + ' have set to bidMultiplier-> ' + adGroupTargetList.bidMultiplier
        + ', deviceType-> ' + adGroupTargetList.target.deviceTarget.deviceType);

    } else {
      let adGroupTargetList = adGroupTargetsGet.values[i].adGroupTargetList;
      Logger.log('adGroupId-> ' + adGroupTargetList.adGroupId
        + ', campaignId-> ' + adGroupTargetList.campaignId
        + ' could not to set to bidMultiplier-> ' + adGroupTargetList.bidMultiplier
        + ', deviceType-> ' + adGroupTargetList.target.deviceTarget.deviceType);
        
    }
  }
}
```

### 曜日時間帯ターゲティングと入札価格調整率の更新をする / Set schedule and bid modifiers
```.js
function setScheduleAndBidModifiers() {
  
  const accountId = AdsUtilities.getCurrentAccountId();
  
  const adGroupTargetArray = [
    {
      adGroupId: 111111111,
      bidMultiplier: 1.2,
      campaignId: 22222222,
      target: {
        adScheduleTarget: {
          dayOfWeek: 'MONDAY',
          startHour: 12,
          endHour: 15,
        },
        targetType: 'AD_SCHEDULE_TARGET',
      },
    },
    {
      adGroupId: 333333333,
      bidMultiplier: 1.5,
      campaignId: 44444444,
      target: {
        adScheduleTarget: {
          dayOfWeek: 'SUNDAY',
          startHour: 17,
          endHour: 18,
        },
        targetType: 'AD_SCHEDULE_TARGET',
      },
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
        + ' have set to dayOfWeek-> ' + adGroupTargetList.target.adScheduleTarget.dayOfWeek
        + ', Hour->' + adGroupTargetList.target.adScheduleTarget.startHour 
        + '-' + adGroupTargetList.target.adScheduleTarget.endHour
        + ', bidMultiplier-> ' + adGroupTargetList.bidMultiplier);

    } else {
      let adScheduleTarget = adGroupTargetArray[i].target.adScheduleTarget;
      Logger.log('adGroupId-> ' + adGroupTargetArray[i].adGroupId
        + ', campaignId-> ' + adGroupTargetArray[i].campaignId
        + ' could not to set to dayOfWeek-> ' + adScheduleTarget.dayOfWeek
        + ', Hour->' + adScheduleTarget.startHour + '-' + adScheduleTarget.endHour
        + ', bidMultiplier-> ' + adGroupTargetArray[i].bidMultiplier);
    }
  }
}
```

### 年齢ターゲティングと入札価格調整率の更新をする / Set age and bid modifiers
```.js
function setAgeAndBidModifiers() {
  
  const accountId = AdsUtilities.getCurrentAccountId();

  const adGroupTargetArray = [
    {
      adGroupId: 111111111,
      bidMultiplier: 1.2,
      campaignId: 22222222,
      target: {
        ageTarget: {
          age: 'GT_RANGE20_24',
        },
        targetType: 'AGE_TARGET',
      },
    },
    {
      adGroupId: 333333333,
      bidMultiplier: 1.5,
      campaignId: 44444444,
      target: {
        ageTarget: {
          age: 'GT_RANGE70_UL2',
        },
        targetType: 'AGE_TARGET',
      },
    }
  ];//Multiple selections are possible
  
  const adGroupTargets = Display.AdGroupTargetService.add({
    accountId: accountId,
    operand: adGroupTargetArray,
  }).rval;

  for (let i = 0; i < Object.keys(adGroupTargets.values).length; i++) {
    if (adGroupTargets.values[i].operationSucceeded) {
      let adGroupTargetList = adGroupTargets.values[i].adGroupTargetList;
      let age = adGroupTargetList.target.ageTarget.age;
      let ageRange = 'UNKNOWN';
      if (age == 'GT_RANGE70_UL2') {
        ageRange = '70-';
      } else if (age.indexOf('GT_RANGE') >= 0) {
        ageRange = age.replace('GT_RANGE', '').replace('_', '-');
      }
      
      Logger.log('adGroupId-> ' + adGroupTargetList.adGroupId
        + ', campaignId-> ' + adGroupTargetList.campaignId
        + ' have set to age-> ' + ageRange
        + ', bidMultiplier-> ' + adGroupTargetList.bidMultiplier);

    } else {
      let age = adGroupTargetArray[i].target.ageTarget.age;
      let ageRange = 'UNKNOWN';
      if (age == 'GT_RANGE70_UL2') {
        ageRange = '70-';
      } else if (age.indexOf('GT_RANGE') >= 0) {
        ageRange = age.replace('GT_RANGE', '').replace('_', '-');
      }
      
      Logger.log('adGroupId-> ' + adGroupTargetArray[i].adGroupId
        + ', campaignId-> ' + adGroupTargetArray[i].campaignId
        + ' could not to set to age-> ' + ageRange
        + ', bidMultiplier-> ' + adGroupTargetArray[i].bidMultiplier);
    }
  }
}
```
