# Sample Hardhat Project

This project demonstrates a basic Hardhat use case. It comes with a sample contract, a test for that contract, and a Hardhat Ignition module that deploys that contract.

Try running some of the following tasks:

```shell
npx hardhat help
npx hardhat test
REPORT_GAS=true npx hardhat test
npx hardhat node
npx hardhat ignition deploy ./ignition/modules/Lock.js
```

# Transactions Contract

This is a simple Ethereum smart contract written in Solidity that allows for the tracking of transactions on the blockchain.

## Contract Details

The `Transactions` contract keeps track of transactions, each represented by a `TransferStruct` which includes the sender, receiver, amount, message, timestamp, and a keyword.

### Functions

- `addToBlockchain(address payable receiver, uint amount, string memory message, string memory keyword)`: This function allows a user to add a transaction to the blockchain. It emits a `Transfer` event and increments the `transactionCount`.

- `getAllTransactions()`: This function returns all transactions that have been added to the blockchain.

- `getTransactionCount()`: This function returns the total number of transactions that have been added to the blockchain.

## Setup

To compile the contract, use the Solidity compiler with a version of 0.8.0 or higher.

## Usage

To interact with the contract, you can use a web3 provider like Metamask and a frontend JavaScript library like ethers.js or web3.js.

## License

This project is unlicensed.
