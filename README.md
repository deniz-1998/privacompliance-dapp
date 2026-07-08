# PrivaCompliance dApp 🌌 (Midnight Level 1)

This repository contains the frontend implementation, smart contract integration, and automated toolchain verification for the **PrivaCompliance** decentralized application, deployed on the **Midnight Preprod Network**.

The application demonstrates strict regulatory and legal compliance *without revealing* the underlying user identity or sensitive credentials by leveraging Zero-Knowledge (ZK) circuits.

---

## 🚀 Live Demonstration
The dApp is successfully built and deployed on Vercel:
👉 **[PrivaCompliance Live dApp](https://privacompliance-dapp-ksm4.vercel.app)**

---

## 🌗 Level 2 - Waxing Crescent Specifications

### 🛡️ Privacy Claim & Observable Behavior
Our dApp proves strict regulatory and legal compliance *without revealing* the underlying user identity or sensitive credentials:
* **Proven (What the world sees):** A verified state transition on the Midnight Preprod testnet (`isValidated = true`).
* **Concealed (What remains hidden):** The private execution parameters analyzed locally inside the ZK circuit (`witness.assertEligible`).

### 📝 Verification Checklist
* **Wallet Integration:** Full Lace Wallet Connect/Disconnect cycle implemented on the Preprod network.
* **Circuit Execution:** Verified zero-knowledge pipeline handling secure state modification logs dynamically from the frontend.

---

## 🛠️ Tech Stack & Configuration

The application is built with a modern, high-performance web stack tailored for zero-knowledge dApp interactions:

* **Framework:** React 18 + Vite 5 (Optimized ESM Build)
* **Styling:** Tailwind CSS v3 (PostCSS Architecture)
* **Language:** TypeScript
* **Blockchain Network:** Midnight Network (Preprod Testnet)
* **Hosting:** Vercel Production Pipeline

---

## 💻 Local Development

Follow these steps to spin up the project locally in your development environment:

1. **Clone the repository:**
   ```bash
   git clone [https://github.com/deniz-1998/privacompliance-dapp.git](https://github.com/deniz-1998/privacompliance-dapp.git)
   cd privacompliance-dapp
