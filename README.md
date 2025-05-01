# SimpleStorage.sol
# SimpleStorage Smart Contract

This is my first smart contract built using Solidity. It is a basic example that allows storing and retrieving a number on the Ethereum blockchain.

## About the Contract

The contract is called `SimpleStorage`. It has:
- A state variable `number` to store a `uint` value.
- A `setNumber()` function to update the number.
- A `getNumber()` function to read the stored number.

## Contract Code

```solidity
// SPDX-License-Identifier: MIT
pragma solidity ^0.8.0;

contract SimpleStorage {
    uint public number;

    function setNumber(uint _number) public {
        number = _number;
    }

    function getNumber() public view returns (uint) {
        return number;
    }
}
