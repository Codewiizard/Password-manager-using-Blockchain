# 🔐 Password Manager using Blockchain

This project is a Password Manager built on the Aptos blockchain utilizing the Move programming language for smart contracts and TypeScript for the frontend. The password manager ensures secure storage and access to sensitive credentials by leveraging blockchain's transparency and immutability.

---

## Features

- **Secure Credential Storage**: Store encrypted passwords on the Aptos blockchain.
- **Immutable History**: Track password changes with blockchain transparency.
- **Decentralized**: No central authority controlling access.
- **User Authentication**: Frontend ensures only the authorized user can manage their passwords.
- **Encryption**: Passwords are encrypted before storage for extra security.

---

## Technologies Used

- **Aptos Blockchain**: Base layer for storing data in a decentralized way.
- **Move Language**: Used to write smart contracts on the Aptos platform.
- **TypeScript**: For building a user-friendly frontend and interacting with the blockchain.
- **Aptos SDK**: To connect the frontend to the Aptos network.

---

## Prerequisites

- **Node.js**: Ensure Node.js is installed. [Download Node.js](https://nodejs.org)  
- **Aptos CLI**: Install Aptos CLI for deploying Move contracts.  
- **Aptos Wallet**: Set up an Aptos wallet for testing.
- **Typescript**: Install TypeScript globally if not already installed:


## Setup Instructions

1. **Clone the repository**
2. **Install dependencies:**
   ```bash
   npm install
   ```
3.**Compile the Move contract:**
   ```bash
aptos move compile --package-dir ./move_contract
   ```
4.**Deploy the Move contract:**
Replace <account_address> with your Aptos wallet address:
```bash
aptos move publish --package-dir ./move_contract --sender <account_address>
   ```
5.**Configure environment variables:**
Create a .env file with the following variables:
```bash
APTOS_NETWORK=https://fullnode.devnet.aptoslabs.com/v1
CONTRACT_ADDRESS=<deployed_contract_address>
   ```
6.**Run the frontend:**
```bash
npm run start
   ```
---
## Frontend Overview

The frontend, built in **TypeScript**, interacts with the Aptos blockchain to provide a user-friendly interface for password management.
---
### Key Features:

- **Password Encryption**: Uses AES or another encryption algorithm before storing data.
- **Blockchain Interaction**: Uses Aptos SDK to interact with smart contracts.
- **Account Management**: Displays saved accounts and allows updates.

---

## Usage

1. **Login with Aptos Wallet**: Connect your Aptos wallet.
2. **Add Password**: Enter account details and encrypted password.
3. **Update Password**: Modify existing credentials.
4. **View Accounts**: Display stored accounts from the blockchain.

---

## License

This project is licensed under the [MIT License](https://opensource.org/licenses/MIT).

---
