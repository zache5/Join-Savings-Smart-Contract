# Join-Savings-Smart-Contract\
This is a smart contract written in Solidity that creates a joint savings account, where two users can control the account by transferring and withdrawing funds. The contract has been written with a few requirements from a financial institution in mind.

## Features
The smart contract features the following functions:

1 == withdraw(uint amount, address payable recipient): Allows users to withdraw funds from the account. The function takes in two arguments, the amount to withdraw and the recipient address. The function checks if the recipient is equal to either accountOne or accountTwo, and if there are sufficient funds in the contract, and then transfers the amount to the recipient. The function also sets lastToWithdraw to the current recipient, lastWithdrawAmount to the amount that was withdrawn, and updates the contractBalance.

2 == deposit(): Allows users to deposit funds to the account. The function receives Ether with the payable modifier and updates the contractBalance variable.

3 == setAccounts(address payable account1, address payable account2): Sets the addresses of the two account holders.

4 == fallback(): A fallback function that stores any Ether sent to the contract address outside of the deposit function.

## Usage
To use the smart contract, you need to create and work within a local blockchain development environment using the JavaScript VM provided by the Remix IDE. You can deploy the JointSavings smart contract by compiling and deploying it using Remix IDE or any other Solidity development environment. Once deployed, you can interact with the contract by calling its functions, including withdraw(), deposit(), and setAccounts(). The contract also allows you to send Ether to its address to store it in the account.

## Requirements
This smart contract has been written in Solidity version 0.5.0. You will need to have a blockchain development environment, such as Remix IDE, to compile and deploy the contract. You will also need some knowledge of Solidity programming to modify and work with the contract.

## Contributors
I am the main contributor for this code!
