# ERC20 Offchain Token Approval

This ERC20 token has the ability to reduce gas spending when using the transferFrom function by approving a contract's spending and doing the token transferFrom in 1 transaction. Standard ERC20 tokens will need to do this in 2 separate transactions.

To test this, you can download or clone this repository and do the following:

```shell
# Install Hardhat
npm i -D hardhat

# Run this, and click enter 4 times:
npx hardhat

# Install Hardhat dependencies
npm i -D @nomiclabs/hardhat-waffle
npm install --save-dev @nomicfoundation/hardhat-chai-matchers

# Test ERC20 Permit
npx hardhat test test/erc20-permit.js
```
