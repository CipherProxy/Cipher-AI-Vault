# 🔐 Cipher AI Vault 🚀
## Version 2.2.2

Welcome to the **Cipher AI Vault** demo repository—a fully in-browser, in-memory showcase of the Internet Computer's (IC) cutting-edge capabilities. This demo seamlessly integrates `ic-auth` for secure authentication, asset storage, an in-memory VectorDB with LLM, and cycles-distro top-up functionality. With zero server-side components, Cipher AI Vault highlights the power and versatility of the Internet Computer's decentralized architecture, demonstrating its potential to run sophisticated applications entirely within a sandboxed environment.

*The demo is a proof of concept and is not intended for production use. This project is part of a [Developer Grant from the DFINITY Foundation](https://dfinity.org/grants).*

*The demo canister is currently running on the following canister url: https://qehbq-rqaaa-aaaan-ql2iq-cai.icp0.io/*

### ⚙️ Prerequisites

**WebGPU:** This project runs best in a [WebGPU](https://developer.mozilla.org/en-US/docs/Web/API/WebGPU_API) enabled browser. We suggest [Chrome Canary](https://www.google.com/chrome/canary/).

You will need to have DFX and NodeJS set up to use this repo. This project uses the Azle development kit from Demergent Labs. If you need help getting setup, check out these links:

**DFX Setup:** https://internetcomputer.org/docs/current/developer-docs/getting-started/install
<br>
**NodeJS Setup:** https://docs.npmjs.com/downloading-and-installing-node-js-and-npm
<br>
**Azle Docs:** https://github.com/demergent-labs/azle

You will need one of the following wallets to  run the demo:
- [Plug Wallet](https://plugwallet.ooo/)
- [Stoic Wallet](https://www.stoicwallet.com/)
- [NFID Wallet](https://nfid.one/)
- [Internet Identity](https://identity.raw.ic0.app/)

### 🛠️ Setup Instructions

#### Clone The Repo:
```bash
git clone https://github.com/supaIC/Cipher-AI-Vault.git
cd ic-storage-module
```

#### Project Setup:

As long as you have already installed and configured Node and DFX, the easy setup command should take care of everything for you:

```
npm run setup
```

If for some reason the automatic command doesn't work, you can use the manual commands:

```
npm install && npm audit fix
dfx start --clean --background
dfx canister create --all
dfx build
dfx deploy
dfx stop
```
*Note: You may be prompted to enter your DFX identity password during setup.*

**👨‍💻 Developer Mode:**
```bash
npm run dev
```

or

```bash
cd frontend
dfx start --background --clean
dfx deploy
dfx stop
```

This Project has two main canisters, each provided with their own dfx.json file:
- The Frontend Canister: `frontend`
- The Cycles Distro Canister: `distro-canister`

### Future Plans:

- List of planned features and improvements.