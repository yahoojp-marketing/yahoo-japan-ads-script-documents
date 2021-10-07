# Account


## Get details on the current account
```.js
function getAccount(){
 
    const accountId = AdsUtilities.getCurrentAccountId();
     
    const account = Search.AccountService.get({
        "accountIds": [
            accountId
        ],
    }).rval.values[0].account;
     
    Logger.log('accountId => ' + account.accountId + ', accountName => ' + account.accountName);
     
}
```

## Pause a account
```.js
function pauseAccount(){
 
    const accountId = AdsUtilities.getCurrentAccountId();
     
    const accountsGet = Search.AccountService.get({
        "accountIds": [
            accountId
        ],
    }).rval;
     
    let accountArray = [];
     
    for (let i = 0; i < accountsGet.totalNumEntries; i++) {
        let account = accountsGet.values[i].account;
         
        account.deliveryStatus = "PAUSED";
         
        accountArray.push(account);
    }
     
    const accountsSet = Search.AccountService.set({
        "accountId": accountId,
        "operand": accountArray,
    }).rval;
 
    for (let i = 0; i < Object.keys(accountsSet.values).length; i++){
        let account = accountsSet.values[i].account;
         
        Logger.log('accountId -> ' + accountId + ', deliveryStatus -> ' + account.deliveryStatus);
    }
}
```