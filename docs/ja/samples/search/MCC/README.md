# MCCアカウント / MCC account


## MCC配下の全てのアカウント情報を取得する / Get all accounts
```.js
function getAllMccAccounts(){
  
  const managerAccountId = AdsUtilities.getCurrentAccountId();
  
  const accountLinks = Search.AccountLinkService.get({
    managerAccountId: managerAccountId,
  }).rval;
   
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
function pauseAllAccounts(){
  
  const managerAccountId = AdsUtilities.getCurrentAccountId();
  
  const accountLinks = Search.AccountLinkService.get({
    managerAccountId: managerAccountId,
  }).rval;
  
  let accountIds = [];
  for (let i = 0; i < Object.keys(accountLinks.values).length; i++){
    let accountLink = accountLinks.values[i].accountLink;
    accountIds.push(accountLink.accountId);
  }
   
  const accountsGet = Search.AccountService.get({
    accountIds: accountIds,
  }).rval;
   
  for (let i = 0; i < Object.keys(accountsGet.values).length; i++){
    let account = accountsGet.values[i].account;
    account.deliveryStatus = 'PAUSED';
    
    const accountsSet = Search.AccountService.set({
      accountId: account.accountId,
      operand: [account],
    }).rval;
    
    if (accountsSet.values[0].operationSucceeded) {
      Logger.log('accountId-> ' + accountsSet.values[0].account.accountId
        + ', accountName-> ' + accountsSet.values[0].account.accountName 
        + ' has been stopped.');
      
    } else {
      Logger.log('accountId-> ' + account.accountId + ' could not be stopped.');
      
    }
  }
}
```
