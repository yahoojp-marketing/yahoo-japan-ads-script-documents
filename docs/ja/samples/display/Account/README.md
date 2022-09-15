# アカウント / Account

### アカウント詳細情報を取得する / Get details on the current account
```.js
function getDetailsOnCurrentAccount() {
 
  const accountId = AdsUtilities.getCurrentAccountId();
     
  const account = Display.AccountService.get({
    accountIds: [accountId],
  }).rval.values[0].account;
   
  Logger.log('accountId-> ' + account.accountId + ', accountName-> ' + account.accountName);
}
```

### アカウントを配信停止にする / Pause an account
```.js
function pauseAccount() {

  const accountId = AdsUtilities.getCurrentAccountId();
  
  const accountGet = Display.AccountService.get({
    accountIds: [accountId],
  }).rval.values[0].account;
  
  accountGet.deliveryStatus = 'PAUSED';

  const accountsSet = Display.AccountService.set({
    accountId: accountId,
    operand: [accountGet],
  }).rval;

  if (accountsSet.values[0].operationSucceeded) {
    Logger.log('accountId-> ' + accountsSet.values[0].account.accountId + ' have paused.');

  } else {
    Logger.log('accountId-> ' + accountId + ' could not to be paused.');
    
  }
}
```
