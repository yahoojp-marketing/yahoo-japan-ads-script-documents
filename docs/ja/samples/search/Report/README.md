# レポート / report

### アカウントレポートを作成する / Create an account report
```.js
function createAccountReport(){
  
  const accountId = AdsUtilities.getCurrentAccountId();
  const startDate = yyyyMMdd;//Write the date in yyyyMMdd format
  const endDate = yyyyMMdd;
  
  const report = AdsUtilities.getSearchReport({
    accountId: accountId,
    dateRange: {
      endDate: endDate,
      startDate: startDate,
    },
    fields: ['ACCOUNT_ID', 'IMPS', 'CLICKS', 'COST'],
    reportDateRangeType: 'CUSTOM_DATE',
    reportType: 'ACCOUNT',
  }).reports[0].rows;
  
  for (let i = 0; i < report.length; i++){
    Logger.log('ACCOUNT_ID-> ' + report[i][0] + ', IMPS-> ' + report[i][1]
      + ', CLICKS-> ' + report[i][2] + ', COST-> ' + report[i][3]);
  }
}
```

### キーワードレポートを作成する / Create a keyword report
```.js
function createKeywordReport(){
 
  const accountId = AdsUtilities.getCurrentAccountId();

  const report = AdsUtilities.getSearchReport({
    accountId: accountId,
    fields: ['KEYWORD', 'IMPS', 'CLICKS', 'COST'],
    reportDateRangeType: 'THIS_MONTH',
    reportType: 'KEYWORDS',
  }).reports[0].rows;

  for (let i = 0; i < report.length; i++){
    Logger.log('KEYWORD-> ' + report[i][0] + ', IMPS-> ' + report[i][1]
      + ', CLICKS-> ' + report[i][2] + ', COST-> ' + report[i][3]);
  }  
}
```
