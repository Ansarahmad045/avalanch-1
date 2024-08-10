# Solidity ERC20 & Vault Contracts

This Solidity project consists of two smart contracts: an ERC20 token implementation and a Vault contract. The ERC20 contract provides a basic implementation of the ERC20 standard, while the Vault contract allows users to deposit and withdraw ERC20 tokens in exchange for shares representing their ownership in the Vault.

## Description

The project includes the following components:

1. **ERC20 Token Contract**: Implements a simple ERC20 token with minting and burning functionalities. This contract allows users to transfer tokens, approve allowances, and perform transfers on behalf of other users.

2. **Vault Contract**: The Vault contract allows users to deposit ERC20 tokens and receive shares in return. These shares represent a portion of the total tokens held in the Vault. Users can later withdraw their tokens by burning their shares. The Vault contract calculates the number of shares to mint or burn based on the current total supply and the balance of tokens in the Vault.

## Getting Started

### Prerequisites

To interact with these contracts, you'll need:

- A Solidity development environment like [Remix](https://remix.ethereum.org/).
- Basic knowledge of Solidity and smart contracts.

### Executing the Program

To run these contracts, follow the steps below:

1. **Open Remix**: Go to [Remix](https://remix.ethereum.org/) and create a new file. You can name it `ERC20Vault.sol`.

2. **Copy the Code**: Paste the provided Solidity code into the file.

3. **Compile the Contracts**:
   - In the Remix IDE, click on the "Solidity Compiler" tab.
   - Ensure the compiler version is set to `^0.8.17`.
   - Click on the "Compile" button to compile the contracts.

4. **Deploy the ERC20 Contract**:
   - Go to the "Deploy & Run Transactions" tab.
   - Select the `ERC20` contract from the dropdown menu.
   - Click "Deploy" to deploy the ERC20 token contract.
   - Note the deployed contract address; you'll need it for the Vault contract.

5. **Deploy the Vault Contract**:
   - In the "Deploy & Run Transactions" tab, select the `Vault` contract.
   - Enter the ERC20 contract address as the `_token` parameter in the deployment field.
   - Click "Deploy" to deploy the Vault contract.

6. **Interact with the Contracts**:
   - **Minting Tokens**: Use the `mint` function of the ERC20 contract to mint tokens to your address.
   - **Approving Allowance**: Use the `approve` function of the ERC20 contract to allow the Vault contract to spend tokens on your behalf.
   - **Depositing Tokens**: Call the `deposit` function of the Vault contract to deposit tokens in exchange for shares.
   - **Withdrawing Tokens**: Use the `withdraw` function of the Vault contract to redeem your shares for tokens.

## License
This project is licensed under the MIT License - see the `LICENSE.md` file for details.
