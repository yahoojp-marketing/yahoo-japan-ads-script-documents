# アカウント予算 / Budget Orders

### アカウント予算情報を更新する / Set budget order
```.js
function setBudgetOrder(){
     
  const accountId = AdsUtilities.getCurrentAccountId();
   
  const budgetOrdersGet = Search.BudgetOrderService.get({
    accountIds: [accountId],
  }).rval;
  
  if (budgetOrdersGet.totalNumEntries == 0) {
    Logger.log('Target ID does not exist.');
    return;
  }
  
  let budgetOrder = budgetOrdersGet.values[0].budgetOrder;
  if (budgetOrder.accountType != 'INVOICE') {
    Logger.log('Target ID of INVOICE does not exist.');
    return;
  }
  budgetOrder.amount = 3000;//Budget amount is 1000 yen unit, 3000 yen or more
   
  const budgetOrdersSet = Search.BudgetOrderService.set({
    accountId: accountId,
    operand: [budgetOrder],
  }).rval;
   
  if (budgetOrdersSet.values[0].operationSucceeded) {
    Logger.log('accountId-> ' + accountId + ' has been changed to amount-> ' + budgetOrdersSet.values[0].budgetOrder);
          
  } else {
    Logger.log('accountId-> ' + accountId + ' budget could not be changed.');
        
  }
}
```

### アカウント予算情報を取得する / Get budget order
```.js
function getBudgetOrder(){
     
  const accountId = AdsUtilities.getCurrentAccountId();
   
  const budgetOrders = Search.BudgetOrderService.get({
    accountIds: [accountId],
  }).rval;
  
  if (budgetOrders.totalNumEntries == 0) {
    Logger.log('Target ID does not exist.');
    return;
  }
   
  let budgetOrder = budgetOrders.values[0].budgetOrder;
  Logger.log('accountId-> ' + accountId + ', accountType-> ' + budgetOrder.accountType
    + ', amount-> ' + budgetOrder.amount + ', limitChargeType-> ' + budgetOrder.limitChargeType);
}
```

