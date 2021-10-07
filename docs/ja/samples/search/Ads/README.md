# Ads

### Add an expanded text ad
```.js
function addExpandedTextAd(){
     
    const accountId = AdsUtilities.getCurrentAccountId();
 
    const adGroupAdServices = Search.AdGroupAdService.add({
        "accountId": accountId,
        "operand": [
            {
                "ad": {
                    "adType": "EXTENDED_TEXT_AD",
                    "advancedUrl": "http://xxxxxx.co.jp",
                    "description1": "ZZZZZZ",
                    "headline1": "XXXXXX",
                    "extendedTextAd": {
                        "headline2": "YYYYYY",
                    },
                },
                "adGroupId": 111111111,
                "adName": "CCCCCC",
                "campaignId": 222222,
                "userStatus": "ACTIVE",
            }
        ]
    }).rval;
     
    for (let i = 0; i < Object.keys(adGroupAdServices.values).length; i++){
        let adGroupAd = adGroupAdServices.values[i].adGroupAd;
        Logger.log('advancedUrl -> ' + adGroupAd.ad.advancedUrl
            + ', headline1 -> ' + adGroupAd.ad.headline1
            + ', headline2 -> ' + adGroupAd.ad.extendedTextAd.headline2
            + ', description1 -> ' + adGroupAd.ad.description1); 
    }
}
```

### Add a responsive search ad
```.js
function addResponsiveSearchAd(){
     
    const accountId = AdsUtilities.getCurrentAccountId();
 
    const adGroupAdServices = Search.AdGroupAdService.add({
        "accountId": accountId,
        "operand": [
            {
                "ad": {
                    "adType": "RESPONSIVE_SEARCH_AD",
                    "advancedUrl": "http://yahoo.co.jp",
                    "responsiveSearchAd": {
                        "headlines": [//3 or more and less than 15
                            {
                                "text": "HEADLINEAAA",
                            },
                            {
                                "text": "HEADLINEBBB",
                            },
                            {
                                "text": "HEADLINECCC",
                            }
                        ],
                        "descriptions": [//2 or more and less than 4
                            {
                                "text": "DESCRIPTIONAAA",
                            },
                            {
                                "text": "DESCRIPTIONBBB",
                            }
                        ],
                    },
                },
                "adGroupId": 111111111,
                "adName": "ADNAME_AAAAA",
                "campaignId": 222222,
                "userStatus": "ACTIVE",
            }
        ]
    }).rval;
     
    for (let i = 0; i < Object.keys(adGroupAdServices.values).length; i++){
        let adGroupAd = adGroupAdServices.values[i].adGroupAd;
         
        Logger.log('adType -> ' + adGroupAd.ad.adType
            + ', advancedUrl -> ' + adGroupAd.ad.advancedUrl
            + ', adGroupId -> ' + adGroupAd.adGroupId
            + ', adName -> ' + adGroupAd.adName
            + ', campaignId -> ' + adGroupAd.campaignId);
             
        let responsiveSearchAd = adGroupAd.ad.responsiveSearchAd;
         
        for (let j = 0; j < responsiveSearchAd.headlines.length; j++){
            Logger.log('headline' + j + ' -> ' + responsiveSearchAd.headlines[j].text);
        }
 
        for (let j = 0; j < responsiveSearchAd.descriptions.length; j++){
            Logger.log('description' + j + ' -> ' + responsiveSearchAd.descriptions[j].text);
        }
    }
}
```

### Pause ads in an ad group
```.js
function pauseAdsInAdGroup(){
     
    const accountId = AdsUtilities.getCurrentAccountId();
 
    let AdGroupAdsGet = Search.AdGroupAdService.get({
        "accountId": accountId,
        "adGroupIds": [
          325526300,//Multiple selections are possible
        ]
    }).rval;
     
    let AdGroupAdArray = [];
     
    for (let i = 0; i < AdGroupAdsGet.totalNumEntries; i++) {
        let AdGroupAd = AdGroupAdsGet.values[i].adGroupAd;
 
        AdGroupAd.userStatus = "PAUSED";
         
        AdGroupAdArray.push(AdGroupAd);
    }
 
    const AdGroupAdsSet = Search.AdGroupAdService.set({
        "accountId": accountId,
        "operand": AdGroupAdArray,
    }).rval;
 
    for (let i = 0; i < Object.keys(AdGroupAdsSet.values).length; i++) {
        let AdGroupAd = AdGroupAdsSet.values[i].adGroupAd;
         
        Logger.log('adId -> ' + AdGroupAd.adId
          + ', adName -> ' + AdGroupAd.adName
          + ', adGroupId -> ' + AdGroupAd.adGroupId
          + ', adGroupName -> ' + AdGroupAd.adGroupName
          + ', userStatus -> ' + AdGroupAd.userStatus);
    }
}
```

### Get all ads
```.js

function getAllAds(){
     
    const accountId = AdsUtilities.getCurrentAccountId();
 
    const adGroupAdServices = Search.AdGroupAdService.get({
        "accountId": accountId,
    }).rval;
     
    for (let i = 0; i < adGroupAdServices.totalNumEntries; i++){
        let adGroupAd = adGroupAdServices.values[i].adGroupAd;
        Logger.log('adId -> ' + adGroupAd.adId + ', adName -> ' + adGroupAd.adName);
    }
}
```

### Get all ads by id
```.js

function getAllAdsById(){
     
    const accountId = AdsUtilities.getCurrentAccountId();
 
    const adGroupAdServices = Search.AdGroupAdService.get({
        "accountId": accountId,
        "adIds": [
            111111111, 222222222,//Multiple selections are possible
        ],
    }).rval;
     
    for (let i = 0; i < adGroupAdServices.totalNumEntries; i++){
        let adGroupAd = adGroupAdServices.values[i].adGroupAd;
        Logger.log('adId -> ' + adGroupAd.adId + ', adName -> ' + adGroupAd.adName);
    }
}
```

### Get expanded text ads in an ad group
```.js
function getExpandedTextAdsInAdGroup(){
     
    const accountId = AdsUtilities.getCurrentAccountId();
 
    const adGroupAdServices = Search.AdGroupAdService.get({
        "accountId": accountId,
        "adGroupIds": [
          325456241, 325446248,//Multiple selections are possible
        ],
        "adTypes": [
          "EXTENDED_TEXT_AD"
        ],
    }).rval;
     
    for (let i = 0; i < adGroupAdServices.totalNumEntries; i++){
        let adGroupAd = adGroupAdServices.values[i].adGroupAd;
         
        Logger.log('adGroupId -> ' + adGroupAd.adGroupId
            + ', adType -> ' + adGroupAd.ad.adType
            + ', advancedUrl -> ' + adGroupAd.ad.advancedUrl
            + ', description1 -> ' + adGroupAd.ad.description1
            + ', headline1 -> ' + adGroupAd.ad.headline1
            + ', headline2 -> ' + adGroupAd.ad.extendedTextAd.headline2);
    }
}
```

### Get responsive search ad in an ad group
```.js
function getResponsiveSearchAdInAdGroup(){
     
    const accountId = AdsUtilities.getCurrentAccountId();
 
    const adGroupAdServices = Search.AdGroupAdService.get({
      "accountId": accountId,
      "adGroupIds": [
        325536233, 325436233,//Multiple selections are possible
      ],
      "adTypes": [
        "RESPONSIVE_SEARCH_AD",
      ],
    }).rval;
     
    for (let i = 0; i < adGroupAdServices.totalNumEntries; i++){
        let adGroupAd = adGroupAdServices.values[i].adGroupAd;
 
        Logger.log('adType -> ' + adGroupAd.ad.adType
            + ', advancedUrl -> ' + adGroupAd.ad.advancedUrl
            + ', adGroupId -> ' + adGroupAd.adGroupId
            + ', adName -> ' + adGroupAd.adName
            + ', campaignId -> ' + adGroupAd.campaignId);
             
        let responsiveSearchAd = adGroupAd.ad.responsiveSearchAd;
         
        for (let j = 0; j < responsiveSearchAd.headlines.length; j++){
            Logger.log('headline' + j + ' -> ' + responsiveSearchAd.headlines[j].text);
        }
 
        for (let j = 0; j < responsiveSearchAd.descriptions.length; j++){
            Logger.log('description' + j + ' -> ' + responsiveSearchAd.descriptions[j].text);
        }
    }
}
```