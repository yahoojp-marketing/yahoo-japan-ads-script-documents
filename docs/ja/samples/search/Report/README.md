# README.md

### Create an account report
```$xslt

function createAccountReport(){
 
    const accountId = AdsUtilities.getCurrentAccountId();
 
    const reports = AdsUtilities.getSearchReport({
         
        accountId: accountId,
        fields: ["ACCOUNT_ID","IMPS","CLICKS","COST"],
        reportDateRangeType: "THIS_MONTH",
        reportType: "ACCOUNT",
    });
 
    for (let i = 0; i < Object.keys(reports.reports).length; i++){
        var report = reports.reports[i].rows;
         
        for (let j = 1; j < report.length; j++){
            Logger.log('ACCOUNT_ID->' + report[j][0]
                + ', IMPS->' + report[j][1]
                + ', CLICKS->' + report[j][2]
                + ', COST->' + report[j][3]);
        }
    }
}
```

### Create a keyword report
```$xslt
function createKeywordReport(){
 
    const accountId = AdsUtilities.getCurrentAccountId();
 
    const reports = AdsUtilities.getSearchReport({
         
        accountId: accountId,
        fields: ["KEYWORD","IMPS","CLICKS","COST"],
        reportDateRangeType: "THIS_MONTH",
        reportType: "KEYWORDS",
    });
 
    for (let i = 0; i < Object.keys(reports.reports).length; i++){
        var report = reports.reports[i].rows;
         
        for (let j = 1; j < report.length; j++){
            Logger.log('KEYWORD->' + report[j][0]
                + ', IMPS->' + report[j][1]
                + ', CLICKS->' + report[j][2]
                + ', COST->' + report[j][3]);
        }
    }
}
```