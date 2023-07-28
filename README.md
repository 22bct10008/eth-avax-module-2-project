# Bank App Metacrafters

Welcome to the Bank App Metacrafters project! This application combines a Solidity smart contract called "BankApp" with a React frontend, allowing users to experience basic banking functionalities on the Ethereum blockchain.

## Overview

The Bank App Metacrafters project aims to provide users with a secure and user-friendly way to manage their finances using the Ethereum blockchain. The smart contract, "BankApp," serves as the backbone of the application, offering features like account creation, deposit, withdrawal, and balance inquiry. To interact with the smart contract seamlessly, the project incorporates a React frontend.

## Getting Started

Follow these steps to run the project locally:

1. Clone the project repository from GitHub: [Bank App Metacrafters Repo](https://github.com/gautham2k3/ETH-AVAX_Mod-2_Project/).
2. Navigate to the project directory on your local machine.

## Running the Application

Before you start, ensure you have [MetaMask](https://metamask.io/) installed in your web browser. Then, execute the following:

```bash
npm install
npm start
```

Click the "Connect Wallet" button to establish a secure connection with your MetaMask wallet and the application.

## Troubleshooting

If you encounter any issues while running the application, consider the following steps:

1. Verify that MetaMask is correctly installed and set up in your web browser.
2. Double-check that you are connected to the correct Ethereum network (localhost).
3. Ensure your MetaMask wallet has sufficient funds to perform transactions on the Ethereum blockchain.

Open [http://localhost:3000](http://localhost:3000) to view the application in your browser. The page will automatically reload if you make any changes, and you can check the console for potential lint errors.

## Functionality

The Bank App Metacrafters project offers the following functions:

### `connectWalletHandler`

This function establishes a secure connection between the application and your MetaMask wallet. When you click the "Connect Wallet" button, it enables you to interact with the application using your Ethereum address.

### `accountChangedHandler`

The `accountChangedHandler` function triggers when there is a change in the connected MetaMask account. It updates the default Ethereum address in the frontend, ensuring smooth communication with the smart contract using the new account.

### `chainChangedHandler`

When there is a change in the selected blockchain network within your MetaMask wallet, the `chainChangedHandler` function ensures the application adapts to the new network settings and continues to function seamlessly.

### `updateEthers`

The `updateEthers` function plays a vital role in facilitating communication between the application, the deployed smart contract, and the MetaMask wallet's provider network. By utilizing the Web3Provider and Signer from ethers.js library, this function establishes the necessary connections for smooth data exchange between the frontend and the smart contract.

### `createAccount`

With the `createAccount` function, users can easily create a bank account within the Bank Dapp. By triggering this function, a new account will be registered in the bank, enabling secure deposit, withdrawal, and fund transfer.

### `checkAccountExists`

The `checkAccountExists` function allows users to verify if their account is listed within the Bank Dapp. By invoking this function, users can confirm the existence of their account before proceeding with transactions.

### `accountBalance`

Using the `accountBalance` function, users can check the balance of their bank account. Upon calling this function, the application communicates with the smart contract to fetch and display the current balance associated with the user's account.

### `depositBalance`

The `depositBalance` function facilitates the process of depositing funds from the user's MetaMask wallet into their bank account. By specifying the deposit amount, users can initiate the transaction to increase their account balance.

### `withdrawBalance`

With the `withdrawBalance` function, users can easily withdraw funds from their bank account to their MetaMask wallet address. Users specify the withdrawal amount, and the application processes the request, deducting the amount from the account balance and transferring it to the designated wallet address.

## Authors

- Mohith 
- Email: 22bct10008@cuchd.in

## License

This project is licensed under the MIT License.
