# アカウント / Account


## アカウント詳細情報を取得する / Get details on the current account
```.js
function getAccount(){
 
  const accountId = AdsUtilities.getCurrentAccountId();
   
  const accounts = Search.AccountService.get({
    accountIds: [accountId],
  }).rval;
  
  if (accounts.totalNumEntries == 0) {
    Logger.log('Target ID does not exist.');
    return;
  }

  let account = accounts.values[0].account;
  Logger.log('accountId-> ' + account.accountId + ', accountName-> ' + account.accountName);
}
```

## アカウントを配信停止にする / Pause an account
```.js
function pauseAccount(){
 
  const accountId = AdsUtilities.getCurrentAccountId();
   
  const accountsGet = Search.AccountService.get({
    accountIds: [accountId],
  }).rval;
  
  if (accountsGet.totalNumEntries == 0) {
    Logger.log('Target ID does not exist.');
    return;
  }
  
  let account = accountsGet.values[0].account;
  account.deliveryStatus = 'PAUSED';
   
  const accountsSet = Search.AccountService.set({
    accountId: accountId,
    operand: [account],
  }).rval;

  if (accountsSet.values[0].operationSucceeded) {
    Logger.log('accountId -> ' + accountId + ', accountName-> ' + accountsSet.values[0].account.accountName
      + ' has been paused.');
    
  } else {
    Logger.log('accountId -> ' + accountId + ', accountName-> ' + accountsGet.values[0].account.accountName
      + ' could not be stopped.');
    
  }
}
```
