------------------------------------------------------------------------------------------------------------------------------------------------------
Bug : Transfer event is missing and amount to transfer is amount*amount
_balances[recipient] = _balances[recipient].add(amount*amount);
//emit Transfer(sender, recipient, amount);
------------------------------------------------------------------------------------------------------------------------------------------------------
     No 'Transfer' events found
      + expected - actual

      -false
      +true
      
      at Function.inLogs (node_modules/@openzeppelin/test-helpers/src/expectEvent.js:37:32)
      at Function.deprecated [as inLogs] (internal/util.js:81:15)
      at Context.<anonymous> (test/ERC20.behavior.js:210:21)
      at runMicrotasks (<anonymous>)
      at processTicksAndRejections (internal/process/task_queues.js:97:5)



--------------------|----------|----------|----------|----------|----------------|
File                |  % Stmts | % Branch |  % Funcs |  % Lines |Uncovered Lines |
--------------------|----------|----------|----------|----------|----------------|
 contracts/         |     69.7 |     62.5 |    68.57 |    68.66 |                |
  Context.sol       |       50 |      100 |    66.67 |    33.33 |          24,25 |
  ERC20.sol         |      100 |      100 |      100 |      100 |                |
  ERC20Detailed.sol |        0 |      100 |        0 |        0 |... 21,28,36,52 |
  ERC20Mock.sol     |      100 |      100 |      100 |      100 |                |
  GoodContract.sol  |        0 |      100 |        0 |        0 |             10 |
  IERC20.sol        |      100 |      100 |      100 |      100 |                |
  SafeMath.sol      |    36.84 |       25 |     37.5 |    36.84 |... 136,153,154 |
--------------------|----------|----------|----------|----------|----------------|
All files           |     69.7 |     62.5 |    68.57 |    68.66 |                |
--------------------|----------|----------|----------|----------|----------------|

> Istanbul reports written to ./coverage/ and ./coverage.json
> solidity-coverage cleaning up, shutting down ganache server
Error: ❌ 8 test(s) failed under coverage.

------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------


Coverage analysis:

 ===== celioggr/eth-unit-testing@1.1.0 =====

  contract: TestToken - 81.2%
    ERC20.approve - 100.0%
    ERC20.totalSupply - 0.0%
    ERC20.transferFrom - 100.0%
    ERC20.increaseAllowance - 100.0%
    ERC20.balanceOf - 100.0%
    ERC20.decreaseAllowance - 100.0%
    ERC20.transfer - 100.0%
    ERC20.allowance - 100.0%
    ERC20._approve - 75.0%
    ERC20._transfer - 100.0%
    Context._msgSender - 100.0%
    SafeMath.sub - 75.0%
    SafeMath.add - 75.0%

