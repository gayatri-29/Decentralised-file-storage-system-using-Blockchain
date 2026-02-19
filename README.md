# Decentralised File Storage System

A decentralized image upload platform built using Solidity, React, and IPFS.
This project allows users to securely upload images to IPFS and control access permissions through Ethereum smart contracts.

# Project Overview

This application replicates a simplified decentralized version of Google Drive for images. Instead of storing files on centralized servers, images are stored on IPFS and access control is managed using a Solidity smart contract deployed on the Ethereum blockchain.

Users can:

1.Upload images to IPFS

2.Store the IPFS hash on the blockchain

3.Grant access to specific Ethereum addresses

4.Revoke access when needed

5.View images shared with them

# Tech Stack

1. Solidity – Smart contract for ownership and access control

2. Hardhat – Ethereum development environment

3. React.js – Frontend user interface

4. IPFS (Pinata) – Decentralized image storage

5. MetaMask – Wallet integration for blockchain interaction

# Features
1. Decentralized Storage

   Images are uploaded to IPFS via Pinata, ensuring decentralized and immutable storage.

2. Smart Contract Access Control

   Ownership and permission management are handled via Solidity smart contracts deployed on Ethereum.

3. Grant / Revoke Access

   Users can grant or revoke image access to specific Ethereum addresses.

4. Secure & Transparent

   All access permissions are recorded on the blockchain.

# Installation & Setup
1. Install Hardhat Dependencies
   npm install 

2. Compile Smart Contract
   npx hardhat compile

3. Deploy Smart Contract
   npx hardhat run scripts/deploy.js --network <network-name>

4. Setup React Frontend
   cd client
   npm install
   npm start 

# Configuration
Pinata API Setup

Create an account at https://www.pinata.cloud

Generate API Key and Secret

Add your API keys inside:
client/src/components/FileUpload.js
