# Synch Privacy Trading Pool Smart Contract

These smart contracts are in beta, please use for testing purpose only

## Features
1. Deposit token can be pre-selected as any ERC20 token
2. Contain trading state and epoch
3. Privacy feature
4. Trade from a Uniswap-like AMM with any pairs
5. Synch token deposit required for accessing the pool

## Notice
1. During trading mode, deposit and withdraw are not allowed.
2. Airdrop feature has been removed, as it is better to done it in a Synch Trading LP pool instead.
3. Withdraw has to be in terms of base token.

## How we achieve privacy
We have one controller contract mesh all money from different pools together so when a trade happen, outsiders can not identify if the trade is for a particular pool. However we do need to submit a Keccak256 hash as a proof in the trade transaction so that later on, when fund withdraw to a particular pool, we reveal the information behind these hashes and everyone can check if the balance was correct.

Synch Tech Team
