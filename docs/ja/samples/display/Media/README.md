# Media

### Get all images
```$xslt
function getAllImages(){
 
    const accountId = AdsUtilities.getCurrentAccountId();
 
    const medias = Display.MediaService.get({
        "accountId": accountId,
    }).rval;
 
    for (let i = 0; i < medias.totalNumEntries; i++){
        let mediaRecord = medias.values[i].mediaRecord;
         
        Logger.log('campaignBannerFlg -> ' + mediaRecord.campaignBannerFlg
            + ', logoFlg -> ' + mediaRecord.logoFlg
            + ', mediaType -> ' + mediaRecord.imageMedia.mediaType
            + ', mediaFileType -> ' + mediaRecord.imageMedia.mediaFileType
            + ', mediaId -> ' + mediaRecord.mediaId
            + ', mediaName -> ' + mediaRecord.mediaName
            + ', mediaTitle -> ' + mediaRecord.mediaTitle);
    }
}
```

### Add a image from Google Drive
```$xslt
function addImageFromGoogleDrive(){
  const accountId = AdsUtilities.getCurrentAccountId();
  
  const fileId = "1234ABCD";
  const fileBytes = DriveApp.getFileById(fileId).getBlob().getBytes();

  var encoded = Utilities.base64Encode(fileBytes);

  const medias = Display.MediaService.add({
    "accountId": accountId,
    "operand": [
      {
        "accountId": accountId,
        "imageMedia": {
            "data": encoded,
        },
        "mediaName": "AAAAA.jpg",
        "mediaTitle": "BBBBB",
        "userStatus": "ACTIVE",
      }
    ]
  }).rval;

  for (let i = 0; i < Object.keys(medias).length; i++){
    let mediaRecord = medias.values[i].mediaRecord;
    
    Logger.log('mediaId -> ' + mediaRecord.mediaId
      + ', mediaName -> ' + mediaRecord.mediaName
      + ', mediaTitle -> ' + mediaRecord.mediaTitle);
  }
}
```

### Pause a image
```$xslt
function pauseImage(){
     
    const accountId = AdsUtilities.getCurrentAccountId();
 
    const mediasGet = Display.MediaService.get({
        "accountId": accountId,
    }).rval;
     
    let mediaArray = [];
 
    for (let i = 0; i < mediasGet.totalNumEntries; i++){
        let mediaRecord = mediasGet.values[i].mediaRecord;
         
        mediaRecord.userStatus = "PAUSED";
         
        mediaArray.push(mediaRecord);
    }
     
    const mediasSet = Display.MediaService.set({
        "accountId": accountId,
        "operand": mediaArray,
    }).rval;
     
    for (let i = 0; i < Object.keys(mediasSet.values).length; i++){
        let mediaRecord = mediasSet.values[i].mediaRecord;
         
        Logger.log('mediaId -> ' + mediaRecord.mediaId
            + ', mediaName -> ' + mediaRecord.mediaName
            + ', mediaTitle -> ' + mediaRecord.mediaTitle
            + ', mediaTitle -> ' + mediaRecord.userStatus);
    }
}
```
