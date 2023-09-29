## BCDV_4028_Assignment_01_101504708
Assignment 01 for BCDV 4028 - Advanced Smart Contracts

Anishkumar Pankajkumar Patel

101504708

---

# Cross-Chain ERC20 Bridge Application

## Introduction
This application is a cross-chain ERC20 bridge that allows for the transfer of tokens from one blockchain network to another. It includes two bridge contracts and two ERC20 token contracts. It is demonstrated on two Ethereum testnets.

## Contracts
1. `BridgeA.sol`: Handles locking and releasing of tokens on the source blockchain.
2. `BridgeB.sol`: Handles the minting of tokens on the destination blockchain.
3. `TokenA.sol`: ERC20 token contract for the source blockchain.
4. `TokenB.sol`: ERC20 token contract for the destination blockchain.

## Testnets Used
1. Ganache local testnet
2. Sepolia testnet

## Contract Addresses
- `BridgeA`: ```0xd75f4178Be0497BA8A77046569599B54C539f3f2``` Ganache BridgeA Address
- `BridgeB`: ```0xB4fe84040A272A028D593f29d4e2ad660d85cd8A``` Sepolia BridgeB Address
- `TokenA`: ```0xcd79caC35aFb2A54EdfB3E9e2F78B252cfe52DF7``` Ganache TokenA Address
- `TokenB`: ```0x26CE552E97f1974B7cc0a3B73372B2899c2eDE97``` Sepolia TokenB Address
- `Wallet Metamask`: ```0x2C60503A0A02D73E64CdC22303977f1768127751``` Sepolia Wallet Address
- `Wallet Ganache`: ```0xE378BC1F244ed543A96649D236d5237edD781dD5``` Ganache Walled Address
## Installation and Setup
1. Clone the repository.
2. Make sure to install nodejs, truffle, ethers and fs. 
3. Compile the contracts using `truffle compile`.
4. Deploy the contracts to the respective testnets using -
   - ```truffle migrate --network development```. (Considering ```development``` as Ganache settings in ```truffle-config.js```)
   - ```truffle migrate --network sepolia```. (Considering ```sepolia``` as Sepolia settings in ```truffle-config.js```)


## Testing
Run the truffle test using the following command:
- ```truffle test```

This will run the test file ```test/bridgeA.test.js```, which tests the BridgeA contract.

## Demonstration Script
Run the demonstration script using the following command:
- ```truffle exec scripts/bridge_demo.js --network development```

This script will demonstrate sending and receiving tokens over the bridge.

## Screenshots
Included are the screenshots demonstrating token transfers and the passing of unit tests.

- Screenshot of ```truffle test``` output.
  ![Screenshot_2](https://github.com/apatel2582/BCDV_4028_Assignment_01_101504708/assets/126298288/72b47e49-4dc5-4a8c-a01f-ea26f28ad4aa)
- Screenshot of sending tokens from one bridge to another.
  ![Screenshot_1](https://github.com/apatel2582/BCDV_4028_Assignment_01_101504708/assets/126298288/b57ea4a1-7113-4f27-abe0-8e825171dc1b)
  ![Screenshot_4](https://github.com/apatel2582/BCDV_4028_Assignment_01_101504708/assets/126298288/0bdc3262-05bf-42ec-b94a-8c57a8742027)
  ![Screenshot_5](https://github.com/apatel2582/BCDV_4028_Assignment_01_101504708/assets/126298288/4c58cacd-b8a6-4e3b-9c91-76922b6a339d)
  ![Screenshot_6](https://github.com/apatel2582/BCDV_4028_Assignment_01_101504708/assets/126298288/9eb58354-0f08-45d0-aa3e-e80432178c06)
  ![Screenshot_3](https://github.com/apatel2582/BCDV_4028_Assignment_01_101504708/assets/126298288/5a96eaec-9f5f-4ec7-86d5-9b711d10b2d8)
- Screenshot of receiving tokens on the other side of the bridge.
  ![Screenshot_8](https://github.com/apatel2582/BCDV_4028_Assignment_01_101504708/assets/126298288/a45fd701-ef07-44d8-a342-e9b30e22c584)
  ![Screenshot_9](https://github.com/apatel2582/BCDV_4028_Assignment_01_101504708/assets/126298288/e72e4f9b-5ea0-4750-bcd3-cac8d9afe096)
  ![Screenshot_10](https://github.com/apatel2582/BCDV_4028_Assignment_01_101504708/assets/126298288/95c2148a-f7c4-48ba-b6d5-f26191e09e8f)
  ![Screenshot_7](https://github.com/apatel2582/BCDV_4028_Assignment_01_101504708/assets/126298288/18da68af-3798-4a45-8fc9-0fe4bc22d52d)

## Thank You!
