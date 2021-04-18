# Synch Trading Pool Smart Contracts

These smart contracts are in beta, please use it at your own risk.

First standalone version was tested in the mainnet at March 3, 2021

Auditing has not yet.

## Pool Choices
1. Standalone pool
    Does not have any privacy feature. Only 1 smart contract required
2. Privacy pools
    System of smart contracts achieving the goal of privacy. Each system has 1 Synch Controller contract in charge of trading and storage and multiple Synch privacy pool contracts in charge of deposit/withdraw, synch security deposit and LP token issuance. Each trade request in Synch Controller has to contain a Keccak256 hash proof to help verify later on that the transaction was genuine

Synch Tech Team
