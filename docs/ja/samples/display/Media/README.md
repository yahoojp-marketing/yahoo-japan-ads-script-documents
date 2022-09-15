# メディア情報 / Media

### メディア情報を取得する / Get all images
```.js
function getAllImages() {
  
  const accountId = AdsUtilities.getCurrentAccountId();
  
  const medias = Display.MediaService.get({
    accountId: accountId,
  }).rval;
  
  if (medias.totalNumEntries == 0) {
    Logger.log('Media does not exist.');
    return;
  }
  
  for (let i = 0; i < Object.keys(medias.values).length; i++){
    let mediaRecord = medias.values[i].mediaRecord;
    Logger.log('mediaType-> ' + mediaRecord.imageMedia.mediaType
      + ', mediaFileType-> ' + mediaRecord.imageMedia.mediaFileType
      + ', mediaId-> ' + mediaRecord.mediaId
      + ', mediaName-> ' + mediaRecord.mediaName
      + ', mediaTitle-> ' + mediaRecord.mediaTitle);
  }
}
```

### Googleドライブからメディア情報を追加する / Add an image from Google Drive
```.js
function addImageFromGoogleDrive() {
  
  const accountId = AdsUtilities.getCurrentAccountId();
  
  const fileId = 'fileIdAAA';
  const fileBytes = DriveApp.getFileById(fileId).getBlob().getBytes();
  const encoded = Utilities.base64Encode(fileBytes);

  const mediaArray = [
    {
      accountId: accountId,
      imageMedia: {
        data: encoded,
      },
      mediaName: 'mediaNameAAA.png',
      mediaTitle: 'mediaTitleAAA',
      userStatus: 'ACTIVE',
    }
  ];//Only 1 object can be set
  
  const medias = Display.MediaService.add({
    accountId: accountId,
    operand: mediaArray,
  }).rval;
  
  if (medias.values[0].operationSucceeded) {
    let mediaRecord = medias.values[0].mediaRecord;
    Logger.log('mediaId -> ' + mediaRecord.mediaId
      + ', mediaName -> ' + mediaRecord.mediaName
      + ', mediaTitle -> ' + mediaRecord.mediaTitle + ' have been added.');
    
  } else {
    Logger.log('mediaName-> ' + mediaArray[0].mediaName
      + ', mediaTitle-> ' + mediaArray[0].mediaTitle + ' could not to be added.');
      
  }
}
```

### メディア情報を配信停止にする / Pause an image
```.js
function pauseImage() {
  
  const accountId = AdsUtilities.getCurrentAccountId();
  const mediaIds = [10331155, 10266867, 10266864];//Empty when not specified
  
  const mediasGet = Display.MediaService.get({
    accountId: accountId,
    mediaIds: mediaIds,
    userStatuses: ['ACTIVE'],
  }).rval;
  
  if (mediasGet.totalNumEntries == 0) {
    Logger.log('Media does not exist.');
    return;
  }
  
  let mediaArray = [];
  for (let i = 0; i < Object.keys(mediasGet.values).length; i++){
    let mediaRecord = mediasGet.values[i].mediaRecord;
    mediaRecord.userStatus = 'PAUSED';
    mediaArray.push(mediaRecord);
  }
  
  const mediasSet = Display.MediaService.set({
    accountId: accountId,
    operand: mediaArray,
  }).rval;
  
  for (let i = 0; i < Object.keys(mediasSet.values).length; i++){
    if (mediasSet.values[i].operationSucceeded) {
      let mediaRecord = mediasSet.values[i].mediaRecord;
      Logger.log('mediaId-> ' + mediaRecord.mediaId
        + ', mediaName-> ' + mediaRecord.mediaName
        + ', mediaTitle-> ' + mediaRecord.mediaTitle + ' stopped.');
      
    } else {
      let mediaRecord = mediasGet.values[i].mediaRecord;
      Logger.log('mediaId-> ' + mediaRecord.mediaId
        + ', mediaName-> ' + mediaRecord.mediaName
        + ', mediaTitle-> ' + mediaRecord.mediaTitle + ' could not stopped.');
        
    }
  }
}
```
