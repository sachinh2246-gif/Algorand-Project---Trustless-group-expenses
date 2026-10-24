[README.md](https://github.com/user-attachments/files/33911184/README.md)
# Algorand-Project---Trustless-group-expenses
A decentralized group expense-splitting dApp on Algorand: track shared expenses on-chain and settle balances instantly in ALGO
# AlgoSplit: Trustless Group Expense Splitting on Algorand

AlgoSplit is a decentralized application (dApp) built on the [Algorand](https://algorand.co) blockchain that lets groups pool money for shared expenses (trips, flatmates, events) and settle up automatically, with no middleman and with every payment recorded transparently on-chain.

> **Status:** Early development. This repository is being built as part of an Algorand development course project.

## Problem

Splitting costs among friends or flatmates usually means spreadsheets, chasing people for payments, and trusting one person to hold the money. There is no shared, tamper-proof record of who paid what and who still owes.

## Solution

AlgoSplit uses an Algorand smart contract to:

- Create a shared expense group with a defined list of members
- Record expenses on-chain so everyone sees the same ledger
- Calculate each member's balance automatically
- Settle balances with low-fee, near-instant ALGO transactions

## Planned Features

- [ ] Create an expense group and add members by Algorand address
- [ ] Log an expense (amount, payer, description)
- [ ] Equal-split calculation per member
- [ ] On-chain balance tracking (who owes whom)
- [ ] One-click settlement in ALGO
- [ ] Simple web front end with wallet connection (Pera / Defly)
- [ ] Deployment to Algorand TestNet

## Tech Stack

| Layer | Tool |
|-------|------|
| Blockchain | Algorand (TestNet for development) |
| Smart contracts | Algorand Python (PuyaPy) via AlgoKit |
| Tooling | [AlgoKit](https://github.com/algorandfoundation/algokit-cli) |
| Front end | React + TypeScript (planned) |
| Wallet | Pera Wallet / Defly (planned) |

## Getting Started

### Prerequisites

- [Git](https://git-scm.com/)
- [Python 3.12+](https://www.python.org/)
- [Docker](https://www.docker.com/) (for the AlgoKit local network)
- [AlgoKit CLI](https://github.com/algorandfoundation/algokit-cli)

### Setup

```bash
# Clone the repository
git clone https://github.com/<your-username>/algosplit.git
cd algosplit

# Install AlgoKit (if not already installed)
pipx install algokit

# Bootstrap project dependencies
algokit project bootstrap all
```

### Run a local Algorand network

```bash
algokit localnet start
```

> Setup steps will be refined as the project structure is finalized.

## Project Structure

```
algosplit/
├── README.md          # Project overview (this file)
├── contracts/         # Algorand smart contracts (planned)
├── frontend/          # Web interface (planned)
└── docs/              # Design notes and diagrams (planned)
```

## Roadmap

1. **Week 1:** Repository setup, project scope, README
2. **Next:** Smart contract for group creation and expense logging
3. **Then:** Settlement logic and tests
4. **Finally:** Front end and TestNet deployment

## Learning Goals

- Understand Algorand accounts, transactions, and smart contract (application) basics
- Practice writing and testing contracts with AlgoKit
- Build and maintain a real project in a single, consistent repository

## Contributing

This is a personal course project, but feedback and suggestions are welcome. Feel free to open an issue.

## License

This project is licensed under the MIT License.

## Author

**<Your Name>**
GitHub: [@your-username](https://github.com/your-username)
