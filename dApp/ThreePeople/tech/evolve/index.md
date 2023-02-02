# Introduction
The SOP of evolving smart contract in production which makes dApp upgradeable.

# Archetect
- features:
  1. Downward compatible. At any point of time, user with certain ealier version can interact with others who have new version.
  2. Extenable. The whole system is avaliable to add new features with low cost.

- Archetect:


# Common practice
## Using delegatecall
Use delegatecall to choose contracts in context of runtime.[Official doc about delegatecall](https://docs.soliditylang.org/en/v0.4.21/introduction-to-smart-contracts.html#delegatecall-callcode-and-libraries)
- Pros:
- Cons:
  1. The methods in the proxy contract must have logic contract address as input.
## Separate state and logic contract
Seperate the data part and logic part of contracts.
- Pros:
- Cons:
  1. Everytime the contract iterates, the user needs to switch to new contract.

# Reference
https://dev.to/mrhmp/evolving-ethereum-smart-contracts-in-production-without-dataloss-2196