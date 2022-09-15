# アカウント予算 / Budget Orders

### アカウント予算情報の更新をする / Set budget order
```.js
function setBudgetOrder() {
  
  const accountId = AdsUtilities.getCurrentAccountId();
  
  let budgetOrderGet = Display.BudgetOrderService.get({
    accountIds: [accountId],
  }).rval.values[0].budgetOrder;

  if (budgetOrderGet.accountType != 'INVOICE') {
    Logger.log('This accountId could not set amount because accountType is not INVOICE.');
    return;
  }
  
  budgetOrderGet.amount = 100000;
  
  const budgetOrderSet = Display.BudgetOrderService.set({
    accountId: accountId,
    operand: [budgetOrderGet],
  }).rval;
  
  if (budgetOrderSet.values[0].operationSucceeded) {
    let budgetOrder = budgetOrderSet.values[0].budgetOrder;
    Logger.log('This accountId set as limitChargeType-> ' + budgetOrder.limitChargeType
      + ' to amount-> ' + budgetOrder.amount);
    
  } else {
    Logger.log('This accountId could not to set as limitChargeType-> ' + budgetOrderGet.limitChargeType
      + ' to amount-> ' + budgetOrderGet.amount);
    
  }
}
```

### アカウント予算情報の取得する / Get budget order
```.js
function getBudgetOrder() {
  
  const accountId = AdsUtilities.getCurrentAccountId();
  
  const budgetOrder = Display.BudgetOrderService.get({
    accountIds: [accountId],
  }).rval.values[0].budgetOrder;
  
  Logger.log('accountType-> ' + budgetOrder.accountType
    + ', amount-> ' + budgetOrder.amount
    + ', limitChargeType-> ' + budgetOrder.limitChargeType);
}
```
