# RIDAM Token (RUK) README

## Introduction

Welcome to the RIDAM Token (RUK) repository! This repository contains the Solidity smart contract code for the RUK token, an ERC-20 compatible token designed for various purposes. RUK tokens can be used for transactions, rewards, and other activities within an ecosystem.

This README file provides an overview of the RUK token contract and includes instructions on how to deploy the contract to the local Hardhat test network using Remix Connect Localhost and how to interact with it using Remix with Hardhat provider.

## Contract Details

The `Token.sol` file contains the source code for the RUK token contract. Here are the key details of the contract:

- Token Name: RIDAM Token
- Token Symbol: RUK
- Decimals: 18
- Total Supply: 0 (initially)

The contract includes standard ERC-20 functions such as `balanceOf` and `transfer`. It also includes functionalities for minting and burning tokens, accessible only by the contract owner.

The contract owner has special privileges and is the only address allowed to mint new tokens. Other addresses can interact with the contract by transferring tokens and burning their own tokens.

## Deployment on Local Hardhat Test Network using Remix Connect Localhost

To deploy the RUK token contract to the local Hardhat test network using Remix Connect Localhost, follow these steps:

1. Clone the repository and install its dependencies:

```sh
git clone https://github.com/RIDAMSINHA/INTERACTING-AND-DEPLOYING-ON-LOCAL-NETWORK.git
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

After deploying the RUK token contract to the local Hardhat test network, you can interact with the contract using Remix with Hardhat provider. Here are the steps to get started:

1. Open the [Remix](https://remix.ethereum.org/) online IDE in your browser.

2. In the "File Explorer" section, locate the `Token.sol` file and open it.

3. In the "Deployed Contracts" section, click on the contract named `Token`.

4. In the "At Address" input field, enter the contract address obtained during deployment.

5. Click the "At Address" button to load the contract instance.

6. You can now interact with the RUK token contract through the provided functions.

   - Use the `balanceOf` function to check the token balance of a specific address.
   - Use the `transfer` function to send RUK tokens from your address to another address.
   - Use the `mint` function (accessible only to the contract owner) to mint

 new RUK tokens.
   - Use the `burn` function to burn a specific amount of your RUK tokens.

7. Set the required parameters for each function and click the corresponding button to execute the transaction.

8. Confirm the transaction details and sign the transaction in Remix.

9. Wait for the transaction to be confirmed on the local Hardhat network.

10. You can view the transaction status and emitted events in the Remix console.

## Authors

RIDAM ADITYA SINHA

https://www.linkedin.com/in/ridam-sinha-188133210/

ridamsinha20@gmail.com

## License

The RIDAM Token (RUK) contract is licensed under the MIT License. See the [`LICENSE`](LICENSE) file for more information.

## Disclaimer

Please note that this contract and the associated README file are provided for informational purposes only. Deploying and interacting with smart contracts involves risks, and it is your responsibility to review and understand the code before proceeding. Make sure to exercise caution and perform appropriate testing before deploying any smart contract on a live network.
