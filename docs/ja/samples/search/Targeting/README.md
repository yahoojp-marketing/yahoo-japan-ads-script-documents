# ターゲティング / Targeting

### 地域ターゲティングと入札価格調整率を更新する / Set location and bid modifiers
```.js
function setLocationAndBidModifiers() {

  const dictionaries = Search.DictionaryService.getGeographicLocation({
    lang: 'JA',
  }).rval;
  
  const geoName = '東京都';
  
  let targetId;
  for (let i = 0; i < dictionaries.totalNumEntries; i++){
    let geographicLocation = dictionaries.values[i].geographicLocation;
    if(geographicLocation.fullName == geoName){
      targetId = geographicLocation.code;
      break;
    }
  }
  if (targetId == undefined) {
    Logger.log('code of ' + geoName + ' is not found');
    return;
  }
 
  const accountId = AdsUtilities.getCurrentAccountId();
  
  const campaignTargetArray = [
    {
      accountId: accountId,
      bidMultiplier: 1.50,
      campaignId: 1111111,
      target: {
        locationTarget: {
          excludedType: 'INCLUDED',
        },
        targetId: targetId,
        targetType: 'LOCATION'
      }
    },
    {
      accountId: accountId,
      bidMultiplier: 1.20,
      campaignId: 2222222,
      target: {
        locationTarget: {
          excludedType: 'EXCLUDED',
        },
        targetId: targetId,
        targetType: 'LOCATION'
      }
    }
  ];//Multiple selections are possible
   
  const campaignTargets = Search.CampaignTargetService.add({
    accountId: accountId,
    operand: campaignTargetArray,
  }).rval;
   
  for (let i = 0; i < Object.keys(campaignTargets.values).length; i++){
    if (campaignTargets.values[i].operationSucceeded) {
      let campaignTarget = campaignTargets.values[i].campaignTarget;
      Logger.log('campaignId-> ' + campaignTarget.campaignId + ', campaignName-> ' + campaignTarget.campaignName
        + ' set LocationTarget as geoName-> ' + geoName + ', excludedType-> '
        + campaignTarget.target.locationTarget.excludedType + ', bidMultiplier->' + campaignTarget.bidMultiplier);
        
    } else {
      Logger.log('campaignId-> ' + campaignTargetArray[i].campaignId + ' could not set LocationTarget as geoName-> '
      + geoName + ', bidMultiplier-> ' + campaignTargetArray[i].bidMultiplier
      + ', excludedType-> ' + campaignTargetArray[i].target.locationTarget.excludedType);

    }
  }
}
```

### デバイスターゲティングと入札価格調整率を更新する / Set device and bid modifiers
```.js
function setDeviceAndBidModifiers() {
   
  const accountId = AdsUtilities.getCurrentAccountId();
  const campaignIds = [1111111, 2222222];//Empty when not specified

  const campaignTargetsGet = Search.CampaignTargetService.get({
    accountId: accountId,
    campaignIds: campaignIds,
    targetTypes: ['PLATFORM'],
  }).rval;
  
  if (campaignTargetsGet.totalNumEntries == 0) {
    Logger.log('Target ID of PLATFORM does not exist.');
    return;
  }
   
  let campaignTargetArray = [];
  for (let i = 0; i < Object.keys(campaignTargetsGet.values).length; i++){
    let campaignTarget = campaignTargetsGet.values[i].campaignTarget;
    switch(campaignTarget.target.platformTarget.platformType){
      case 'SMART_PHONE':
        campaignTarget.bidMultiplier = 1.0;//0: stop Ad.
        break;
      case 'TABLET':
        campaignTarget.bidMultiplier = 1.2;
        break;
      case 'DESKTOP':
        campaignTarget.bidMultiplier = 1.5;
        break;
      default:
        break;
    }
    campaignTargetArray.push(campaignTarget);
  }
   
  const campaignTargetsSet = Search.CampaignTargetService.set({
    accountId: accountId,
    operand: campaignTargetArray,
  }).rval;
   
  for (let i = 0; i < Object.keys(campaignTargetsSet.values).length; i++){
    if (campaignTargetsSet.values[i].operationSucceeded) {
      let campaignTarget = campaignTargetsSet.values[i].campaignTarget;
      Logger.log('campaignId-> ' + campaignTarget.campaignId + ', campaignName-> ' + campaignTarget.campaignName
        + ' set PlatformTarget as platformType-> ' + campaignTarget.target.platformTarget.platformType
        + ', bidMultiplier-> ' + campaignTarget.bidMultiplier);
        
    } else {
      Logger.log('campaignId-> ' + campaignTargetArray[i].campaignId + ', campaignName-> ' + campaignTargetArray[i].campaignName
        + ' could not set PlatformTarget as platformType-> ' + campaignTargetArray[i].target.platformTarget.platformType
        + ', bidMultiplier-> ' + campaignTargetArray[i].bidMultiplier);
        
    }
  }
}
``` 

### 曜日時間帯ターゲティングと入札価格調整率を更新する / Set schedule and bid modifiers
```.js
function setScheduleAndBidModifiers() {
   
  const accountId = AdsUtilities.getCurrentAccountId();
  const campaignTargetArray = [
    {
      accountId: accountId,
      bidMultiplier: 1.50,//default:1.00
      campaignId: 1111111,
      target: {
        scheduleTarget: {
          dayOfWeek: 'MONDAY',
          endHour: 21,
          endMinute: 'FIFTEEN',
          startHour: 8,
          startMinute: 'FORTY_FIVE'
        },
        targetType: 'SCHEDULE'
      }
    },
    {
      accountId: accountId,
      campaignId: 2222222,
      target: {
        scheduleTarget: {
          dayOfWeek: 'SUNDAY',
          endHour: 22,
          endMinute: 'ZERO',
          startHour: 7,
          startMinute: 'THIRTY'
        },
        targetType: 'SCHEDULE'
      }
    }
  ];//Multiple selections are possible
   
  const campaignTargets = Search.CampaignTargetService.add({
    accountId: accountId,
    operand: campaignTargetArray,
  }).rval;
   
  for (let i = 0; i < Object.keys(campaignTargets.values).length; i++){
    if (campaignTargets.values[i].operationSucceeded) {
      let campaignTarget = campaignTargets.values[i].campaignTarget;
      Logger.log('campaignId-> ' + campaignTarget.campaignId + ', campaignName-> ' + campaignTarget.campaignName
        + ' set ScheduleTarget as dayOfWeek-> ' + campaignTarget.target.scheduleTarget.dayOfWeek
        + ', bidMultiplier-> ' + campaignTarget.bidMultiplier);
        
    } else {
      Logger.log('campaignId-> ' + campaignTargetArray[i].campaignId
        + ' could not set ScheduleTarget as dayOfWeek-> ' + campaignTargetArray[i].target.scheduleTarget.dayOfWeek
        + ', bidMultiplier-> ' + campaignTargetArray[i].bidMultiplier);
        
    }
  }
}
```
