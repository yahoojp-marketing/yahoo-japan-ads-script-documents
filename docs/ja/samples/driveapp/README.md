# Googleドライブ / DriveApp

### 新しいフォルダーを作成する / Create a new folder
```.js
function createNewFolder(){
   
  const name = 'newFolderName';
  const newFolder = DriveApp.createFolder(name);
   
  Logger.log('newFolderId -> ' + newFolder.getId());
}
```

### フォルダー内に新しいファイルを作成する / Create a new file in a folder
```.js
function createNewFileInFolder(){
 
  const folderId = '1234ABCD';
  const folder = DriveApp.getFolderById(folderId);
   
  const fileName = 'newFile';
  const newFile = folder.createFile(fileName, 'Hello, world');
}
```

### フォルダー内のファイルリスト / List of files in a folder
```.js
function listOfFilesInFolder(){
 
  const folderId = '1234ABCD';
  const files = DriveApp.getFolderById(folderId).getFiles();
   
  while (files.hasNext()) {
     
    const file = files.next();
    Logger.log('fileId-> ' + file.getId() + ', fileName-> ' + file.getName());
     
  }
}
```
