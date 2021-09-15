# MCC


## Get all accounts
```$xslt
function getAllMccAccounts(){
   
  const managerAccountId = AdsUtilities.getCurrentAccountId();
  
  const accountLinks = Display.AccountLinkService.get({
    managerAccountId: managerAccountId,
  }).rval;
   
  for (let i = 0; i < accountLinks.totalNumEntries; i++){
    let accountLink = accountLinks.values[i].accountLink;
     
    Logger.log("accountId-> " + accountLink.accountId + ", linkAccessPermission-> " + accountLink.linkAccessPermission + ", ownerShipType-> " + accountLink.ownerShipType);
  }
   
}
```

## Pause a account
```$xslt
function pauseAnAccounts(){
  
  const managerAccountId = AdsUtilities.getCurrentAccountId();
  
  const accountLinks = Display.AccountLinkService.get({
    managerAccountId: managerAccountId,
  }).rval;
   
  let accountIdsArray = [];
   
  for (let i = 0; i < accountLinks.totalNumEntries; i++){
    let accountLink = accountLinks.values[i].accountLink;
     
    accountIdsArray.push(accountLink.accountId);
  }
   
  const accountsGet = Display.AccountService.get({
    accountIds: accountIdsArray,
  }).rval;
   
  for (let i = 0; i < accountsGet.totalNumEntries; i++){
    let account = accountsGet.values[i].account;
     
    account.deliveryStatus = "PAUSED";
 
    const accountsSet = Display.AccountService.set({
      accountId: account.accountId,
      operand: [
        account,
      ],
    }).rval;
     
    Logger.log("accountId-> " + accountsSet.values[0].account.accountId + ", deliveryStatus-> " + accountsSet.values[0].account.deliveryStatus);
  }
 
}
```
