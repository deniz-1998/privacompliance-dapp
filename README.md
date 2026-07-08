# PrivaCompliance dApp 🌙 (Midnight Level 2)

This repository contains the frontend implementation, smart contract integration, and automated toolchain verification for the **PrivaCompliance** decentralized application, deployed on the **Midnight Preprod Network**.

## 📑 Privacy Claim & Observable Behavior
Our dApp proves strict regulatory and legal compliance *without revealing* the underlying user identity or sensitive credentials. 
* **The Privacy Behavior:** The ZK circuit verifies that the user's `eligibilityProof` matches network compliance criteria. The application successfully logs `isValidated: true` on the public ledger while keeping the secret witness parameter completely hidden from the public state.

## 🚀 Live Demonstration
* **Live dApp Deployment:** [https://privacompliance-dapp-ksm4.vercel.app/](https://privacompliance-dapp-ksm4.vercel.app/)
* **Preprod Contract Address:** `0000000000000000000000000000000000000000000000000000000000000001::PrivaCompliance`

## 🛠️ Technical Stack & Frameworks
* **Language:** Compact 0.1.0 & TypeScript
* **Frontend:** React 19 & Vite
* **Wallet Connector:** Midnight.js DApp Connector API (Lace Wallet Preprod)