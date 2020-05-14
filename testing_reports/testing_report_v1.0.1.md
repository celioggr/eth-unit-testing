------------------------------------------------------------------------------------------------------------------------------------------------------
Bug : Amount to be transfered is amount*amount
_balances[recipient] = _balances[recipient].add(amount*amount); 
------------------------------------------------------------------------------------------------------------------------------------------------------
      AssertionError: expected '10000' to equal '100'
      + expected - actual

      -10000
      +100
      
      at Context.<anonymous> (test/ERC20.behavior.js:182:64)
      at runMicrotasks (<anonymous>)
      at processTicksAndRejections (internal/process/task_queues.js:97:5)



--------------------|----------|----------|----------|----------|----------------|
File                |  % Stmts | % Branch |  % Funcs |  % Lines |Uncovered Lines |
--------------------|----------|----------|----------|----------|----------------|
 contracts/         |    70.15 |     62.5 |    68.57 |    69.12 |                |
  Context.sol       |       50 |      100 |    66.67 |    33.33 |          24,25 |
  ERC20.sol         |      100 |      100 |      100 |      100 |                |
  ERC20Detailed.sol |        0 |      100 |        0 |        0 |... 21,28,36,52 |
  ERC20Mock.sol     |      100 |      100 |      100 |      100 |                |
  GoodContract.sol  |        0 |      100 |        0 |        0 |             10 |
  IERC20.sol        |      100 |      100 |      100 |      100 |                |
  SafeMath.sol      |    36.84 |       25 |     37.5 |    36.84 |... 136,153,154 |
--------------------|----------|----------|----------|----------|----------------|
All files           |    70.15 |     62.5 |    68.57 |    69.12 |                |
--------------------|----------|----------|----------|----------|----------------|

> Istanbul reports written to ./coverage/ and ./coverage.json


------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------



Coverage analysis:

 ===== BuggycontractaProject =====

  contract: BuggyContractA - 72.9%
    ERC20.approve - 100.0%

    ERC20.totalSupply - 0.0%

    ERC20.transferFrom - 33.3%

    ERC20.increaseAllowance - 100.0%

    ERC20.balanceOf - 100.0%

    ERC20.decreaseAllowance - 100.0%

    ERC20.transfer - 100.0%

    ERC20.allowance - 100.0%

    ERC20._approve - 75.0%

    ERC20._transfer - 80.0%

    Context._msgSender - 100.0%

    SafeMath.sub - 75.0%

    SafeMath.add - 75.0%

Coverage report saved at /home/honeybadger/novoteste/reports/coverage.json
View the report using the Brownie GUI


=========================================================== 1 passed in 419.79s (0:06:59) ============================================================


