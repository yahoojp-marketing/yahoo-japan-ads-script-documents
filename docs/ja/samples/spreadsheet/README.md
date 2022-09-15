# Googleスプレッドシート / Spreadsheet

### スプレッドシートに行を追加する / Append rows to a spreadsheet
```.js
function appendRowsToSpreadsheet(){
 
  const spreadsheetId = 'スプレッドシートID';
  const ss = SpreadsheetApp.openById(spreadsheetId);
  const sheetName = 'test';
   
  let sh = ss.getSheetByName(sheetName);
   
  sh.appendRow(['Armadillo', 'Bear', 'Cat']);
}
```

### 範囲の値を設定する / Set a range's values
```.js
function setRangeValues(){
 
  const spreadsheetId = 'スプレッドシートID';
  const ss = SpreadsheetApp.openById(spreadsheetId);
  const sheetName = 'test1';
 
  let sh = ss.getSheetByName(sheetName);
 
  const dataArray = [
    ['America','Brazil','Canada','Denmark'],
    ['Apple','Banana','Cherry','Daikon'],
  ];
 
  sh.getRange('A1').setValues(dataArray);
}
```

### スプレッドシートのデータをログ出力する / Log the data of a spreadsheet
```.js
function logDataOfSpreadsheet(){
 
  const spreadsheetId = 'スプレッドシートID';
  const ss = SpreadsheetApp.openById(spreadsheetId);
  
  const sheetName = 'test1';
  let sh = ss.getSheetByName(sheetName);
   
  let dataArray = sh.getDataRange().getValues();
 
  for (let i = 0; i < dataArray.length; i++){
    Logger.log(dataArray[i].join(', '));   
  }
}
```

### シートの値をクリアにする / Clear a sheets values
```.js
function clearSheetsValues(){
   
  const spreadsheetId = 'スプレッドシートID';
  const ss = SpreadsheetApp.openById(spreadsheetId);
  const sheetName = 'test1';
   
  let sh = ss.getSheetByName(sheetName);
   
  sh.getRange('A1:C2').clear();
}
```

### スプレッドシートにレポート情報を出力する / Report data to a spreadsheet
```.js
function reportDataToSpreadsheet(){
 
  const spreadsheetId = 'スプレッドシートID';
  const ss = SpreadsheetApp.openById(spreadsheetId);
  const sheetName = 'test1';
   
  let sh = ss.getSheetByName(sheetName);
   
  const reports = AdsUtilities.getSearchReport({
    accountId: AdsUtilities.getCurrentAccountId(),
    fields: [
      'ACCOUNT_ID','IMPS','CLICKS','COST'
    ],
    reportDateRangeType: 'THIS_MONTH',
    reportType: 'ACCOUNT',
  });
   
  sh.getRange('A1').setValues(reports.reports[0].rows);
}
```
