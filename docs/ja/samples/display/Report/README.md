# Report

### Create an account report
```$xslt
function createAccountReport(){
  
    const accountId = AdsUtilities.getCurrentAccountId();
  
    const reports = AdsUtilities.getDisplayReport({
        accountId: accountId,
        fields: [
          "ACCOUNT_ID", "ACCOUNT_NAME", "IMPS", "CLICK", "COST"
        ],
        reportDateRangeType: "THIS_MONTH",
    });
 
    for (let i = 0; i < reports.reports.length; i++){
        var report = reports.reports[i].rows;
          
        for (let j = 1; j < report.length; j++){
            Logger.log('ACCOUNT_ID-> ' + report[j][0]
              + ', ACCOUNT_NAME-> ' + report[j][1]
              + ', IMPS-> ' + report[j][2]
              + ', CLICKS-> ' + report[j][3]
              + ', COST-> ' + report[j][4]);
        }
    }
}
```

### Create an ad report
```$xslt
function createAdReport(){
  
    const accountId = AdsUtilities.getCurrentAccountId();
  
    const reports = AdsUtilities.getDisplayReport({
        accountId: accountId,
        fields: [
          "AD_ID", "AD_NAME", "IMPS", "CLICK", "COST"
        ],
        reportDateRangeType: "THIS_MONTH",
    });
 
    for (let i = 0; i < reports.reports.length; i++){
        var report = reports.reports[i].rows;
          
        for (let j = 1; j < report.length; j++){
            Logger.log('AD_ID-> ' + report[j][0]
              + ', AD_NAME-> ' + report[j][1]
              + ', IMPS-> ' + report[j][2]
              + ', CLICKS-> ' + report[j][3]
              + ', COST-> ' + report[j][4]);
        }
    }
}
```