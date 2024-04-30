# Dynamic (Mood) NFT 

## Overview
This project allows users to mint Non-Fungible Tokens (NFTs) that reflect their current mood, represented by SVG images. The project includes a smart contract for minting NFTs, a deployment script, and a testing suite. The metadata for each NFT is stored on-chain and encoded in base64.
It also includes code for the deployment of a basic NFT that leverages IFPS for storage. 

## Features
- **Mood Representation**: Users can mint NFTs that represent either a "Happy" or "Sad" mood using SVG images.
- **On-chain Metadata**: Metadata for each NFT is stored directly on the blockchain and includes mood-specific details.
- **Interactivity**: Owners of the NFTs can flip the mood of their NFTs post-minting.

## Prerequisites
- Node.js (v14.x or newer recommended)
- [Foundry](https://github.com/foundry-rs/foundry) for Solidity testing and deployment
- An Ethereum wallet with Ether for deploying contracts (if deploying to a live network)

## Installation
Clone the repository and install dependencies:

```bash
git clone https://github.com/yourrepository/MoodNftProject.git
cd MoodNftProject
```

## Usage
Deploying the Contract

To deploy the Mood NFT contract, use the provided script:
```bash
forge script script/DeployMoodNft.s.sol --rpc-url <RPC_URL> --private-key <YOUR_PRIVATE_KEY> --broadcast
```
Replace <RPC_URL> and <YOUR_PRIVATE_KEY> with your Ethereum node RPC URL and private key.

## Minting an NFT

After deployment, you can mint an NFT by interacting with the deployed contract. Here is how you can do it using a script or through a frontend interface connected to your contract.

## Flipping the Mood of an NFT

Owners of the NFT can change its mood by calling the flipMood function with the NFT's token ID.

## Smart Contracts

    1. MoodNft.sol: Defines the NFT structure and minting functionality.
    2. DeployMoodNft.s.sol: Script for deploying the NFT contract.
    3. MoodNftTest.sol: Contains tests for the functionality of the Mood NFT.

## Running Tests

Execute the following command to run tests:
```bash
forge test
```
This will run unit tests defined in the test/ directory to ensure the contract functions as expected.

## Contributing

Contributions are welcome! Please feel free to submit pull requests or open issues to suggest improvements or add new features.

## License

This project is licensed under the MIT License - see the LICENSE.md file for details.



