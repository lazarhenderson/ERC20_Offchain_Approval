# ERC20 Offchain Token Approval

This ERC20 token has the ability to reduce gas spending when using the transferFrom function by approving a contract's spending and doing the token transferFrom in 1 transaction. Standard ERC20 tokens will need to do this in 2 separate transactions.

## Test the ERC20 Offchain Token Approval

First ensure you have Node.js installed, you can see if you have it installed by using the following command line prompt to see your Node.js version:

```shell
# Command Prompt (Windows)
node -- version

# Terminal (Mac)
node -v
```

If no Node.js version is shown then it's not installed. Click on the following link for Node.js's download page: [Node.js Download](https://nodejs.org/en/download)

Once you have Node.js installed, you can download or clone this repository and do the following:

```shell
# Install Hardhat:
npm i -D hardhat

# Run this, and click enter 4 times:
npx hardhat

# Install Hardhat dependencies:
npm i -D @nomiclabs/hardhat-waffle
npm install --save-dev @nomicfoundation/hardhat-chai-matchers

# Test ERC20 Permit with offchain approval:
npx hardhat test test/erc20-permit.js
```
