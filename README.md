# Wave Portal

Hardhat sample project for an Ethereum smart contract that records waves and rewards users probabilistically.

## About

This repo is a Solidity + Hardhat tutorial-style application. The contract stores wave messages, rate-limits repeat submissions, and conditionally sends a small prize from the contract balance. It works well as a compact portfolio example for an on-chain state machine and deployment workflow.

## Key Features

- Solidity smart contract with event emission
- Hardhat deployment and execution scripts
- Test scaffold and local contract workflow
- Environment-driven network configuration

## Architecture

- `contracts/WavePortal.sol` holds the contract logic
- `scripts/deploy.js` deploys the contract
- `scripts/run.js` exercises the contract from a script
- `hardhat.config.js` configures the network and wallet credentials

## Tech Stack

- Solidity
- Hardhat
- ethers.js
- mocha/chai test tooling

## Prerequisites

- Node.js
- A configured Ethereum RPC endpoint
- A funded deployer wallet for live networks

## Installation

```bash
npm install
```

## Configuration

- `STAGING_ALCHEMY_KEY`
- `PRIVATE_KEY`

## How to Run

```bash
npx hardhat compile
npx hardhat test
npx hardhat run scripts/run.js
npx hardhat run scripts/deploy.js --network rinkeby
```

## Example Usage

- Compile the contract
- Run the script that deploys and waves twice
- Print configured accounts with the Hardhat task

## Project Structure

- `contracts/` - Solidity source
- `scripts/` - deployment and demo scripts
- `test/` - contract tests
- `artifacts/` and `cache/` - generated Hardhat output

## Current Status

Tutorial-style demo that is functional for local Hardhat workflows.

## Limitations

- No explicit top-level license file in the workspace snapshot
- Generated build output is now removed from the workspace snapshot

## License

No explicit license file was found at the repository root.
