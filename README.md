# Interact your smart-contract with frontend and connect it to MetaMask Wallet
In this section we will be connecting our smart contract with the frontend and a METAMASK wallet to increment and decrement Ethers.

## Description
It contains 3 Files namely app.js, index.html and bank.sol in the 3 folders.

## Getting Started
To run this program, you can use REMIX IDE by clicking the link https://remix.ethereum.org/#lang=en&optimize=false&runs=200&evmVersion=null&version=soljson-v0.8.26+commit.8a97fa7a.js

### Executing program for frontend and smart contract
1. copy and paste the index.html, bank.sol and app.js from the repository into vs code and remix
2. Remember index. html contains the frontend code.
3. Open two additional terminals in vscode

// SPDX-License-Identifier: MIT
pragma solidity ^0.8.0;

    contract Bank {
    int private bal;

    constructor() {
        bal = 1;
    }

    function getBalance() public view returns (int) {
        return bal;
    }

    function withdraw(int amt) public {
        bal = bal - amt;
    }

    function deposit(int amt) public {
        bal = bal + amt;
    }
    }



### wallet setup
To interact with the smart contract, we need to set up a network with the MetaMask wallet.
1. Click on the MetaMask extension and then click on the top right button -> settings.
2. Click on "Add a Network."
3. Click on "Add a Network Manually."
4. Give the Network name (whatever you want).


## License

This project is licensed under the MIT License - see the LICENSE.md file for details

## HELP
Compiler Mistakes: Solidity version 0.8.18 or higher is installed on  system.

## AUTHOR
Sanskriti Anand
SANSKRITIANAND@132

## LICENSE
This project is licensed under the METACRAFT License (https://github.com/Sanskriti132/front.sol/edit/main/README.md)

