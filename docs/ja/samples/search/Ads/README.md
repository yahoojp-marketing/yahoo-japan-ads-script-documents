# 広告 / Ads

### テキスト広告を新規追加する / Add an expanded text ad
```.js
function addExpandedTextAd(){
     
  const accountId = AdsUtilities.getCurrentAccountId();
  
  const adGroupAdArray = [
    {
      ad: {
        adType: 'EXTENDED_TEXT_AD',
        advancedUrl: 'http://xxxxxx.co.jp',
        description1: 'First description',
        headline1: 'First headline',
        extendedTextAd: {
          headline2: 'Second headline',
        },
      },
      adGroupId: 1111111111,
      adName: 'adNameAAA',
      campaignId: 2222222,
      userStatus: 'ACTIVE',
    }
  ];//Multiple selections are possible

  const adGroupAds = Search.AdGroupAdService.add({
    accountId: accountId,
    operand: adGroupAdArray,
  }).rval;
   
  for (let i = 0; i < Object.keys(adGroupAds.values).length; i++){
    if (adGroupAds.values[i].operationSucceeded) {
      let adGroupAd = adGroupAds.values[i].adGroupAd;
      Logger.log('adId-> ' + adGroupAd.adId + ', adName-> ' + adGroupAd.adName
        + ', adType-> ' + adGroupAd.ad.adType + ' has been added.');
      
    } else {
      Logger.log('adName-> ' + adGroupAdArray[i].adName + ' could not be added.');
      
    }
  }
}
```

### レスポンシブ広告を新規追加する / Add a responsive search ad
```.js
function addResponsiveSearchAd(){
     
  const accountId = AdsUtilities.getCurrentAccountId();
  
  const adGroupAdArray = [
    {
      ad: {
        adType: 'RESPONSIVE_SEARCH_AD',
        advancedUrl: 'http://xxxxxx.co.jp',
        responsiveSearchAd: {
          headlines: [//3 or more and less than 15
            {
              text: 'First headline',
            },
            {
              text: 'Second headline',
            },
            {
              text: 'Third headline',
            }
          ],
          descriptions: [//2 or more and less than 4
            {
              text: 'First description',
            },
            {
              text: 'Second description',
            }
          ],
        },
      },
      adGroupId: 1111111111,
      adName: 'adNameAAA',
      campaignId: 2222222,
      userStatus: 'ACTIVE',
    }
  ];//Multiple selections are possible

  const adGroupAds = Search.AdGroupAdService.add({
    accountId: accountId,
    operand: adGroupAdArray,
  }).rval;
   
  for (let i = 0; i < Object.keys(adGroupAds.values).length; i++){
    if (adGroupAds.values[i].operationSucceeded) {
      let adGroupAd = adGroupAds.values[i].adGroupAd;
      Logger.log('adId-> ' + adGroupAd.adId + ', adName-> ' + adGroupAd.adName
        + ', adType-> ' + adGroupAd.ad.adType + ' has been added.');
        
    } else {
      Logger.log('adName-> ' + adGroupAdArray[i].adName + ' could not be added.');
      
    }
  }
}
```

### 指定した広告グループ配下の広告を配信停止にする / Pause ads in an ad group
```.js
function pauseAdsInAdGroup(){
  
  const accountId = AdsUtilities.getCurrentAccountId();
  const adGroupIds = [111111111, 222222222];//Empty when not specified
  
  const adGroupAdsGet = Search.AdGroupAdService.get({
    accountId: accountId,
    adGroupIds: adGroupIds,
    userStatuses: ['ACTIVE'],
  }).rval;
  
  if (adGroupAdsGet.totalNumEntries == 0) {
    Logger.log('Target ID does not exist.');
    return;
  }
  
  let adGroupAdArray = [];
  for (let i = 0; i < Object.keys(adGroupAdsGet.values).length; i++) {
    let adGroupAd = adGroupAdsGet.values[i].adGroupAd;
    adGroupAd.userStatus = 'PAUSED';
    adGroupAdArray.push(adGroupAd);
  }
  
  const adGroupAdsSet = Search.AdGroupAdService.set({
    accountId: accountId,
    operand: adGroupAdArray,
  }).rval;
  
  for (let i = 0; i < Object.keys(adGroupAdsSet.values).length; i++) {
    if (adGroupAdsSet.values[i].operationSucceeded) {
      let adGroupAd = adGroupAdsSet.values[i].adGroupAd;
      Logger.log('adId-> ' + adGroupAd.adId 
        + ', adName-> ' + adGroupAd.adName
        + ', adGroupId-> ' + adGroupAd.adGroupId 
        + ', adGroupName-> ' + adGroupAd.adGroupName + ' has been paused.');
    
    } else {
      let adGroupAd = adGroupAdsGet.values[i].adGroupAd;
      Logger.log('adName-> ' + adGroupAd.adName 
        + ', adGroupName-> ' + adGroupAd.adGroupName + ' could not be stopped.');
    
    }
  }
}
```

### 全ての広告情報を取得する / Get all ads
```.js
function getAllAds(){
  
  const accountId = AdsUtilities.getCurrentAccountId();
  
  const adGroupAds = Search.AdGroupAdService.get({
    accountId: accountId,
    numberResults: 10000,//Max ads you can get is 10000.
  }).rval;
  
  if (adGroupAds.totalNumEntries == 0) {
    Logger.log('Ad does not exist.');
    return;
  }
   
  for (let i = 0; i < Object.keys(adGroupAds.values).length; i++){
    let adGroupAd = adGroupAds.values[i].adGroupAd;
    Logger.log('adGroupId-> ' + adGroupAd.adGroupId 
      + ', adGroupName-> ' + adGroupAd.adGroupName
      + ', adId-> ' + adGroupAd.adId 
      + ', adName-> ' + adGroupAd.adName);
  }
}
```

### 指定した全ての広告情報を取得する / Get all ads by id
```.js
function getAllAdsById(){
  
  const accountId = AdsUtilities.getCurrentAccountId();
  const adIds = [1111111111, 2222222222];//Multiple selections are possible
  
  const adGroupAds = Search.AdGroupAdService.get({
    accountId: accountId,
    adIds: adIds,
  }).rval;
  
  if (adGroupAds.totalNumEntries == 0) {
    Logger.log('Target ID does not exist.');
    return;
  }
  
  for (let i = 0; i < Object.keys(adGroupAds.values).length; i++){
    let adGroupAd = adGroupAds.values[i].adGroupAd;
    Logger.log('adGroupId-> ' + adGroupAd.adGroupId 
      + ', adGroupName-> ' + adGroupAd.adGroupName
      + ', adId-> ' + adGroupAd.adId 
      + ', adName-> ' + adGroupAd.adName);
  }
}
```

### 指定した広告グループ配下のテキスト広告情報を取得する / Get expanded text ads in an ad group
```.js
function getExpandedTextAdsInAdGroup(){
  
  const accountId = AdsUtilities.getCurrentAccountId();
  const adGroupIds = [111111111, 222222222];//Multiple selections are possible
  
  const adGroupAds = Search.AdGroupAdService.get({
    accountId: accountId,
    adGroupIds: adGroupIds,
    adTypes: ['EXTENDED_TEXT_AD'],
  }).rval;
  
  if (adGroupAds.totalNumEntries == 0) {
    Logger.log('Target ID does not exist.');
    return;
  }
  
  for (let i = 0; i < Object.keys(adGroupAds.values).length; i++){
    let adGroupAd = adGroupAds.values[i].adGroupAd;
    let ad = adGroupAd.ad;
     
    Logger.log('adGroupId-> ' + adGroupAd.adGroupId 
      + ', adGroupName-> ' + adGroupAd.adGroupName
      + ', adId-> ' + adGroupAd.adId 
      + ', adName-> ' + adGroupAd.adName
      + ', advancedUrl-> ' + ad.advancedUrl 
      + ', description1-> ' + ad.description1
      + ', headline1-> ' + ad.headline1 
      + ', headline2-> ' + ad.extendedTextAd.headline2);
  }
}
```

### 指定した広告グループ配下のレスポンシブ広告情報を取得する / Get responsive search ad in an ad group
```.js
function getResponsiveSearchAdInAdGroup(){
     
  const accountId = AdsUtilities.getCurrentAccountId();
  const adGroupIds = [111111111, 222222222];//Multiple selections are possible
  
  const adGroupAds = Search.AdGroupAdService.get({
    accountId: accountId,
    adGroupIds: adGroupIds,
    adTypes: ['RESPONSIVE_SEARCH_AD'],
  }).rval;
  
  if (adGroupAds.totalNumEntries == 0) {
    Logger.log('Target ID does not exist.');
    return;
  }
   
  for (let i = 0; i < Object.keys(adGroupAds.values).length; i++){
    let adGroupAd = adGroupAds.values[i].adGroupAd;
    
    Logger.log('adGroupId-> ' + adGroupAd.adGroupId  
      + ', adGroupName-> ' + adGroupAd.adGroupName
      + ', adId-> ' + adGroupAd.adId + ', adName-> ' 
      + adGroupAd.adName + ', advancedUrl-> ' + adGroupAd.ad.advancedUrl);
    
    let responsiveSearchAd = adGroupAd.ad.responsiveSearchAd;
    let headlines = [];
    let descriptions = [];
    
    for (let j = 0; j < responsiveSearchAd.headlines.length; j++){
      headlines.push('headline' + (j + 1) + '-> ' 
        + responsiveSearchAd.headlines[j].text);
    }
    Logger.log('***' + headlines.join(', '));
    
    for (let j = 0; j < responsiveSearchAd.descriptions.length; j++){
      descriptions.push('description' + (j + 1) + '-> ' 
        + responsiveSearchAd.descriptions[j].text);
    }
    Logger.log('***' + descriptions.join(', '));
  }
}
```
