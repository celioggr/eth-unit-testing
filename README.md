# eth-unit-testing

This repository has the test setup used for unit testing on Openzeppelin implementation. It is supposed to test ERC20 behaviours and the implementation itself (buggy or not).

## Dependencies

For this test setup, following are the modules being used and its versions.


* openzeppelin/contracts@v2.5.0
* openzeppelin/test-environment@0.1.4
* openzeppelin/test-helpers@0.5.5
* mocha@7.1.1
* chai@4.2.0

## Test environment setup

setup_env script will create a truffle project, a npm package to accomodate and install locally the above modules.

### Manual steps are required after script execution

Edit *package.json*

    "scripts": {
    -  "test": "npx truffle test"
    +  "test": "npx mocha --exit --recursive"
    }
    
Edit *truffle-config.js*
    
    / package.json
    mocha: {
    // timeout: 100000
    },
    + plugins: ["solidity-coverage"],
    
# Usage

Some commands commonly used.

##### Run test coverage 
    npx truffle run coverage 
##### Run tests
    npm test
##### Compile
    npm truffle compile
