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

contract SmartContract{
    function validateInput(uint256 inputValue) public pure {
        require(inputValue < 100, "Input exceeds the maximum allowed value of 99");
    }
    function checkValue(uint256 value) public pure {
        if (value >= 100) {
            revert("Value is out of the permitted range (must be less than 100)");
        }
    }
    function ensureSpecificValue(uint256 number) public pure {
        assert(number == 50);
    }
    function customRequireCheck(uint256 amount) public pure {
        bool AmountValid = amount < 100;
        if (AmountValid) {
            require(false, "Amount is too high (must be less than 100)");
        }
    }
    function customAssertCheck(uint256 inputValue) public pure {
        bool InputFifty = (inputValue == 50);
        assert(InputFifty);
    }
}

```


```

## Authors

Julian Caster Troy Lopez





