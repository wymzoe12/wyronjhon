# wyronjhon
# Creating a Token

Simple overview of use/purpose.
Making a token involves  knowledge and work than making a cryptocurrency coin. Typically, creating a coin requires a group of programmers and industry professionals. While the creation of a token still requires technical expertise, other blockchains like Ethereum, BNB Smart Chain (BSC), Solana, and Polygon make it feasible to do it quickly. 

## Description

An in-depth paragraph about your project and overview of use.
The term "token" refers to an asset that makes use of an existing blockchain and is not a standalone blockchain. A token that utilizes the Ethereum blockchain is considered to be part of the Ethereum ecosystem. However, cryptocurrency currencies usually need their own blockchain; for instance, Ether is the cryptocurrency that runs the Ethereum blockchain. On a blockchain, there can often be a plethora of unique tokens but only one cryptocurrency.

## Getting Started

### Installing

* How/where to download your program
* Any modifications needed to be made to files/folders

### Executing program

* How to run the program
* Step-by-step bullets
To run this program, you can use Remix, an online Solidity IDE. To get started, go to the Remix website at https://remix.ethereum.org/.
```
code blocks for commands
// SPDX-License-Identifier: MIT
pragma solidity 0.8.18;
contract MyToken {
    // public variables here
string public tokenName = "WYRON";
string public tokenAbbrv = "WY";
uint public totalSupply = 0;
    // mapping variable here
mapping(address => uint) public balances;
    // mint function
function mint (address token_address, uint token_value) public{
    totalSupply += token_value;
    balances[token_address] += token_value;
}
    // burn function
function burn (address token_address, uint token_value) public{
    if (balances[token_address] >= token_value){
        totalSupply -= token_value;
        balances[token_address] -= token_value;
        }
    }
}
```
To make your code ready, first, go to the "Solidity Compiler" section on the left side of the screen. After that, click on the "Compile [file_name].sol" button. Once the code is all set, you can put it into action by going to the "Deploy & Run Transactions" area on the left. There, you'll find information about the token name, token abbreviation, and the total supply you've selected.

```
Copy the default address and paste it in the "mint" section. Choose an amount to mint and click "transact." Then, check the total supply.

Copy the address and paste it in the "balances" section.

Now, try burning tokens using the same process. Afterward, check the total supply and balances to see if they've decreased by the amount you chose.

Lastly, test whether you can't burn more tokens than you have. If everything is working correctly, the total supply and balances should remain unchanged.

Thank youu

## Authors

Wyron Mediavillo
202010658@fit.edu.ph


