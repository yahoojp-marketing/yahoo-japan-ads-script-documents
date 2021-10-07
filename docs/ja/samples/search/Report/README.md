# README.md

### Create an account report
```.js

function createAccountReport(){
 
    const accountId = AdsUtilities.getCurrentAccountId();
 
    const reports = AdsUtilities.getSearchReport({
         
        accountId: accountId,
        fields: ["ACCOUNT_ID","IMPS","CLICKS","COST"],
        reportDateRangeType: "THIS_MONTH",
        reportType: "ACCOUNT",
    });
 
    var report = reports.reports[0].rows;
         
    for (let i = 1; i < report.length; i++){
        Logger.log('ACCOUNT_ID->' + report[i][0]
            + ', IMPS->' + report[i][1]
            + ', CLICKS->' + report[i][2]
            + ', COST->' + report[i][3]);
    }
}
```

### Create a keyword report
```.js
function createKeywordReport(){
 
    const accountId = AdsUtilities.getCurrentAccountId();
 
    const reports = AdsUtilities.getSearchReport({
         
        accountId: accountId,
        fields: ["KEYWORD","IMPS","CLICKS","COST"],
        reportDateRangeType: "THIS_MONTH",
        reportType: "KEYWORDS",
    });

    var report = reports.reports[0].rows;
         
    for (let i = 1; i < report.length; i++){
        Logger.log('KEYWORD->' + report[i][0]
            + ', IMPS->' + report[i][1]
            + ', CLICKS->' + report[i][2]
            + ', COST->' + report[i][3]);
    }  
}
```
