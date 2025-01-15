# FINAL PROJECT

Over the past weeks, we have thoroughly explored what blockchain represents, its architecture, and how to build on it. Now, it's time to bring all these concepts together and create your first decentralized application.

---
## File Structure

```
.
├── README.md
├── client
│   ├── README.md
│   ├── jsconfig.json
│   ├── next.config.mjs
│   ├── package-lock.json
│   ├── package.json
│   ├── postcss.config.mjs
│   ├── src
│   │   └── app
│   │       ├── favicon.ico
│   │       ├── fonts
│   │       │   ├── GeistMonoVF.woff
│   │       │   └── GeistVF.woff
│   │       ├── globals.css
│   │       ├── layout.js
│   │       └── page.js
│   ├── tailwind.config.js
│   └── yarn.lock
├── core
│   ├── README.md
│   ├── contracts
│   │   └── Lock.sol
│   ├── hardhat.config.ts
│   ├── ignition
│   │   └── modules
│   │       └── Lock.ts
│   ├── package.json
│   ├── test
│   │   └── Lock.ts
│   ├── tsconfig.json
│   └── yarn.lock
├── fundme
│   ├── Cargo.lock
│   ├── Cargo.toml
│   ├── README.md
│   ├── docs.md
│   ├── examples
│   │   └── counter.rs
│   ├── header.png
│   ├── licenses
│   │   ├── Apache-2.0
│   │   ├── COPYRIGHT.md
│   │   ├── DCO.txt
│   │   └── MIT
│   ├── rust-toolchain.toml
│   └── src
│       ├── lib.rs
│       └── main.rs
└── scripts
    ├── Cargo.toml
    └── src
        └── main.rs

16 directories, 38 files
```
You have above a template of 4 major folders. 

1. `Client`: build an interface that communicates with your solidity smart contract
2. `Core`: A folder that contains the smart contract and it's tests. This template was created using hardhat, typescript and viem.
3. `Fundme`: This is the final piece of the project. A stylus implement of a fundme contract.
4. `Scrpts`: This is a script that interacts with the fundme contract written in rust.


## IMPLEMENTATION
To successfully complete this module, you are required to build two DApps: one using Solidity and one using Rust. Below, you will find a list of five optional DApp examples to build with Solidity and the required "FundMe" DApp to build with Rust. You only need to select one of the optional Solidity DApps and complete the required "FundMe" DApp in Rust.  

For the Rust implementation (FundMe), there is no need to connect to a UI client. Instead, you are required to write Rust scripts that interact with your smart contract. These scripts should be placed in the `scripts` folder.

## OPTIONAL DAPPS

### **1. Decentralized Marketplace**  
**Objective:** Create a platform where users can buy and sell products or services using cryptocurrency.  

**Features:**  
- **Product Listings:** Sellers can list items for sale with a price in cryptocurrency.  
- **Purchase Mechanism:** Buyers can purchase items via a smart contract.  
- **Escrow Service:** Funds are held in escrow until the buyer confirms receipt of the product.  
- **Rating System:** Enable users to rate transactions for trust-building.  

---

### **2. Supply Chain Tracker**  
**Objective:** Develop a platform to track the lifecycle of products from manufacturing to the consumer.  

**Features:**  
- **Product Registration:** Manufacturers can register products on the blockchain with unique IDs.  
- **Status Updates:** Track product status (e.g., shipped, received) via smart contracts.  
- **Transparency:** Allow end-users to verify the product's authenticity and origin.  
- **QR Code Integration:** Scan a QR code to fetch the product's blockchain history.  

---

### **3. Decentralized Lending and Borrowing Platform**  
**Objective:** Create a simple lending DApp where users can lend cryptocurrency to earn interest or borrow against collateral.  

**Features:**  
- **Lending Pool:** Lenders deposit funds into a pool to earn interest.  
- **Collateralized Loans:** Borrowers deposit collateral to take loans.  
- **Smart Contract Automation:** Automate interest calculations and loan repayments.  

---


### **4. Blockchain-Based Identity Management System**  
**Objective:** Create a DApp where users can securely store and verify their identity documents.  

**Features:**  
- **Document Upload:** Users can upload and verify identity documents (e.g., passports, licenses).  
- **Decentralized Storage:** Use IPFS or similar for document storage with a blockchain-based hash for verification.  
- **Verification Requests:** Third parties can request to verify a user’s identity.  
- **Permissioned Access:** Users control who can view their documents.  

---

### **5. Proof-of-Attendance Token System**  
**Objective:** Build a system that issues proof-of-attendance tokens (POAPs) to users attending specific events.  

**Features:**  
- **Event Creation:** Event organizers can create events and issue unique tokens.  
- **Attendance Verification:** Users receive tokens after proving attendance (e.g., scanning a QR code).  
- **NFT Display:** Users can view their tokens in a digital wallet as collectibles.  

---

## REQUIRED DAPP (RUST)
### FUNDME  
Objective: Build a platform where users can donate funds to various causes and track how donations are spent.

**Features:**  

- **Campaign Creation:** Allow NGOs or individuals to create donation campaigns.
- **Transparent Donations:** Record all donations on the blockchain for transparency.
- **Goal Tracking:** Track the progress toward the campaign’s funding goal.
- **Donor Recognition:** Issue NFTs as badges to recognize donors.

>NOTE: YOU ARE NOT REQUIRED TO BUILD YOUR FUNDME WITH STYLUS. YOU ARE ALLOWED TO EXPLORE OTHER CHAINS LIKE POLKADOT, CONCORDIUM, SUI AND SOLANA !!!.