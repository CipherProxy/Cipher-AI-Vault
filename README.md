# Cipher AI Vault

**Cipher AI Vault** is an Azle-based proof of concept designed with a strong emphasis on abstraction, seamlessly integrating in-memory VectorDB, in-memory LLM, secure asset storage, stable memory data storage, cycles-distro top-up, and ic-auth for authentication. This adaptability makes it well-suited for a wide range of AI-driven use cases. The project showcases the Internet Computer's potential for secure, sandboxed AI development, offering versatile tools for diverse applications.

*Please note that this demo is a proof of concept and is not intended for production use. This project was developed as part of a [**Developer Grant from the DFINITY Foundation**](https://dfinity.org/grants).*

## Demo Canisters and Repositories

The demo canister is live and can be accessed [**here**](https://qehbq-rqaaa-aaaan-ql2iq-cai.icp0.io/).

### Standalone Demo Canisters
- [**WebGPU LLM Demo**](https://f45ub-wiaaa-aaaap-ahskq-cai.icp0.io/)

### Grant Deliverables Repositories
- [**ic-auth**](https://github.com/supaIC/ic-auth)
- [**Cycles Distro**](https://github.com/supaIC/cycles-distro)
- [**Data Store Canister**](https://github.com/supaIC/data-store-canister)

## Core Features

- **Frontend Canister**: The main entry point for user interactions.
- **In-memory VectorDB**: Stores and manages embeddings for efficient retrieval.
- **In-memory LLM**: Processes natural language queries and interacts with the VectorDB.
- **Secure Asset Storage**: A dedicated module that securely stores assets.
- **Secure Data Store**: A dedicated canister for storing data in stable memory.
- **Cycles Distro Canister**: Manages cycles and top-ups.
- **ic-auth**: Handles authentication with various wallets such as Plug, Stoic, NFID, and Internet Identity.

## Prerequisites

**WebGPU:** For the best experience, use a [**WebGPU**](https://developer.mozilla.org/en-US/docs/Web/API/WebGPU_API) enabled browser. We recommend [**Chrome Canary**](https://www.google.com/chrome/canary/).

To use this repository, ensure that DFX and Node.js are installed. This project leverages the Azle development kit from Demergent Labs. For setup assistance, refer to the following resources:

- [**DFX Setup**](https://internetcomputer.org/docs/current/developer-docs/getting-started/install)
- [**Node.js Setup**](https://docs.npmjs.com/downloading-and-installing-node-js-and-npm)
- [**Azle Documentation**](https://github.com/demergent-labs/azle)

### Required Wallets

To run the demo, you will need one of the following wallets:

- [**Plug Wallet**](https://plugwallet.ooo/)
- [**Stoic Wallet**](https://www.stoicwallet.com/)
- [**NFID Wallet**](https://nfid.one/)
- [**Internet Identity**](https://identity.raw.ic0.app/)

## Quick Setup Instructions

### Clone The Repo:
```bash
git clone https://github.com/supaIC/Cipher-AI-Vault.git
cd Cipher-AI-Vault
```

### Quick Setup:

As long as you have already installed and configured Node and DFX, the easy setup command should take care of everything for you:

```
npm run setup
```
*Note: You may be prompted to enter your DFX identity password during setup.*

## Detailed Setup and Deployment Instructions

For detailed setup and deployment instructions, refer to the following README files within this repository:

- **Frontend Canister**: [**Setup and Deployment**](frontend/README.md)
- **Cycles Distro Canister**: [**Setup and Deployment**](distro-canister/README.md)
- **Data Store Canister**: [**Setup and Deployment**](data-store/README.md)

## Cipher AI Vault Roadmap

- [ ] Data Store backup canister
- [ ] Edit Data Store file entries
- [ ] Multiple in-memory LLM support
- [ ] Models stored in asset canisters
- [ ] Embeddings backed up in Stable Memory
- [ ] Generate a Data File from a document using in-memory LLM
- [ ] Generate images to be stored in the Image Store using in-memory Stable Diffusion

## License

This project is licensed under the MIT License - see the [**LICENSE**](LICENSE) file for details.