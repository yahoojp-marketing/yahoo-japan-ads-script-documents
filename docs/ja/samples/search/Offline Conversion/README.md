# オフラインコンバージョン / Offline Conversion


## Googleドライブからオフラインコンバージョン情報をアップロード処理 / Upload processing of offline conversion data from Google Drive
```.js
function uploadProcessingOfOfflineConversionData(){

  const accountId = AdsUtilities.getCurrentAccountId();
  
  const fileId = '11111AAAAAbbbbb_-222222BBBBBccccc';
  const fileData = DriveApp.getFileById(fileId).getBlob().getBytes();
  
  const offlineConversions = Search.OfflineConversionService.upload(
    accountId,
    'NEW',
    'sampleData.csv',
    fileData
  ).rval;
}
```
