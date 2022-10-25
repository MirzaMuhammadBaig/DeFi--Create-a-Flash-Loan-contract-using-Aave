# Creating a Flash Loan using Aave

### In this project

- Create and deploy a Flash loan smart contract
- Receive funding with the liquidity protocol called Aave 
- Transact with our deployed contract to execute a Flash loan


##### What is flash loan:
```
In traditional finance, borrowers many times are required to offer collateral to receive a loan. This collateral is usually in the form of an asset like a car or home. Banks use this collateral as security to cover losses if the borrower fails to pay. 

In the world of Decentralized Finance(DeFi), a borrower can receive a loan without the need for providing collateral by using flash loans.

In a flash loan, lenders can both provide a loan to a borrower and be paid back for that loan in a single transaction. This is possible because of the time that a transaction is started and when it is finally committed to a block on the blockchain. 
```

### Requirements

- Remix IDE 

- Metamask Wallet 

### Setup Of Smart-Contract

- Open remix then create a folder and in that folder you will paste all contracts same as mentioned in my github.


### About contracts

#### Flashloan.sol 

- This is the flash loan smart contract. It contains an ExecuteOperation function that the contract 
will call to complete the operations that will use the funds from the loan. 

#### FlashLoanRecieverBase.sol / IFlashLoanReciever.sol   

- This is what allows the contract to receive funds for the flash loan

#### ILendingPool.sol  / ILendingPoolAddressProvider.sol  

- Points to the Aave lending pools that will fund the flash loan

#### Withdrawable.sol 

- Allows for other contracts to withdraw funds from this contract in the case of incorrect or stuck funds

- Note: Do inject web3

```
Note: Make sure funds should be in your wallets 
```

```
Note: Use kovan address
```