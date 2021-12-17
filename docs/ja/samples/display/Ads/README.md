# 広告 / Ads

### テキスト広告を新規追加する / Add a text ad
```.js
function addTextAd(){

  const accountId = AdsUtilities.getCurrentAccountId();

  const adGroupAds = Display.AdGroupAdService.add({
    accountId: accountId,
    operand: [
      {
        accountId: accountId,
        ad: {
          adType: 'TEXT_LONG_AD1',
          textAd: {
            description: 'DESCRIPTIONAAA',
            headline: 'HEADLINEAAA',
            displayUrlLevel: 'DOMAIN',
            finalUrl: 'http://yahoo.co.jp'
          }
        },
        adGroupId: 111111,
        adName: 'ADNAME_AAA',
        campaignId: 222222,
        userStatus: 'ACTIVE',
      }
    ]
  }).rval;
     
  for (let i = 0; i < Object.keys(adGroupAds.values).length; i++){
    let adGroupAd = adGroupAds.values[i].adGroupAd;
         
    Logger.log('adType-> ' + adGroupAd.ad.adType
      + ', description-> ' + adGroupAd.ad.textAd.description
      + ', headline-> ' + adGroupAd.ad.textAd.headline
      + ', finalUrl-> ' + adGroupAd.ad.textAd.finalUrl
      + ', adId-> ' + adGroupAd.adId
      + ', adName-> ' + adGroupAd.adName
      + ', adGroupId-> ' + adGroupAd.adGroupId
      + ', campaignId-> ' + adGroupAd.campaignId);
  } 
}
```

### 画像広告を新規追加する / Add an image ad
```.js
function addImageAd(){
     
  const accountId = AdsUtilities.getCurrentAccountId();
     
  const adGroupAds = Display.AdGroupAdService.add({
    accountId: accountId,
    operand: [
      {
        accountId: accountId,
        ad: {
          adType: 'BANNER_IMAGE_AD',
          bannerImageAd: {
            displayUrlLevel: 'DOMAIN',
            finalUrl: 'http://yahoo.co.jp'
          },
        },
        adGroupId: 111111,
        adName: 'CCC',
        adStyle: 'IMAGE',
        campaignId: 222222,
        mediaId: 333333,
        userStatus: 'ACTIVE',
      }
    ]
  }).rval;
     
  for (let i = 0; i < Object.keys(adGroupAds.values).length; i++){
    let adGroupAd = adGroupAds.values[i].adGroupAd;
         
    Logger.log('adType-> ' + adGroupAd.ad.adType
      + ', finalUrl-> ' + adGroupAd.ad.bannerImageAd.finalUrl
      + ', adGroupId-> ' + adGroupAd.adGroupId
      + ', adName-> ' + adGroupAd.adName
      + ', adId-> ' + adGroupAd.adId
      + ', adStyle-> ' + adGroupAd.adStyle
      + ', campaignId-> ' + adGroupAd.campaignId);
  } 
}
```

### 広告グループ配下の広告を配信停止にする / Pause ads in an ad group
```.js
function pauseAdsInAdGroup(){
     
  const accountId = AdsUtilities.getCurrentAccountId();
     
  const adGroupAdsGet = Display.AdGroupAdService.get({
    accountId: accountId,
    adGroupIds: [
      111111,//Multiple selections are possible
    ]
  }).rval;
  
  let adGroupAdArray = [];
  
  for (let i = 0; i < adGroupAdsGet.totalNumEntries; i++){
    let adGroupAd = adGroupAdsGet.values[i].adGroupAd;
    adGroupAd.userStatus = 'PAUSED';
    adGroupAdArray.push(adGroupAd);
  }
     
  const adGroupAdsSet = Display.AdGroupAdService.set({
    accountId: accountId,
    operand: adGroupAdArray,
  }).rval;
     
  for (let i = 0; i < Object.keys(adGroupAdsSet.values).length; i++){
    let adGroupAd = adGroupAdsSet.values[i].adGroupAd;
         
    Logger.log('adGroupId-> ' + adGroupAd.adGroupId
      + ', adName-> ' + adGroupAd.adName
      + ', adId-> ' + adGroupAd.adId
      + ', campaignId-> ' + adGroupAd.campaignId
      + ', userStatus-> ' + adGroupAd.userStatus);
  }
}
```

### 全ての広告情報を取得する / Get all ads
```.js
function getAllAds(){
 
  const accountId = AdsUtilities.getCurrentAccountId();
  
  const adGroupAds = Display.AdGroupAdService.get({
    accountId: accountId,
  }).rval;
 
  for (let i = 0; i < adGroupAds.totalNumEntries; i++){
    let adGroupAd = adGroupAds.values[i].adGroupAd;
         
    Logger.log('adType-> ' + adGroupAd.ad.adType
      + ', adGroupId-> ' + adGroupAd.adGroupId
      + ', adGroupName-> ' + adGroupAd.adGroupName
      + ', adId-> ' + adGroupAd.adId
      + ', adName-> ' + adGroupAd.adName
      + ', adStyle-> ' + adGroupAd.adStyle
      + ', campaignId-> ' + adGroupAd.campaignId
      + ', campaignName-> ' + adGroupAd.campaignName
      + ', mediaId-> ' + adGroupAd.mediaId);
  }
}
```

### 指定の広告情報を取得する / Get all ads by id
```.js
function getAllAdsById(){
    
  const accountId = AdsUtilities.getCurrentAccountId();
     
  const adGroupAds = Display.AdGroupAdService.get({
    accountId: accountId,
    adIds: [
      111111, 222222,//Multiple selections are possible
    ],
  }).rval;
 
  for (let i = 0; i < adGroupAds.totalNumEntries; i++){
    let adGroupAd = adGroupAds.values[i].adGroupAd;
         
    Logger.log('adType-> ' + adGroupAd.ad.adType
      + ', adGroupId-> ' + adGroupAd.adGroupId
      + ', adGroupName-> ' + adGroupAd.adGroupName
      + ', adId-> ' + adGroupAd.adId
      + ', adName-> ' + adGroupAd.adName
      + ', adStyle-> ' + adGroupAd.adStyle
      + ', campaignId-> ' + adGroupAd.campaignId
      + ', campaignName-> ' + adGroupAd.campaignName
      + ', mediaId-> ' + adGroupAd.mediaId);
  }
}
```

### 広告グループ配下の全てのテキスト広告情報を取得する / Get text ad in an ad group
```.js
function getTextAdInAdGroup(){

  const accountId = AdsUtilities.getCurrentAccountId();
     
  const adGroupAds = Display.AdGroupAdService.get({
    accountId: accountId,
    adGroupIds: [
      111111, 222222,//Multiple selections are possible
    ]
  }).rval;
  
  for (let i = 0; i < adGroupAds.totalNumEntries; i++){
    let adGroupAd = adGroupAds.values[i].adGroupAd;
    
    if (adGroupAd.ad.adType == 'TEXT_LONG_AD1' || adGroupAd.ad.adType == 'TEXT_LONG_AD2'){
      
      Logger.log('adType-> ' + adGroupAd.ad.adType
        + ', description-> ' + adGroupAd.ad.textAd.description
        + ', headline-> ' + adGroupAd.ad.textAd.headline
        + ', finalUrl-> ' + adGroupAd.ad.textAd.finalUrl
        + ', adGroupId-> ' + adGroupAd.adGroupId
        + ', adGroupName-> ' + adGroupAd.adGroupName
        + ', adId-> ' + adGroupAd.adId
        + ', adName-> ' + adGroupAd.adName
        + ', adStyle-> ' + adGroupAd.adStyle
        + ', campaignId-> ' + adGroupAd.campaignId
        + ', campaignName-> ' + adGroupAd.campaignName
        + ', mediaId-> ' + adGroupAd.mediaId);
    }
  }
}
```

### 広告グループ配下の全ての画像広告情報を取得する / Get image ad in an ad group
```.js
function getImageAdInAdGroup(){
     
  const accountId = AdsUtilities.getCurrentAccountId();
  
  const adGroupAds = Display.AdGroupAdService.get({
    accountId: accountId,
    adGroupIds: [
      111111,//Multiple selections are possible
    ]
  }).rval;
  
  for (let i = 0; i < adGroupAds.totalNumEntries; i++){
    let adGroupAd = adGroupAds.values[i].adGroupAd;
    
    if (adGroupAd.ad.adType == 'BANNER_IMAGE_AD') {
      Logger.log('adType-> ' + adGroupAd.ad.adType
        + ', displayUrl-> ' + adGroupAd.ad.bannerImageAd.displayUrl
        + ', finalUrl-> ' + adGroupAd.ad.bannerImageAd.finalUrl
        + ', adGroupId-> ' + adGroupAd.adGroupId
        + ', adGroupName-> ' + adGroupAd.adGroupName
        + ', adId-> ' + adGroupAd.adId
        + ', adName-> ' + adGroupAd.adName
        + ', adStyle-> ' + adGroupAd.adStyle
        + ', campaignId-> ' + adGroupAd.campaignId
        + ', campaignName-> ' + adGroupAd.campaignName
        + ', mediaId-> ' + adGroupAd.mediaId);
    }
  }
}
```
