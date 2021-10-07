# Ads

### Add an text ad
```.js
function addTextAd(){
     
    const accountId = AdsUtilities.getCurrentAccountId();
     
    const AdGroupAds = Display.AdGroupAdService.add({
        "accountId": accountId,
        "operand": [
            {
                "accountId": accountId,
                "ad": {
                    "adType": "TEXT_LONG_AD1",
                    "textAd": {
                        "description": "DESCRIPTIONAAA",
                        "displayUrl": "yahoo.co.jp",
                        "headline": "HEADLINEAAA",
                        "url": "http://yahoo.co.jp"
                    }
                },
                "adGroupId": 209780518,
                "adName": "ADNAME_AAA",
                "campaignId": 27462571,
                "userStatus": "ACTIVE",
            }
        ]
    }).rval;
     
    for (let i = 0; i < Object.keys(AdGroupAds).length; i++){
        let adGroupAd = AdGroupAds.values[i].adGroupAd;
         
        Logger.log('adType-> ' + adGroupAd.ad.adType
            + ', description-> ' + adGroupAd.ad.textAd.description
            + ', headline-> ' + adGroupAd.ad.textAd.headline
            + ', url-> ' + adGroupAd.ad.textAd.url
            + ', adId-> ' + adGroupAd.adId
            + ', adName-> ' + adGroupAd.adName
            + ', adGroupId-> ' + adGroupAd.adGroupId
            + ', campaignId-> ' + adGroupAd.campaignId);
    } 
}
```

### Add a image ad
```.js
function addImageAd(){
     
    const accountId = AdsUtilities.getCurrentAccountId();
     
    const AdGroupAds = Display.AdGroupAdService.add({
        "accountId": accountId,
        "operand": [
            {
                "accountId": accountId,
                "ad": {
                    "adType": "BANNER_IMAGE_AD",
                    "bannerImageAd": {
                        "displayUrl": "yahoo.co.jp",
                        "url": "http://yahoo.co.jp"
                    },
                },
                "adGroupId": 209780573,
                "adName": "CCC",
                "adStyle": "IMAGE",
                "campaignId": 27462586,
                "mediaId": 1090046405,
                "userStatus": "ACTIVE",
            }
        ]
    }).rval;
     
    for (let i = 0; i < Object.keys(AdGroupAds.values).length; i++){
        let adGroupAd = AdGroupAds.values[i].adGroupAd;
         
        Logger.log('adType-> ' + adGroupAd.ad.adType
            + ', url-> ' + adGroupAd.ad.bannerImageAd.url
            + ', adGroupId-> ' + adGroupAd.adGroupId
            + ', adName-> ' + adGroupAd.adName
            + ', adId-> ' + adGroupAd.adId
            + ', adStyle-> ' + adGroupAd.adStyle
            + ', campaignId-> ' + adGroupAd.campaignId);
    } 
}
```

### Pause ads in an ad group
```.js
function pauseAdsInAdGroup(){
     
    const accountId = AdsUtilities.getCurrentAccountId();
     
    const adGroupAdsGet = Display.AdGroupAdService.get({
        "accountId": accountId,
        "adGroupIds": [
          209780518,//Multiple selections are possible
        ]
    }).rval;
 
    let adGroupAdArray = [];
     
    for (let i = 0; i < adGroupAdsGet.totalNumEntries; i++){
        let adGroupAd = adGroupAdsGet.values[i].adGroupAd;
         
        adGroupAd.userStatus = "PAUSED";
         
        adGroupAdArray.push(adGroupAd);
    }
     
    const adGroupAdsSet = Display.AdGroupAdService.set({
        "accountId": accountId,
        "operand": adGroupAdArray,
    }).rval;
     
    for (let i = 0; i < Object.keys(adGroupAdsSet).length; i++){
        let adGroupAd = adGroupAdsSet.values[i].adGroupAd;
         
        Logger.log('adGroupId-> ' + adGroupAd.adGroupId
            + ', adName-> ' + adGroupAd.adName
            + ', adId-> ' + adGroupAd.adId
            + ', campaignId-> ' + adGroupAd.campaignId
            + ', userStatus-> ' + adGroupAd.userStatus);
    }
}
```

### Get all ads
```.js
function getAllAds(){
 
    const accountId = AdsUtilities.getCurrentAccountId();
     
    const adGroupAds = Display.AdGroupAdService.get({
        "accountId": accountId,
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

### Get all ads by id
```.js
function getAllAdsById(){
 
    const accountId = AdsUtilities.getCurrentAccountId();
     
    const adGroupAds = Display.AdGroupAdService.get({
        "accountId": accountId,
        "adIds": [
            360710405, 360660477,//Multiple selections are possible
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

### Get text ad in an ad group
```.js
function getTextAdInAdGroup(){
 
    const accountId = AdsUtilities.getCurrentAccountId();
     
    const adGroupAds = Display.AdGroupAdService.get({
        "accountId": accountId,
        "adGroupIds": [
            209780575, 209780518,//Multiple selections are possible
        ]
    }).rval;
 
    for (let i = 0; i < adGroupAds.totalNumEntries; i++){
        let adGroupAd = adGroupAds.values[i].adGroupAd;
 
        if (adGroupAd.ad.adType == "TEXT_LONG_AD1" || adGroupAd.ad.adType == "TEXT_LONG_AD2"){
            Logger.log('adType-> ' + adGroupAd.ad.adType
                + ', description-> ' + adGroupAd.ad.textAd.description
                + ', headline-> ' + adGroupAd.ad.textAd.headline
                + ', url-> ' + adGroupAd.ad.textAd.url
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

### Get image ad in an ad group
```.js
function getImageAdInAdGroup(){
     
    const accountId = AdsUtilities.getCurrentAccountId();
 
    const adGroupAds = Display.AdGroupAdService.get({
        "accountId": accountId,
        "adGroupIds": [
            209780573,//Multiple selections are possible
        ]
    }).rval;
 
    for (let i = 0; i < adGroupAds.totalNumEntries; i++){
        let adGroupAd = adGroupAds.values[i].adGroupAd;
         
        if (adGroupAd.ad.adType == "BANNER_IMAGE_AD") {
            Logger.log('adType-> ' + adGroupAd.ad.adType
                + ', displayUrl-> ' + adGroupAd.ad.bannerImageAd.displayUrl
                + ', url-> ' + adGroupAd.ad.bannerImageAd.url
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
