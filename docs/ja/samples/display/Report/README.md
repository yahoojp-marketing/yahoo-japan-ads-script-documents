# レポート / Report

### アカウントレポートを作成する / Create an account report
```.js
function createAccountReport(){

  const accountId = AdsUtilities.getCurrentAccountId();
  
  const reports = AdsUtilities.getDisplayReport({
    accountId: accountId,
    fields: [
      'ACCOUNT_ID', 'ACCOUNT_NAME', 'IMPS', 'CLICK', 'COST'
    ],
    reportDateRangeType: 'THIS_MONTH',
  });
  
  const report = reports.reports[0].rows;
  
  for (let i = 0; i < report.length; i++){
    Logger.log('ACCOUNT_ID-> ' + report[i][0]
      + ', ACCOUNT_NAME-> ' + report[i][1]
      + ', IMPS-> ' + report[i][2]
      + ', CLICKS-> ' + report[i][3]
      + ', COST-> ' + report[i][4]);
  }

}
```

### 広告レポートを作成する / Create an ad report
```.js
function createAdReport(){
  
  const accountId = AdsUtilities.getCurrentAccountId();
  
  const reports = AdsUtilities.getDisplayReport({
    accountId: accountId,
    fields: [
      'AD_ID', 'AD_NAME', 'IMPS', 'CLICK', 'COST'
    ],
    reportDateRangeType: 'THIS_MONTH',
  });
  
  const report = reports.reports[0].rows;
  
  for (let i = 0; i < report.length; i++){
    Logger.log('AD_ID-> ' + report[i][0]
      + ', AD_NAME-> ' + report[i][1]
      + ', IMPS-> ' + report[i][2]
      + ', CLICKS-> ' + report[i][3]
      + ', COST-> ' + report[i][4]);
  }
}
```
