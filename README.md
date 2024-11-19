
# Foundry Fundamentals - Section 2: Fund Me

This repository contains the project developed during **Section 2** of the [Foundry Fundamentals](https://updraft.cyfrin.io/courses/foundry) course by Cyfrin. In this section, we implemented the "Fund Me" smart contract, allowing users to contribute funds to a specific project while using Chainlink oracles for currency conversion.

## Section Objectives

- **Implement the "Fund Me" Contract**: Create a contract that allows users to send funds and tracks contributors and their contributions.
- **Integrate Chainlink Oracles**: Use oracles to fetch the current ETH to USD exchange rate to ensure accurate contributions.
- **Develop Testing and Deployment Scripts**: Write tests to verify the contract's functionality and scripts for deployment to test networks.

## Features Implemented

- **Contribution Tracking**: The contract stores the address of each contributor and the amount contributed.
- **Currency Conversion**: Integration with Chainlink oracles to fetch real-time ETH/USD conversion rates.
- **Minimum Contribution Threshold**: Ensures each contribution meets a minimum value in USD before being accepted.
- **Withdrawal Functionality**: Allows the contract owner to withdraw the accumulated funds.

## Prerequisites

- Basic knowledge of Solidity and smart contracts.
- Development environment set up with Foundry and associated tools.

## How to Run the Project

1. Clone this repository:
   ```bash
   git clone https://github.com/Khetreiqcer/Sldt.git
   ```
2. Navigate to the project directory:
   ```bash
   cd fund-me
   ```
3. Install the Foundry toolchain if not already installed:
   ```bash
   curl -L https://foundry.paradigm.xyz | bash
   foundryup
   ```
4. Install dependencies:
   ```bash
   forge install
   ```
5. Compile the smart contract:
   ```bash
   forge build
   ```
6. Run tests:
   ```bash
   forge test
   ```
7. Deploy the contract to a local Anvil instance:
   ```bash
   anvil
   forge script script/DeployFundMe.s.sol --fork-url http://127.0.0.1:8545 --broadcast
   ```
8. Interact with the deployed contract (optional):
   Use the Forge console or scripts to test functionality like funding and withdrawing.

## References

- [Foundry Fundamentals Course - Cyfrin](https://updraft.cyfrin.io/courses/foundry)
- [Course GitHub Repository](https://github.com/Cyfrin/foundry-full-course-cu)

## License

This project is licensed under the MIT License. See the LICENSE file for more details.
