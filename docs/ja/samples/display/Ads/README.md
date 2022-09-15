# 広告 / Ads

### テキスト広告を新規追加する / Add a text ad
```.js
function addTextAd() {

  const accountId = AdsUtilities.getCurrentAccountId();
  const adGroupAdArray = [
    {
      accountId: accountId,
      ad: {
        adType: 'TEXT_LONG_AD1',
        textAd: {
          description: 'descriptionAAA',
          displayUrlLevel: 'DOMAIN',
          finalUrl: 'http://xxxxx.co.jp',
          headline: 'headlineAAA',
        }
      },
      adGroupId: 111111111,
      adName: 'adNameAAA',
      campaignId: 22222222,
      userStatus: 'ACTIVE',
    }
  ];//Multiple selections are possible

  const adGroupAds = Display.AdGroupAdService.add({
    accountId: accountId,
    operand: adGroupAdArray,
  }).rval;
     
  for (let i = 0; i < Object.keys(adGroupAds.values).length; i++) {
    if (adGroupAds.values[i].operationSucceeded) {
      let adGroupAd = adGroupAds.values[i].adGroupAd;
      Logger.log('adId-> ' + adGroupAd.adId + ', adName-> ' + adGroupAd.adName 
        + ' be added as headline-> ' + adGroupAd.ad.textAd.headline + ', description-> ' + adGroupAd.ad.textAd.description 
        + ' to adGroupId-> ' + adGroupAd.adGroupId + ', adGroupName-> ' + adGroupAd.adGroupName);
        
    } else {
      Logger.log('adName-> ' + adGroupAdArray[i].adName
        + ' could not to be added as headline-> ' + adGroupAdArray[i].ad.textAd.headline
        + ', description-> ' + adGroupAdArray[i].ad.textAd.description + ' to adGroupId-> ' + adGroupAdArray[i].adGroupId);
        
    }
  } 
}
```

### 画像広告を新規追加する / Add an image ad
```.js
function addImageAd() {
     
  const accountId = AdsUtilities.getCurrentAccountId();
  const adGroupAdArray = [
    {
      accountId: accountId,
      ad: {
        adType: 'BANNER_IMAGE_AD',
        bannerImageAd: {
          displayUrlLevel: 'DOMAIN',
          finalUrl: 'http://xxxxx.co.jp'
        },
      },
      adGroupId: 111111111,
      adName: 'adNameAAA',
      campaignId: 22222222,
      mediaId: 3333333,
      userStatus: 'ACTIVE',
    }
  ];//Multiple selections are possible
     
  const adGroupAds = Display.AdGroupAdService.add({
    accountId: accountId,
    operand: adGroupAdArray,
  }).rval;
     
  for (let i = 0; i < Object.keys(adGroupAds.values).length; i++){
    if (adGroupAds.values[i].operationSucceeded) {
      let adGroupAd = adGroupAds.values[i].adGroupAd;
      Logger.log('adName-> ' + adGroupAd.adName + ', adId-> ' + adGroupAd.adId + ', mediaId-> ' + adGroupAd.mediaId
        + ' be added to adGroupId-> ' + adGroupAd.adGroupId + ', adGroupName-> ' + adGroupAd.adGroupName);
        
    } else {
      Logger.log('adName-> ' + adGroupAdArray[i].adName 
        + ' could not to be added to adGroupId-> ' + adGroupAdArray[i].adGroupId);
        
    }
  } 
}
```

### 広告グループ配下の広告を配信停止にする / Pause ads in an ad group
```.js
function pauseAdsInAdGroup() {
     
  const accountId = AdsUtilities.getCurrentAccountId();
  const adGroupIds = [111111111, 222222222];//Multiple selections are possible
     
  const adGroupAdsGet = Display.AdGroupAdService.get({
    accountId: accountId,
    adGroupIds: adGroupIds,
  }).rval;
  
  if (adGroupAdsGet.totalNumEntries == 0) {
    Logger.log('Target ID does not exist.');
    return;
  }
  
  let adGroupAdArray = [];
  for (let i = 0; i < Object.keys(adGroupAdsGet.values).length; i++){
    let adGroupAd = adGroupAdsGet.values[i].adGroupAd;
    adGroupAd.userStatus = 'PAUSED';
    adGroupAdArray.push(adGroupAd);
  }
     
  const adGroupAdsSet = Display.AdGroupAdService.set({
    accountId: accountId,
    operand: adGroupAdArray,
  }).rval;
     
  for (let i = 0; i < Object.keys(adGroupAdsSet.values).length; i++){
    if (adGroupAdsSet.values[i].operationSucceeded) {
      let adGroupAd = adGroupAdsSet.values[i].adGroupAd;
      Logger.log('adGroupId-> ' + adGroupAd.adGroupId + ', adGroupName-> ' + adGroupAd.adGroupName
        + ', adName-> ' + adGroupAd.adName + ', adId-> ' + adGroupAd.adId + ' have been stopped.');

    } else {
      let adGroupAd = adGroupAdsGet.values[i].adGroupAd;
      Logger.log('adGroupId-> ' + adGroupAd.adGroupId + ', adGroupName-> ' + adGroupAd.adGroupName
        + ', adName-> ' + adGroupAd.adName + ', adId-> ' + adGroupAd.adId + ' could not to be stopped.');

    }
  }
}
```

### 全ての広告情報を取得する / Get all ads
```.js
function getAllAds() {
 
  const accountId = AdsUtilities.getCurrentAccountId();
  
  const adGroupAds = Display.AdGroupAdService.get({
    accountId: accountId,
  }).rval;

  if (adGroupAds.totalNumEntries == 0) {
    Logger.log('Target ID does not exist.');
    return;
  }
  
  for (let i = 0; i < Object.keys(adGroupAds.values).length; i++){
    let adGroupAd = adGroupAds.values[i].adGroupAd;
    Logger.log('adType-> ' + adGroupAd.ad.adType + ', adStyle-> ' + adGroupAd.adStyle
      + ', adGroupId-> ' + adGroupAd.adGroupId + ', adGroupName-> ' + adGroupAd.adGroupName
      + ', adId-> ' + adGroupAd.adId + ', adName-> ' + adGroupAd.adName
      + ', mediaId-> ' + adGroupAd.mediaId);
  }
}
```

### 指定の広告情報を取得する / Get all ads by id
```.js
function getAllAdsById() {
    
  const accountId = AdsUtilities.getCurrentAccountId();
  const adIds = [1111111111, 2222222222];//Multiple selections are possible
     
  const adGroupAds = Display.AdGroupAdService.get({
    accountId: accountId,
    adIds: adIds,
  }).rval;
 
  for (let i = 0; i < Object.keys(adGroupAds.values).length; i++){
    let adGroupAd = adGroupAds.values[i].adGroupAd;
    Logger.log('adType-> ' + adGroupAd.ad.adType + ', adStyle-> ' + adGroupAd.adStyle
      + ', adGroupId-> ' + adGroupAd.adGroupId + ', adGroupName-> ' + adGroupAd.adGroupName
      + ', adId-> ' + adGroupAd.adId + ', adName-> ' + adGroupAd.adName
      + ', mediaId-> ' + adGroupAd.mediaId);
  }
}
```

### 広告グループ配下の全てのテキスト広告情報を取得する / Get text ad in an ad group
```.js
function getTextAdInAdGroup() {

  const accountId = AdsUtilities.getCurrentAccountId();
  const adGroupIds = [111111111, 222222222, 333333333];//Empty when not specified
     
  const adGroupAds = Display.AdGroupAdService.get({
    accountId: accountId,
    adGroupIds: adGroupIds,
  }).rval;
  
  for (let i = 0; i < Object.keys(adGroupAds.values).length; i++){
    let adGroupAd = adGroupAds.values[i].adGroupAd;
    
    if (adGroupAd.adStyle == 'TEXT') {
      Logger.log('adType-> ' + adGroupAd.ad.adType
        + ', description-> ' + adGroupAd.ad.textAd.description + ', headline-> ' + adGroupAd.ad.textAd.headline
        + ', adGroupId-> ' + adGroupAd.adGroupId + ', adGroupName-> ' + adGroupAd.adGroupName
        + ', adId-> ' + adGroupAd.adId + ', adName-> ' + adGroupAd.adName);
    }
  }
}
```

### 広告グループ配下の全ての画像広告情報を取得する / Get image ad in an ad group
```.js
function getImageAdInAdGroup() {
     
  const accountId = AdsUtilities.getCurrentAccountId();
  const adGroupIds = [111111111, 222222222, 333333333];//Empty when not specified
  
  const adGroupAds = Display.AdGroupAdService.get({
    accountId: accountId,
    adGroupIds: adGroupIds,
  }).rval;
  
  for (let i = 0; i < Object.keys(adGroupAds.values).length; i++){
    let adGroupAd = adGroupAds.values[i].adGroupAd;
    
    if (adGroupAd.adStyle == 'IMAGE') {
      Logger.log('adType-> ' + adGroupAd.ad.adType
        + ', adGroupId-> ' + adGroupAd.adGroupId + ', adGroupName-> ' + adGroupAd.adGroupName
        + ', adId-> ' + adGroupAd.adId + ', adName-> ' + adGroupAd.adName
        + ', mediaId-> ' + adGroupAd.mediaId);
    }
  }
}
```
