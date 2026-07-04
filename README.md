# PrivaCompliance dApp (Midnight Level 1)

This repository contains the smart contract implementation and automated toolchain verification for the **PrivaCompliance** decentralized application, built on the **Midnight Network**.

The project fulfills all the core technical requirements for **Level 1 qualification**, demonstrating a fully compatible development environment, zero-knowledge smart contract architecture, and continuous integration verification.

---

## 🛠️ Project Structure

*   `contract.compact`: The core Midnight Zero-Knowledge smart contract written in the Compact language. It defines the state structures (`Ledger`) and private proof logic (`Witness`) to verify regulatory compliance without exposing sensitive user data.
*   `.github/workflows/main.yml`: Automated GitHub Actions workflow acting as our cloud toolchain. It spins up the official Midnight compiler environment inside Docker to dynamically verify code compilation on every update.

---

## 🔐 Smart Contract Logic (`contract.compact`)

The contract implements a private compliance gateway that securely checks user eligibility off-chain and updates the public state anonymously:

1.  **Ledger State (`Ledger`)**: Publicly tracks whether a user has been validated (`isValidated`), ensuring transparent compliance checks for third-party dApps.
2.  **Private Witnesses (`Witness`)**: Evaluates secret constraints (`assertEligible`) locally on the user's machine, keeping personal identification credentials completely private.
3.  **ZK Circuits (`verifyUser`)**: Executes the zero-knowledge logic. It asserts the user's eligibility criteria and signs off on the state transition without publishing any underlying private records to the ledger.

---

## 🚀 Toolchain & Verification

To guarantee architectural compliance and eliminate environment-specific discrepancies, the project utilizes the official **Midnight Toolchain** via isolated execution:

*   **Runtime Environment**: Node.js v22
*   **Compilation Engine**: Official `midnightnetwork/compact` Docker container.
*   **Verification Command**: `compact compile contract.compact`

### CI/CD Build Status
Every code modification triggers our automated cloud compiler. The successful **Green Checkmark (`✓`)** under the GitHub Actions tab formally validates that the environment is sound and the codebase compiles perfectly.


---

## 🌒 Level 2 - Waxing Crescent Specifications

### 🔐 Privacy Claim & Observable Behavior
Our dApp proves strict regulatory and legal compliance *without revealing* the underlying user identity or sensitive credentials:
* **Proven (What the world sees)**: A verified state transition on the Midnight Preprod testnet (`isValidated = true`).
* **Concealed (What remains hidden)**: The private execution parameters analyzed locally inside the ZK circuit (`witness.assertEligible`).

### 🚀 Verification Checklist
* **Wallet integration**: Full Lace Wallet Connect/Disconnect cycle implemented on the Preprod network.
* **Circuit Execution**: Verified zero-knowledge pipeline handling secure state modification logs dynamically from the frontend.
