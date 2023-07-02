# ETH+AVAX PROOF:-Intermediate EVM MODULE 3 PROJECT

# CREATE AND MINT TOKEN

For this project, you will write a smart contract to create your own token on a local HardHat network. Once you have your contract, you should be able to use remix to interact with it. From remix, the contract owner should be able to mint tokens to a provided address. Any user should be able to burn and transfer tokens.



# ABHI Token (MUK) README



## Introduction

Welcome to the ABHI Token (MUK) repository! This repository contains the Solidity smart contract code for the MUK token, an ERC-20 compatible token designed for various purposes. MUK tokens can be used for transactions, rewards, and other activities within an ecosystem.

This README file provides an overview of the MUK token contract and includes instructions on how to deploy the contract to the local Hardhat test network using Remix Connect Localhost and how to interact with it using Remix with Hardhat provider.

## Contract Details

The `Token.sol` file contains the source code for the MUK token contract. Here are the key details of the contract:

- Token Name: ABHI Token
- Token Symbol: MUK
- Decimals: 18
- Total Supply: 0 (initially)

The contract includes standard ERC-20 functions such as `balanceOf` and `transfer`. It also includes functionalities for minting and burning tokens, accessible only by the contract owner.

The contract owner has special privileges and is the only address allowed to mint new tokens. Other addresses can interact with the contract by transferring tokens and burning their own tokens.

Contract Name: Token

State Variables:

# name: A public string variable representing the name of the token ("ABHI Token").

# symbol: A public string variable representing the symbol of the token ("MUK").

# decimals: A public uint8 variable representing the number of decimal places for token balance representation (18 decimals).

# totalSupply: A public uint256 variable representing the total supply of tokens.

# balances: A private mapping that maps addresses to their corresponding token balances.

# allowances: A private mapping that maps addresses to allowances granted by token holders to spend tokens on their behalf.

# owner: A public address variable representing the owner of the token contract.

# Events:

# Transfer: An event emitted when tokens are transferred from one address to another.

Mint: An event emitted when new tokens are minted and added to an address.
Burn: An event emitted when tokens are burned (removed from circulation) from an address.
Modifiers:

onlyOwner: A modifier that restricts the execution of a function to the contract owner only.
Constructor:

The constructor is executed once during contract deployment. It initializes the state variables:
name is set to "ABHI Token".
symbol is set to "MUK".
decimals is set to 18.
totalSupply is set to 0.
owner is set to the address of the contract deployer (msg.sender).
Functions:

balanceOf: A public view function that takes an address as an argument and returns the token balance of that address.

transfer: A public function to transfer tokens from the caller's address to a recipient address.

mint: A public function to mint new tokens and add them to a specified address. Only the contract owner can call this function.

burn: A public function to burn (remove from circulation) a specified amount of tokens from the caller's address.

## Deployment on Local Hardhat Test Network using Remix Connect Localhost

To deploy the MUK token contract to the local Hardhat test network using Remix Connect Localhost, follow these steps:

1. Clone the repository and install its dependencies:

```sh

cd INTERACTING-AND-DEPLOYING-ON-LOCAL-NETWORK
npm install
```

2. Install the `@remix-project/remixd` dependency to connect Remix IDE:

```sh
npm install -g @remix-project/remixd
```

3. Run the following command in the terminal to connect Remix IDE to the Hardhat local host:

```sh
remixd -s ./ --remix-ide https://remix.ethereum.org
```

4. Open a new terminal and start Hardhat's testing network:

```sh
npx hardhat node
```

5. Open the [Remix](https://remix.ethereum.org/) online IDE in your browser.

6. In the file explorer in the workspace, select "localhost" to connect to the local Hardhat network.

7. Rewrite the `Token.sol` file in the contracts directory with your RUK token contract code.

8. Compile the contract in the Remix IDE.

9. In the deploy section of Remix, select the environment as "Dev-Hardhat Provider".

10. Deploy your contract on the local Hardhat network using the deploy button in Remix.

11. Confirm the deployment transaction in Remix.

12. Wait for the deployment transaction to be confirmed on the local Hardhat network.

13. Once the contract is deployed, you will see the contract address in the Remix console. Make note of this address for future interactions.

## Interacting with the Contract using Remix with Hardhat Provider

After deploying the MUK token contract to the local Hardhat test network, you can interact with the contract using Remix with Hardhat provider. Here are the steps to get started:

1. Open the [Remix](https://remix.ethereum.org/) online IDE in your browser.

2. In the "File Explorer" section, locate the `Token.sol` file and open it.

3. In the "Deployed Contracts" section, click on the contract named `Token`.

4. In the "At Address" input field, enter the contract address obtained during deployment.

5. Click the "At Address" button to load the contract instance.

6. You can now interact with the RUK token contract through the provided functions.

   - Use the `balanceOf` function to check the token balance of a specific address.
   - Use the `transfer` function to send MUK tokens from your address to another address.
   - Use the `mint` function (accessible only to the contract owner) to mint

 new RUK tokens.
   - Use the `burn` function to burn a specific amount of your RUK tokens.

7. Set the required parameters for each function and click the corresponding button to execute the transaction.

8. Confirm the transaction details and sign the transaction in Remix.

9. Wait for the transaction to be confirmed on the local Hardhat network.

10. You can view the transaction status and emitted events in the Remix console.

## Authors

ABHISEK BAG
https://www.linkedin.com/in/abhisek-bag-09865421b/
21BCS9333@cuchd.in

## License

The ABHI Token (MUK) contract is licensed under the MIT License. See the [`LICENSE`](LICENSE) file for more information.
The comment // SPDX-License-Identifier: MIT is a special comment that specifies the license under which the code is released. It uses the SPDX-License-Identifier format, which is a standard way of indicating the license for open-source software.

