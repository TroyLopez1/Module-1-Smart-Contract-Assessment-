Smart Contract Project

Write a smart contract that implements the require(), assert() and revert() statements.

## Description

This a program to which explain and implement the use of require(), assert() and revert() statements.

## Getting Started
To run this program, you can use Remix, an online Solidity IDE. To get started, go to the Remix website at https://remix.ethereum.org/.

### Executing program

When in remix start the Project by clicking the New File under that Files section and enter the name of the project and hit enter. Paste the provided code to the remix
```
// SPDX-License-Identifier: MIT
pragma solidity ^0.8.0;

contract mycontract {
    function testRequire(uint _a) public pure {
        require(_a <= 20, "INPUT is greater than 20");
    }
    function testRevert(uint _a) public pure {
        if (_a > 20) {
            revert("INPUT is greater than 20");
        }
    }
    function testAssert(uint _a) public pure{
        assert(_a == 20);
    }
}
```


```

## Authors

Julian Caster Troy Lopez





