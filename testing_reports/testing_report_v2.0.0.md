-----------------------------------------------------------------------------------------------------------------------------------------------------
Bug - in function transfer triggers Approval event instead of Transfer
-----------------------------------------------------------------------------------------------------------------------------------------------------

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
 contracts/         |    70.15 |     62.5 |    68.57 |    69.12 |                |
  Context.sol       |       50 |      100 |    66.67 |    33.33 |          24,25 |
  ERC20.sol         |      100 |      100 |      100 |      100 |                |
  ERC20Detailed.sol |        0 |      100 |        0 |        0 |... 21,28,36,52 |
  ERC20Mock.sol     |      100 |      100 |      100 |      100 |                |
  IERC20.sol        |      100 |      100 |      100 |      100 |                |
  SafeMath.sol      |    36.84 |       25 |     37.5 |    36.84 |... 136,153,154 |
  TestToken.sol     |        0 |      100 |        0 |        0 |             10 |
--------------------|----------|----------|----------|----------|----------------|
All files           |    70.15 |     62.5 |    68.57 |    69.12 |                |
--------------------|----------|----------|----------|----------|----------------|

> Istanbul reports written to ./coverage/ and ./coverage.json
> solidity-coverage cleaning up, shutting down ganache server
Error: ❌ 5 test(s) failed under coverage.


-----------------------------------------------------------------------------------------------------------------------------------------------------
-----------------------------------------------------------------------------------------------------------------------------------------------------

