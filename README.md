# Solana NFT Project

This repository contains the code and resources for creating and managing NFTs (Non-Fungible Tokens) on the Solana blockchain. The project demonstrates how to mint, transfer, and manage NFTs using Solana's tools and libraries.

## Table of Contents
1. [Introduction](#introduction)
2. [Features](#features)
3. [Prerequisites](#prerequisites)
4. [Installation](#installation)
5. [Usage](#usage)
6. [Contributing](#contributing)
7. [License](#license)
8. [Acknowledgments](#acknowledgments)

---

## Introduction

This project is designed to help developers understand how to create and manage NFTs on the Solana blockchain. It includes scripts and tools for minting NFTs, transferring ownership, and interacting with Solana's decentralized ecosystem.

---

## Features

- **Mint NFTs**: Create new NFTs with custom metadata.
- **Transfer NFTs**: Transfer ownership of NFTs between wallets.
- **Metadata Management**: Store and retrieve NFT metadata using Arweave or other decentralized storage solutions.
- **Solana Integration**: Leverage Solana's high-speed, low-cost blockchain for NFT transactions.
- **Command-Line Tools**: Easy-to-use CLI for interacting with the Solana network.

---

## Prerequisites

Before you begin, ensure you have the following installed:

- [Node.js](https://nodejs.org/) (v16 or higher)
- [Solana CLI](https://docs.solana.com/cli/install-solana-cli-tools)
- [Yarn](https://yarnpkg.com/) or [npm](https://www.npmjs.com/)
- A Solana wallet with some SOL (for gas fees)

---

## Installation

1. Clone the repository:
   ```bash
   git clone https://github.com/anagimenez6/SOLANA-NFT.git
   cd SOLANA-NFT
   ```

2. Install dependencies:
   ```bash
   yarn install
   # or
   npm install
   ```

3. Set up your Solana environment:
   - Connect to the Solana devnet:
     ```bash
     solana config set --url devnet
     ```
   - Fund your wallet with SOL (for testing):
     ```bash
     solana airdrop 1
     ```

---

## Usage

### Minting an NFT

1. Update the metadata file (`metadata.json`) with your NFT details (name, description, image URI, etc.).
2. Run the minting script:
   ```bash
   yarn mint-nft
   # or
   npm run mint-nft
   ```

### Transferring an NFT

1. Update the `transfer-nft.js` script with the recipient's wallet address and the NFT mint address.
2. Run the transfer script:
   ```bash
   yarn transfer-nft
   # or
   npm run transfer-nft
   ```

### Viewing NFTs

Use the Solana Explorer or a wallet like Phantom to view your NFTs:
- [Solana Explorer](https://explorer.solana.com/)
- [Phantom Wallet](https://phantom.app/)

---

## Contributing

Contributions are welcome! If you'd like to contribute, please follow these steps:

1. Fork the repository.
2. Create a new branch for your feature or bugfix:
   ```bash
   git checkout -b feature/your-feature-name
   ```
3. Commit your changes:
   ```bash
   git commit -m "Add your feature"
   ```
4. Push to the branch:
   ```bash
   git push origin feature/your-feature-name
   ```
5. Open a pull request.

---

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

---

## Acknowledgments

- [Solana Documentation](https://docs.solana.com/)
- [Metaplex](https://www.metaplex.com/) for NFT standards and tools.
- The Solana community for their support and resources.

---

For any questions or issues, feel free to open an issue or contact the maintainer.
