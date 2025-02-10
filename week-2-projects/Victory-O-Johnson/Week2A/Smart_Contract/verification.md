# Smart Contract Verification
After contract deploy to a live nertwork, the next this is to verify its source code, ie making
 the source code public so that anyone can compile it nad comapre the byte code generated to 
 the code deployed on chain

Smart contract verification is a process that confirms that a smart contract's source code 
matches the bytecode on the blockchain. This process helps to identify vulnerabilities, ensure 
the contract behaves as intended, and build trust among users.
Smart contract when deployed creates an ABI(Application Binary Interface),and Bytecode. The 
bytecode which can only be read by the EVM must match with the contract source code written in 
solidyt language readble by humans, hence the users will not be able to comapre these codes and
this might lead to doubt of the smart contract or errors

## How to verify smart contract deployed by hardhat
Verification of smart contract can be done in two ways
- using etherscan -  https://etherscan.io/
- using hardhat

it is important to note that some Sepolia ether to the address that's going to be making the 
deployment is needed, an ether testnet can be gotten from a faucet, a service that distributes 
testing-ETH for free. Here are some for Sepolia:
- Alchemy Sepolia Faucet
- QuickNode Sepolia Faucet
- Ethereum Ecosystem Sepolia Faucet

So, first login to etherscan, create an account if you dont have one, then open API key tab, 
the click on the ADD button and give a name to the API key you are creating, after that you 
will see the newly created API key
Store the API key as the configuration variable ETHERSCAN_API_KEY:
On yout terminal bash:
$ npx hardhat vars set ETHERSCAN_API_KEY
✔ Enter value: ******************************** 

Open your Hardhat config code and set the Etherscan API key as the stored configuration variable
ETHERSCAN_API_KEY:

const { vars } = require("hardhat/config");

const ETHERSCAN_API_KEY = vars.get("ETHERSCAN_API_KEY");

module.exports = {
  // ...rest of the config...
  etherscan: {
    apiKey: ETHERSCAN_API_KEY,
  },
};

