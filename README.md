
# Project Title: TokenStaker - Decentralized Token Staking Platform

TokenStaker is a full-stack decentralized application (DApp) built on the Ethereum blockchain that allows users to stake their tokens (StakeToken) and earn rewards (RewardToken) over time. 
This project demonstrates a secure and transparent staking mechanism, providing incentives for token holders to participate in the network.


## Project Description

The FlashLoan contract aims to capitalize on the temporary price discrepancies that can occur between different trading pairs on PancakeSwap. It achieves this by:

Borrowing a significant amount of a token (e.g., BUSD) from a PancakeSwap liquidity pool using a flash loan.

Executing a series of trades across different token pairs (e.g., BUSD -> CROX -> CAKE -> BUSD) to take advantage of price differences.

Repaying the flash loan with a portion of the acquired funds.

If the trades result in a net profit, the remaining funds are transferred to the contract owner as profit.
## Key Features

Staking: Users can stake their StakeToken (STK) to earn rewards.

Reward Distribution: Rewards (RWT) are distributed proportionally to the amount staked and the staking duration.

Reward Rate: A constant reward rate ensures predictable earnings.

Withdrawal: Users can withdraw their staked tokens and accumulated rewards.

User Interface: An intuitive front-end allows users to easily manage their staking activities.

Security: The project incorporates the OpenZeppelin library for secure smart contract development.

## Technical Overview

Blockchain: Ethereum (Chosen for its smart contract capabilities and established DeFi ecosystem)

Smart Contracts:
Language: Solidity (>=0.8.2 <0.9.0)
Staking.sol:

Manages the staking logic: staking, withdrawing, reward calculation, and distribution.

stake(uint amount): Allows users to stake their STK tokens.

withdrawStakedTokens(uint amount): Allows users to withdraw staked STK tokens.

getReward(): Allows users to claim accumulated RWT rewards.

StakeToken.sol:
ERC-20 token contract representing the stakeable asset (STK).

RewardToken.sol:
ERC-20 token contract representing the reward token (RWT).





Frontend:
Framework: React (Presumably, based on the .jsx extension)

Components:
App.jsx: Main application component, manages UI and user interactions.

Wallet.jsx: Handles wallet connection and user authentication.

Navigation.jsx: Provides navigation between different sections of the DApp.

DisplayPanel.jsx: Displays staked amount, reward rate, and earned rewards.

TokenApproval.jsx, StakeAmount.jsx: Components for staking.

Withdraw.jsx: Component for withdrawing staked tokens and rewards.
