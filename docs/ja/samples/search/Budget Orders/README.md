# Budget Orders

### Set budget order
```$xslt
function setBudgetOrder(){
     
    const accountId = AdsUtilities.getCurrentAccountId();
     
    const budgetOrdersGet = Search.BudgetOrderService.get({
        "accountIds": [
            accountId,
        ]
    }).rval;
     
    let budgetOrderArray = [];
     
    for (let i = 0; i < Object.keys(budgetOrdersGet.values).length; i++){
        let budgetOrder = budgetOrdersGet.values[i].budgetOrder;
         
        budgetOrder.amount = 100000;//Budget amount is 1000 yen unit, 3000 yen or more
         
        budgetOrderArray.push(budgetOrder);
    }
     
    const budgetOrdersSet = Search.BudgetOrderService.set({
        "accountId": accountId,
        "operand": budgetOrderArray,
    }).rval;
     
    for (let i = 0; i < Object.keys(budgetOrdersSet.values).length; i++){
        let budgetOrder = budgetOrdersSet.values[i].budgetOrder;
         
        Logger.log('accountType-> ' + budgetOrder.accountType
            + ', amount-> ' + budgetOrder.amount
            + ', limitChargeType-> ' + budgetOrder.limitChargeType);
    }
}
```

### Get budget order
```$xslt
function getBudgetOrder(){
     
    const accountId = AdsUtilities.getCurrentAccountId();
     
    const budgetOrders = Search.BudgetOrderService.get({
        "accountIds": [
            accountId,
        ]
    }).rval;
     
    for (let i = 0; i < Object.keys(budgetOrders.values).length; i++){//Object.keys()
        let budgetOrder = budgetOrders.values[i].budgetOrder;
         
        Logger.log('accountType-> ' + budgetOrder.accountType
            + ', amount-> ' + budgetOrder.amount
            + ', limitChargeType-> ' + budgetOrder.limitChargeType);
    }
}
```

