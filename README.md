# Coin Cast

## Problem Statement

Zora creators who minted ERC20 tokens earned LP fees from trading activity, but there was no mechanism to reward the Farcaster community members who actively promoted and supported their content through social engagement. This created a disconnect between on-chain economics and off-chain social influence, leaving valuable community contributors unrewarded for their efforts in driving token adoption and trading volume.

## Solution

We built Coin Cast that enabled Zora creators to delegate a portion of their LP fees to their top 25 Farcaster mindshare contributors. The system established a direct link between social media engagement and financial rewards, creating an incentive structure that aligned creator success with community participation.

## How It Worked

### Zora SDK Integration

The application integrated with the Zora SDK to:
- Connect to creators' Zora posts and ERC20 tokens
- Access LP fee streams from token trading activity
- Redirect fee payments from creators to the distribution system
- Monitor token performance and trading metrics

### Splits Contract Implementation

We utilized Splits.org smart contracts to handle the automated distribution of rewards:
- Created distribution contracts that could handle multiple recipients
- Configured the top 25 mindshare contributors as beneficiaries
- Automated the fee splitting process without manual intervention
- Ensured transparent and trustless reward distribution

### Mindshare Calculation Engine

The system implemented a sophisticated mindshare algorithm that:
- Collected real-time data from Farcaster via the Neynar API
- Analyzed social engagement metrics including reactions, recasts, mentions, and follower counts
- Applied weighted scoring to determine the most influential contributors
- Updated rankings weekly to reflect current community dynamics
- Identified the top 25 contributors who would receive fee distributions

## Key Features

- **Creator Dashboard**: Allowed creators to select Zora posts for delegation and configure reward settings
- **Mindshare Leaderboard**: Displayed top contributors and their engagement metrics
- **Automated Distribution**: Seamlessly distributed LP fees to community members
- **Mobile-First Design**: Optimized for Farcaster's mobile-centric user base
- **Real-Time Updates**: Provided live feedback on community engagement and rewards

### Use of Zora Coins and coin sdk

- Coincast frontend contains the main logic of how creators can delegate the revenue of their zora coins. You can look atHooks folder and dashboard code for reference.
- Coin cast Backend contains the logic of reward collection and delegation of the reward to the users.

## Impact

The project successfully bridged the gap between social influence and economic rewards in the Web3 creator economy. Creators could now directly compensate their most engaged community members, while supporters had tangible incentives to actively promote content they believed in. This created a sustainable ecosystem where social engagement translated into real financial value for all participants.


