# DriveApp

### Create a new folder
```$xslt
function createNewFolder(){
   
  var name = "newFolderName";
  const newFolder = DriveApp.createFolder(name);
   
  Logger.log('newFolderId -> ' + newFolder.getId());
}
```

### Create a new file in a folder
```$xslt
function createNewFileInFolder(){
 
  const folderId = "1234ABCD";
  const folder = DriveApp.getFolderById(folderId);
   
  var fileName = "newFile";
  const newFile = folder.createFile(fileName, "Hello, world");
}
```

### List of files in a folder
```$xslt
function listOfFilesInFolder(){
 
  const folderId = "1234ABCD";
  const files = DriveApp.getFolderById(folderId).getFiles();
   
  while (files.hasNext()) {
     
    const file = files.next();
    Logger.log("fileId-> " + file.getId() + ", fileName-> " + file.getName());
     
  }
}
```