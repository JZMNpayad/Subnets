# Avalanche Subnets Solidity Contracts

This repository contains Solidity smart contracts for Avalanche Subnets. These contracts include an ERC20 token implementation (`ERC20.sol`), an interface for ERC20 (`IERC20.sol`), and a simple vault contract (`Vault.sol`).

## Contracts

### ERC20

`ERC20.sol` is an implementation of the ERC20 token standard. It includes functions for transferring tokens, approving spending, and minting/burning tokens.

### IERC20 Interface

`IERC20.sol` defines the interface for ERC20 tokens. It includes function signatures for total supply, balance of an account, transferring tokens, approving spending, and transferring tokens on behalf of another account.

### Vault

`Vault.sol` is a simple vault contract that allows users to deposit and withdraw ERC20 tokens. It uses a calculation to determine the number of shares to mint when depositing and the amount to withdraw based on the shares when withdrawing.

## Usage

1. Deploy the ERC20 token contract (`ERC20.sol`) to the Avalanche blockchain.

2. Deploy the Vault contract (`Vault.sol`) and pass the ERC20 token address as a constructor parameter.

3. Interact with the deployed contracts using the provided functions (e.g., depositing, withdrawing).

## Deployment

Make sure to deploy the contracts in the correct order: ERC20 first, then the Vault with the ERC20 contract address.
