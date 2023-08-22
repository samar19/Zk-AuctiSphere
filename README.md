
# ZkAuctiSphere

![ZkAuctiSphere](https://github.com/samar19/pic-/blob/master/purple%20monogram%20studio%20logo.png)

This project was scaffolded with [zksync-cli](https://github.com/matter-labs/zksync-cli).

## Introduction

ZkAuctiSphere is an innovative auction platform that leverages account abstraction and zkSync technology to offer users the power of web3 and the simplicity of web2 user experience.

## Problem

Traditional auction platforms often suffer from high fees, slow transaction times, and complex user interfaces. Navigating the world of cryptocurrencies can be intimidating for newcomers, and the existing solutions lack the seamlessness and ease of use that modern consumers demand.

## Solution

ZkAuctiSphere addresses these challenges by introducing a groundbreaking approach to online auctions. Through account abstraction, it eliminates the need for excessive gas fees and minimizes transaction delays, providing users with a fluid and efficient bidding experience. The integration of zkSync technology ensures that transactions are secure and near-instantaneous, so users can bid with confidence.

## Key Features

- **Custom Paymaster:** Pay fees in DAI and USDC, exclusively for approved contracts, making auctions more accessible and cost-effective.

- **Sphere Wallet Multicalls:** Streamlined approval and execution with a single click, thanks to the integration of Sphere wallet's multicall feature.

- **One-Click Buy It Now:** Experience the future of auctions with our one-click buy it now button, bringing unprecedented convenience to your bidding journey.

## Project Structure

- `/contracts`: Smart contracts powering the auction functionality.
- `/deploy`: Deployment and contract interaction scripts.
- `/test`: Comprehensive test suite for validating contract behavior.
- `hardhat.config.ts`: Configuration file for Hardhat, our development environment.
- `/frontend`: Source code for the captivating demo site.

## Environment Variables

We prioritize your security. Our project employs the `dotenv` package to handle environment variables, ensuring your private keys remain safe. To get started, rename `.env.example` to `.env` and input your private key.

```env
WALLET_PRIVATE_KEY=123cde574ccff....
```

## Contracts

ZkAuctiSphere boasts a sophisticated array of contracts:

- [AuctionPaymaster](./contracts/AuctionPaymaster.sol): Facilitates fee payments in DAI or USDC for approved contracts.
- [ZkSyncAuctionItems](./contracts/AuctionItems.sol): Represents ERC721 NFTs that serve as items for auction.
- [Auction](./contracts/Auction.sol): Implements auctions with bid increments based on item prices and supports a convenient buy-it-now option.
- [AuctionFactory](./contracts/AuctionFactory.sol): Orchestrates the creation of new auctions.
- [mocks](./contracts/mocks/): Contains mock contracts for testing purposes.
- [Greeter](./contracts/Greeter.sol): A simple test contract that's not used in the testnet environment.

## Deployment

Deploy ZkAuctiSphere with ease:

For local testing:

```bash
yarn deploy-zkauction-local
```

For ZkSyncEra testnet:

```bash
yarn deploy-zkauction-testnet
```

## Front End

Experience ZkAuctiSphere firsthand:

1. Navigate to the `/frontend` directory.
2. Install dependencies with `yarn`.
3. Launch the local server using `yarn dev`.

Visit the local server at [http://localhost:5173/argent-zkAuction/](http://localhost:5173/argent-zkAuction/).

## Empowering Testing

ZkAuctiSphere places great emphasis on testing:

- Utilize Forge for robust and efficient testing, encompassing fuzzing techniques.
- Test contracts on a local testnet for reliable validation.

## Unlocking the Full Potential

Explore the endless possibilities of ZkAuctiSphere. Join us in shaping the future of online auctions, where blockchain meets user-friendly experience.

Discover more by visiting our [Demo Site](). Watch our [Video]() to witness ZkAuctiSphere in action.

## Overcoming Challenges

Creating ZkAuctiSphere came with its own set of hurdles, such as integrating zkSync technology seamlessly and designing a user-centric interface. However, our team's determination and expertise led us to conquer these challenges and craft a revolutionary auction platform.

## Join the Revolution

Become a part of the ZkAuctiSphere revolution today. Embrace the power of account abstraction, zkSync, and a user-first approach to auctions. Bid, buy, and win like never before with ZkAuctiSphere!
```

