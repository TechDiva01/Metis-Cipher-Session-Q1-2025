# Solidity

Solidity is an object-oriented-that it organizes and structures code around objects and their interactions. A high-level language for implementing smart contracts. 
Smart contracts are programs that govern the behavior of accounts within the Ethereum state.

Solidity is designed to write smart contract on the Ethereum Virtual Machine (EVM). It is influenced by C++, Python, and JavaScript. With Solidity, you can create contracts for use such as voting, crowdfunding, blind auctions,  and multi-signature wallets.

Note: blind auction is a situation whereby bidders of a property or art submit their bid prices without knowing the bid of others elctronically, The highest bidder gets the property
Other Blockcahin that are EVM compactible uses solidity such as ethereum, base,etc.
Smart contract written in solidity language purposes starts with

// SPDX-License-Identifier: GPL-3.0
pragma solidity >=0.4.16 <0.9.0;

The // SPDX-License-Identifier: GPL-3.0 line tells everyone that the code is licensed under the GNU General Public v3.0 License. This means anyone can use, copy, modify, and distribute the code as long as they include the original license. This helps avoid legal problems because everyone knows their rights and obligations when using the code.
However,If you do not want to specify a license or if the source code is not open-source, please use the special value UNLICENSED for no usage allowed, and UNLICENSE for grant usage to everyone.

