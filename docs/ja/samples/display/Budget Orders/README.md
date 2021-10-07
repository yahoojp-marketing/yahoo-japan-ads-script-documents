# Budget Orders

### Set budget order
```.js
function setBudgetOrder(){
 
    const accountId = AdsUtilities.getCurrentAccountId();
     
    const budgetOrdersGet = Display.BudgetOrderService.get({
        "accountIds": [
            accountId,
        ]
    }).rval;
     
    let budgetOrderArray = [];
 
    for (let i = 0; i < budgetOrdersGet.totalNumEntries; i++){
        let budgetOrder = budgetOrdersGet.values[i].budgetOrder;
         
        budgetOrder.amount = 100000;
         
        budgetOrderArray.push(budgetOrder);
    }
     
    const budgetOrdersSet = Display.BudgetOrderService.set({
        "accountId": accountId,
        "operand": budgetOrderArray,
    }).rval;
 
    for (let i = 0; i < Object.keys(budgetOrdersSet.values).length; i++){
        let budgetOrder = budgetOrdersGet.values[i].budgetOrder;
         
        Logger.log('accountType-> ' + budgetOrder.accountType
            + ', amount-> ' + budgetOrder.amount
            + ', limitChargeType-> ' + budgetOrder.limitChargeType);
    }
}
```

### Get budget order
```.js
function getBudgetOrder(){
 
    const accountId = AdsUtilities.getCurrentAccountId();
     
    const budgetOrders = Display.BudgetOrderService.get({
        "accountIds": [
            accountId,
        ]
    }).rval;
 
    for (let i = 0; i < budgetOrders.totalNumEntries; i++){
        let budgetOrder = budgetOrders.values[i].budgetOrder;
         
        Logger.log('accountType-> ' + budgetOrder.accountType
            + ', amount-> ' + budgetOrder.amount
            + ', limitChargeType-> ' + budgetOrder.limitChargeType);
    }
}
```
