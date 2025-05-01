<!-- HouseMe – Real-Estate NFT + Escrow DApp -->

<div align="center">
  <img src="src/assets/houseme-banner.png" width="720" alt="HouseMe banner"/>
</div>

# HouseMe 🏡

**HouseMe** lets anyone mint a property as an ERC-721 NFT and sell it safely through an on-chain escrow contract that mirrors a traditional real-estate closing (buyer ↔ seller ↔ inspector ↔ lender).

- **NFT title deed** – a `RealEstate.sol` token stores the off-chain metadata (IPFS) for each property.  
- **Escrow workflow** – `Escrow.sol` handles earnest money, inspection status, multi-party approvals, and automatic settlement.  
- **React front-end** – browse listings, connect MetaMask, and complete the purchase with one click.  
- **Hardhat** stack – Solidity 0.8, Ethers v5, OpenZeppelin libs, full unit-test coverage.

> Demo video → *add Loom link here*  
> Live test-net → *add Sepolia or Polygon Mumbai link here*

---

## 1. Quick Start

```bash
# clone & install
git clone https://github.com/Stephen-Odumirin/HouseMe.git
cd HouseMe
npm install          # installs both React & Hardhat deps

# compile & test
npx hardhat compile
npx hardhat test

# local chain (http://127.0.0.1:8545)
npx hardhat node
# deploy contracts to the local chain
npx hardhat run scripts/deploy.js --network localhost
