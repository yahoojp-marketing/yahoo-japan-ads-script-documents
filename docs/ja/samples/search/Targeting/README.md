# Targeting

### Set location and bid modifiers
```$xslt
function setLocationAndBidModifiers(){
     
    let targetId;
     
    const dictionaries = Search.DictionaryService.getGeographicLocation({
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
     
    const campaignTargets = Search.CampaignTargetService.add({
        "accountId": accountId,
        "operand": [//Multiple selections are possible
            {
                "accountId": accountId,
                "bidMultiplier": 1.50,//default:1.00
                "campaignId": 927192,
                "target": {
                    "locationTarget": {
                        "excludedType": "INCLUDED",
                    },
                    "targetId": targetId,
                    "targetType": "LOCATION"
                }
            },
            {
                "accountId": accountId,
                "bidMultiplier": 1.20,
                "campaignId": 927191,
                "target": {
                    "locationTarget": {
                        "excludedType": "INCLUDED",
                    },
                    "targetId": targetId,
                    "targetType": "LOCATION"
                }
            }
        ]
    }).rval;
     
    for (let i = 0; i < Object.keys(campaignTargets.values).length; i++){
        let campaignTarget = campaignTargets.values[i].campaignTarget;
         
        Logger.log('campaignId -> ' + campaignTarget.campaignId
            + ', targetId -> ' + campaignTarget.target.targetId
            + ', excludedType -> ' + campaignTarget.target.locationTarget.excludedType
            + ', targetType -> ' + campaignTarget.target.targetType
            + ', bidMultiplier -> ' + campaignTarget.bidMultiplier);
    }
}
```

### Set device and bid modifiers
```$xslt
Set device and bid modifiers

``` 

### Set schedule and bid modifiers
```$xslt
function setScheduleAndBidModifiers(){
     
    const accountId = AdsUtilities.getCurrentAccountId();
     
    const campaignTargets = Search.CampaignTargetService.add({
        "accountId": accountId,
        "operand": [//Multiple selections are possible
            {
                "accountId": accountId,
                "bidMultiplier": 1.50,//default:1.00
                "campaignId": 927192,
                "target": {
                    "scheduleTarget": {
                        "dayOfWeek": "MONDAY",
                        "endHour": 21,
                        "endMinute": "FIFTEEN",
                        "startHour": 8,
                        "startMinute": "FORTY_FIVE"
                    },
                    "targetType": "SCHEDULE"
                }
            },
            {
                "accountId": accountId,
                "bidMultiplier": 1.20,
                "campaignId": 927191,
                "target": {
                    "scheduleTarget": {
                        "dayOfWeek": "FRIDAY",
                        "endHour": 22,
                        "endMinute": "ZERO",
                        "startHour": 7,
                        "startMinute": "THIRTY"
                    },
                    "targetType": "SCHEDULE"
                }
            }
        ]
    }).rval;
     
    for (let i = 0; i < Object.keys(campaignTargets.values).length; i++){
        let campaignTarget = campaignTargets.values[i].campaignTarget;
         
        Logger.log('campaignId -> ' + campaignTarget.campaignId
            + ', targetId -> ' + campaignTarget.target.targetId
            + ', targetType -> ' + campaignTarget.target.targetType
            + ', dayOfWeek -> ' + campaignTarget.target.scheduleTarget.dayOfWeek
            + ', bidMultiplier -> ' + campaignTarget.bidMultiplier);
    }
}
```