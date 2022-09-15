# MCCアカウント / MCC account


## MCCアカウント配下の全てのアカウント情報を取得する / Get all accounts
```.js
function getAllMccAccounts() {
  
  const managerAccountId = AdsUtilities.getCurrentAccountId();
  
  const accountLinks = Display.AccountLinkService.get({
    managerAccountId: managerAccountId,
  }).rval;
  
  if (accountLinks.totalNumEntries == 0) {
    Logger.log('accountId does not exist.');
    return;
  }
  
  for (let i = 0; i < Object.keys(accountLinks.values).length; i++){
    let accountLink = accountLinks.values[i].accountLink;
    
    Logger.log('accountId-> ' + accountLink.accountId 
      + ', linkAccessPermission-> ' + accountLink.linkAccessPermission 
      + ', ownerShipType-> ' + accountLink.ownerShipType);
  }
}
```

## MCCアカウント配下の全てのアカウントを配信停止にする / Pause all accounts
```.js
function pauseAllAccounts() {
  
  const managerAccountId = AdsUtilities.getCurrentAccountId();
  
  const accountLinks = Display.AccountLinkService.get({
    managerAccountId: managerAccountId,
  }).rval;
  
  let accountIdsArray = [];
  for (let i = 0; i < Object.keys(accountLinks.values).length; i++){
    let accountLink = accountLinks.values[i].accountLink;
    accountIdsArray.push(accountLink.accountId);
  }
   
  const accountsGet = Display.AccountService.get({
    accountIds: accountIdsArray,
  }).rval;

  if (accountsGet.totalNumEntries == 0) {
    Logger.log('accountId does not exist.');
    return;
  }
  
  for (let i = 0; i < Object.keys(accountsGet.values).length; i++){
    let account = accountsGet.values[i].account;
    account.deliveryStatus = 'PAUSED';
    
    const accountsSet = Display.AccountService.set({
      accountId: account.accountId,
      operand: [account],
    }).rval;
    
    if (accountsSet.values[0].operationSucceeded) {
      Logger.log('accountId-> ' + accountsSet.values[0].account.accountId + ' have been stopped.');
        
    } else {
      Logger.log('accountId-> ' + account.accountId + ' could not to be stopped.');
      
    }
  }
}
```
