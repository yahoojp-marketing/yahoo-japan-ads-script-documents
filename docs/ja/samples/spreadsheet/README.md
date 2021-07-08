# Spreadsheet

### Append rows to a spreadsheet
```$xslt
function appendRowsToSpreadsheet(){
 
  const spreadsheetId = 'スプレッドシートID';
  var ss = SpreadsheetApp.openById(spreadsheetId);
  var sheetName = 'test';
   
  let sh = ss.getSheetByName(sheetName);
   
  sh.appendRow(['Armadillo', 'Bear', 'Cat']);
}
```

### Set a range's values
```$xslt
function setRangeValues(){
 
    const spreadsheetId = 'スプレッドシートID';
    var ss = SpreadsheetApp.openById(spreadsheetId);
    var sheetName = 'test1';
 
    let sh = ss.getSheetByName(sheetName);
 
    var dataArray = [
        ['America','Brazil','Canada','Denmark'],
        ['Apple','Banana','Cherry','Daikon'],
    ];
 
    sh.getRange('A1').setValues(dataArray);
}
```

### Log the data of a spreadsheet
```$xslt
function logDataOfSpreadsheet(){
 
    const spreadsheetId = '1qa6_LqQZaK4JK9zaonu6uIarlDryzIG_r2lrJNH-xIs';
    var ss = SpreadsheetApp.openById(spreadsheetId);
    
    var sheetName = "test1";
    let sh = ss.getSheetByName(sheetName);
     
    let dataArray = sh.getDataRange().getValues();
 
    for (let i = 0; i < dataArray.length; i++){
        Logger.log(dataArray[i].join(', '));   
    }
}
```

### Clear a sheets values
```$xslt
function clearSheetsValues(){
     
    const spreadsheetId = 'スプレッドシートID';
    var ss = SpreadsheetApp.openById(spreadsheetId);
    var sheetName = 'test1';
     
    let sh = ss.getSheetByName(sheetName);
     
    sh.getRange('A1:C2').clear();
}
```

### Report data to a spreadsheet
```$xslt
function reportDataToSpreadsheet(){
 
    const spreadsheetId = 'スプレッドシートID';
    var ss = SpreadsheetApp.openById(spreadsheetId);
    var sheetName = 'test1';
     
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
