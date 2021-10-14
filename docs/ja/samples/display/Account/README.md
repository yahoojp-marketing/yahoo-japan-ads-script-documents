# アカウント / Account

### アカウント詳細情報を取得する / Get details on the current account
```.js
function getDetailsOnCurrentAccount(){
 
    const accountId = AdsUtilities.getCurrentAccountId();
     
    const account = Display.AccountService.get({
        "accountIds": [
            accountId
        ],
    }).rval.values[0].account;
     
    Logger.log('accountId -> ' + account.accountId + ', accountName -> ' + account.accountName);
}
```

### アカウントを配信停止にする / Pause a account
```.js
function pauseAccount(){
 
    const accountId = AdsUtilities.getCurrentAccountId();
     
    const accountsGet = Display.AccountService.get({
        "accountIds": [
            accountId
        ],
    }).rval;
 
    let accountArray = [];
     
    for (let i = 0; i < accountsGet.totalNumEntries; i++){
        let account = accountsGet.values[i].account;
         
        account.deliveryStatus = "PAUSED";
         
        accountArray.push(account);
    }
     
    const accountsSet = Display.AccountService.set({
        "accountId": accountId,
        "operand": accountArray,
    }).rval;
     
    for (let i = 0; i < Object.keys(accountsSet.values).length; i++){
        let account = accountsSet.values[i].account;
         
        Logger.log('accountId -> ' + account.accountId + ', deliveryStatus -> ' + account.deliveryStatus);
    }
}
```
