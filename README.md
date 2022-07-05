# Ethereum Smart Contracts, Tokens and Dapps - Project Starter

**PROJECT: Decentralized Star Notary Service Project** - For this project, you will create a DApp by adding functionality with your smart contract and deploy it on the public testnet.

### ToDo

The purpose of this project is to develop familiarity with building a decentralized app (DAPP) on Ethereum. In the course, we created v1 of the Star Notary app which used the ERC721 interface to declare a non-fungible token. Previously, we added functions in our StarNotary.sol contract to (i) create a star, (ii) put a star up for sale, and (iii) buy a star.

In this project, we extended the functionality of the dApp by adding a name and symbol to our token and adding additional functionality including:

- looking up the given name of a star given its token id
- exchanging two stars between two owners
- transfering a star from one user to another user

### Submission Information

1. My ERC-721 Token Name: Life With Crypto Coin
2. My ERC-721 Token Symbol: LWC
3. Version of the Truffle and OpenZeppelin used: Truffle v5.5.17 (core: 5.5.17) | OpenZeppelin version 2.3
## The contract passed all the test but failed to deploy on Rinkeby so I use my development contract address
## I understand the concept but it seems like my Ubuntu for windows is having issues using old versions of the libraries
## I added a screenshot of the failed error in the screenshot folder
## Also added the passed test screenshot
4. My “Token Address” on the Rinkeby Network: 0x147637c2D3AfB5312B2D37028beB63970b532747

### Dependencies

For this project, you will need to have:

1. **Node and NPM** installed - NPM is distributed with [Node.js](https://www.npmjs.com/get-npm)

```bash
# Check Node version
node -v
# Check NPM version
npm -v
```

2. **Truffle v5.X.X** - A development framework for Ethereum.

```bash
# Unsinstall any previous version
npm uninstall -g truffle
# Install
npm install -g truffle
# Verify the version
truffle version
```

2. **Metamask: 5.3.1** - If you need to update Metamask just delete your Metamask extension and install it again.

3. [Ganache](https://www.trufflesuite.com/ganache) - Make sure that your Ganache and Truffle configuration file have the same port.

4. **Other mandatory packages**:

```bash
cd app
# install packages
npm install --save  openzeppelin-solidity@2.3
npm install --save  truffle-hdwallet-provider@1.0.17
npm install webpack-dev-server -g
npm install web3
```

### Run the application

1. Clean the frontend

```bash
cd app
# Remove the node_modules
# remove packages
rm -rf node_modules
# clean cache
npm cache clean
rm package-lock.json
# initialize npm (you can accept defaults)
npm init
# install all modules listed as dependencies in package.json
npm install
```

2. Start Truffle by running

```bash
# install all modules listed as dependencies in package.json
npm install

# For starting the development console
truffle develop
# truffle console

# For compiling the contract, inside the development console, run:
compile

# For migrating the contract to the locally running Ethereum network, inside the development console
migrate --reset

# For running unit tests the contract, inside the development console, run:
test
```

3. Frontend - Once you are ready to start your frontend, run the following from the app folder:

```bash
cd app
npm run dev
```

---

### Important

When you will add a new Rinkeyby Test Network in your Metamask client, you will have to provide:

| Network Name      | New RPC URL              | Chain ID |
| ----------------- | ------------------------ | -------- |
| Localhost 8545 | `http://127.0.0.1:7545/` | 1337     |
